## WAM_AAC_Titles_v2_11-2016.xml

### PyTransforms
#### _ObjectLabel_
From column: _Root / ObjRecord / ObjectID_
``` python
return getValue("ObjectID")
```

#### _ObjectURI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "id/object/" + getValue("ObjectID")
```

#### _TitleIDURI_
From column: _Root / ObjRecord / Titles / Title / TitleID_
``` python
return "title/" + getValue("TitleID")
```

#### _IdURI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "id/" + getValue("ObjectID")
```

#### _TitleTypeURI_
From column: _Root / ObjRecord / Titles / Title / TitleType_
``` python
def cleanURI(prefix, value):
    uri_value = value.lower().replace(' ', '_')
    return UM.uri_from_fields(prefix + uri_value)

titleTypePrefix = 'title_type/'
titleType = getValue('TitleType')
if titleType:
    return cleanURI(titleTypePrefix,titleType)
else:
    return ""
```

#### _Title_IDURI_
From column: _Root / ObjRecord / Titles / Title / TitleID_
``` python
return getValue("TitleIDURI")
```


### Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _AppellationURI_ | `uri` | `crm:E82_Actor_Appellation1`|
| _AppellationValue_ | `rdf:value` | `crm:E82_Actor_Appellation1`|
| _Biography_ | `rdf:value` | `crm:E33_Linguistic_Object1`|
| _ClassificationURI_ | `uri` | `crm:E17_Type_Assignment1`|
| _ConstituentURI_ | `uri` | `crm:E39_Actor1`|
| _CreditLine_ | `rdf:value` | `crm:E33_Linguistic_Object3`|
| _CreditLineURI_ | `uri` | `crm:E33_Linguistic_Object3`|
| _Dated_ | `rdfs:label` | `crm:E52_Time-Span1`|
| _DisplayName_ | `rdfs:label` | `crm:E39_Actor1`|
| _DuplicatePublicDescription_ | `dc:description` | `crm:E22_Man-Made_Object1`|
| _ExhBeginISODate_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span1`|
| _ExhEndISODate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span1`|
| _ExhTitle_ | `rdfs:label` | `crm:E41_Appellation1`|
| _ExhTitle_ | `rdf:value` | `crm:E41_Appellation1`|
| _ExhVenueURI_ | `uri` | `crm:E93_Presence1`|
| _ExhibCitation_ | `crm:P3_has_note` | `crm:E33_Linguistic_Object1`|
| _ExhibCitationURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _ExhibitionTimeSpanURI_ | `uri` | `crm:E52_Time-Span1`|
| _ExhibitionTitleURI_ | `uri` | `crm:E41_Appellation1`|
| _ExhibitionURI_ | `uri` | `crm:E5_Event1`|
| _ExhibitionURI_ | `uri` | `crm:E7_Activity1`|
| _GeographyID_ | `rdfs:label` | `crm:E42_Identifier2`|
| _GeographyTerm_ | `rdfs:label` | `crm:E48_Place_Name1`|
| _IdURI_ | `uri` | `crm:E42_Identifier1`|
| _Latitude_ | `rdf:value` | `crm:E47_Spatial_Coordinates2`|
| _Longitude_ | `rdf:value` | `crm:E47_Spatial_Coordinates3`|
| _Medium_ | `rdf:value` | `crm:E33_Linguistic_Object2`|
| _MediumURI_ | `uri` | `crm:E33_Linguistic_Object2`|
| _ObjectID_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectID_ | `rdf:value` | `crm:E42_Identifier1`|
| _ObjectID_ | `rdf:value` | `crm:E42_Identifier2`|
| _ObjectID_GeographyID_ | `uri` | `crm:E11_Modification1`|
| _ObjectLabel_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectLabel_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ObjectURI_ | `uri` | `crm:E42_Identifier1`|
| _PlaceURI_ | `uri` | `crm:E53_Place1`|
| _PrimaryTitleType_ | `crm:P2_has_type` | `crm:E35_Title1`|
| _PrimaryTitleType_ | `crm:P2_has_type` | `crm:E42_Identifier2`|
| _ResourceURI_ | `uri` | `foaf:Document1`|
| _ResourceURL_ | `rdfs:label` | `foaf:Document1`|
| _SpatialCoOrdinates_ | `rdfs:label` | `crm:E47_Spatial_Coordinates1`|
| _TGNTermID_ | `rdfs:label` | `crm:E42_Identifier3`|
| _TGNTermIDURI_ | `uri` | `crm:E42_Identifier3`|
| _TGN_Place_ | `skos:exactMatch` | `crm:E53_Place1`|
| _Title_ | `rdfs:label` | `crm:E22_Man-Made_Object1`|
| _Title_ | `rdf:value` | `crm:E35_Title1`|
| _Title_ | `rdf:value` | `crm:E35_Title1`|
| _Title_ | `rdfs:label` | `crm:E35_Title1`|
| _TitleID_ | `rdf:value` | `crm:E42_Identifier2`|
| _TitleID_ | `rdf:value` | `crm:E42_Identifier1`|
| _TitleIDURI_ | `uri` | `crm:E35_Title1`|
| _TitleType_ | `skos:prefLabel` | `crm:E55_Type1`|
| _TitleType_ | `rdfs:label` | `crm:E55_Type1`|
| _TitleType_ | `skos:prefLabel` | `crm:E55_Type1`|
| _TitleTypeURI_ | `uri` | `crm:E55_Type1`|
| _TitleTypeURI_ | `uri` | `crm:E55_Type1`|
| _TitleURI_ | `uri` | `crm:E35_Title1`|
| _TitleURI_ | `uri` | `crm:E35_Title1`|
| _Title_IDURI_ | `uri` | `crm:E42_Identifier2`|
| _Title_IDURI_ | `uri` | `crm:E42_Identifier2`|
| _Type_Latitude_ | `crm:P2_has_type` | `crm:E47_Spatial_Coordinates2`|
| _Type_Longitude_ | `crm:P2_has_type` | `crm:E47_Spatial_Coordinates3`|
| _Type_PreferredTerm_ | `skos:broadMatch` | `crm:E55_Type1`|
| _Type_UniqueId_ | `crm:P2_has_type` | `crm:E42_Identifier1`|
| _VenueBegDate_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span2`|
| _VenueDisplayName_ | `rdfs:label` | `crm:E93_Presence1`|
| _VenueEndDate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span2`|
| _birthPlace_ | `rdfs:label` | `crm:E53_Place1`|
| _productionURI_ | `uri` | `crm:E12_Production1`|


### Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E22_Man-Made_Object1` | `crm:P102_has_title` | `crm:E35_Title1`|
| `crm:E22_Man-Made_Object1` | `crm:P1_is_identified_by` | `crm:E42_Identifier1`|
| `crm:E35_Title1` | `crm:P1_is_identified_by` | `crm:E42_Identifier2`|
| `crm:E35_Title1` | `crm:P2_has_type` | `crm:E55_Type1`|
| `crm:E42_Identifier1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404621`|
| `crm:E42_Identifier2` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404012`|

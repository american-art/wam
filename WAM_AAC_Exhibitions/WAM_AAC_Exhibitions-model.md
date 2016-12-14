## WAM_AAC_Exhibitions.xml

### PyTransforms
#### _ExhibitionURI_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / ExhibitionURI_
``` python
exhibitID = getValue("ExhibitionID")
if exhibitID != "":
    return "id/exhibition/" + exhibitID
else:
    return ""
```

#### _ExhibitionAppellationURI_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / ExhibitionAppellationURI_
``` python
return getValue("ExhibitionURI") + "/appellation"
```

#### _ExhibitionTimeSpanURI_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / ExhibitionTimeSpanURI_
``` python
return getValue("ExhibitionURI") + "/time_span"
```

#### _ObjectURI_
From column: _Root / ObjRecord / ObjectURI_
``` python
return "id/object/"+getValue("ObjectID")
```

#### _ExhibCitationURI_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / ExhibCitationURI_
``` python
return getValue("ExhibitionURI")+"/citation"
```

#### _ExhVenueURI_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / ExhVenues / ExhVenues / ExhVenueURI_
``` python
def cleanURI(prefix, value):
    uri_value = value.lower().replace(' ', '_')
    return UM.uri_from_fields(prefix + uri_value)

venue = getValue("VenueDisplayName")
if venue:
    prefix = getValue("ExhibitionURI") + "/venue/"
    return cleanURI(prefix, venue)
else:
    return ""
```

#### _ObjectID_Val_
From column: _Root / ObjRecord / ObjectID_Val_
``` python
return getValue("ObjectID")
```

#### _ObjectID_URI_
From column: _Root / ObjRecord / ObjectID_Val_
``` python
return getValue("ObjectURI")
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
| _ExhBeginISODate_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span1`|
| _ExhEndISODate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span1`|
| _ExhEndISODate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span1`|
| _ExhTitle_ | `rdfs:label` | `crm:E41_Appellation1`|
| _ExhTitle_ | `rdf:value` | `crm:E41_Appellation1`|
| _ExhTitle_ | `rdf:value` | `crm:E41_Appellation1`|
| _ExhVenueURI_ | `uri` | `crm:E93_Presence1`|
| _ExhVenueURI_ | `uri` | `crm:E93_Presence1`|
| _ExhibCitation_ | `crm:P3_has_note` | `crm:E33_Linguistic_Object1`|
| _ExhibCitation_ | `crm:P3_has_note` | `crm:E33_Linguistic_Object1`|
| _ExhibCitationURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _ExhibCitationURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _ExhibitionAppellationURI_ | `uri` | `crm:E41_Appellation1`|
| _ExhibitionID_ | `rdfs:label` | `crm:E42_Identifier2`|
| _ExhibitionTimeSpanURI_ | `uri` | `crm:E52_Time-Span1`|
| _ExhibitionTimeSpanURI_ | `uri` | `crm:E52_Time-Span1`|
| _ExhibitionTitleURI_ | `uri` | `crm:E41_Appellation1`|
| _ExhibitionURI_ | `uri` | `crm:E5_Event1`|
| _ExhibitionURI_ | `uri` | `crm:E7_Activity1`|
| _ExhibitionURI_ | `uri` | `crm:E5_Event1`|
| _GeographyID_ | `rdfs:label` | `crm:E42_Identifier2`|
| _GeographyTerm_ | `rdfs:label` | `crm:E48_Place_Name1`|
| _Latitude_ | `rdf:value` | `crm:E47_Spatial_Coordinates2`|
| _Longitude_ | `rdf:value` | `crm:E47_Spatial_Coordinates3`|
| _Medium_ | `rdf:value` | `crm:E33_Linguistic_Object2`|
| _MediumURI_ | `uri` | `crm:E33_Linguistic_Object2`|
| _ObjectID_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectID_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectID_ | `rdf:value` | `crm:E42_Identifier2`|
| _ObjectID_GeographyID_ | `uri` | `crm:E11_Modification1`|
| _ObjectID_URI_ | `uri` | `crm:E42_Identifier1`|
| _ObjectID_Val_ | `rdf:value` | `crm:E42_Identifier1`|
| _ObjectLabel_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ObjectURI_ | `uri` | `crm:E42_Identifier1`|
| _PlaceURI_ | `uri` | `crm:E53_Place1`|
| _PreferredLabel_ | `skos:prefLabel` | `crm:E55_Type1`|
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
| _Title_ | `rdfs:label` | `crm:E35_Title1`|
| _TitleID_ | `rdf:value` | `crm:E42_Identifier1`|
| _TitleType_ | `rdfs:label` | `crm:E55_Type1`|
| _TitleType_ | `skos:prefLabel` | `crm:E55_Type1`|
| _TitleTypeURI_ | `uri` | `crm:E55_Type1`|
| _TitleURI_ | `uri` | `crm:E35_Title1`|
| _TitleURI_ | `uri` | `crm:E35_Title1`|
| _Title_IDURI_ | `uri` | `crm:E42_Identifier2`|
| _Type_Latitude_ | `crm:P2_has_type` | `crm:E47_Spatial_Coordinates2`|
| _Type_Longitude_ | `crm:P2_has_type` | `crm:E47_Spatial_Coordinates3`|
| _Type_PreferredTerm_ | `skos:broadMatch` | `crm:E55_Type1`|
| _Type_UniqueId_ | `crm:P2_has_type` | `crm:E42_Identifier1`|
| _VenueBegDate_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span2`|
| _VenueBegDate_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span2`|
| _VenueDisplayName_ | `rdfs:label` | `crm:E93_Presence1`|
| _VenueDisplayName_ | `rdfs:label` | `crm:E93_Presence1`|
| _VenueEndDate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span2`|
| _VenueEndDate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span2`|
| _birthPlace_ | `rdfs:label` | `crm:E53_Place1`|
| _productionURI_ | `uri` | `crm:E12_Production1`|


### Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E22_Man-Made_Object1` | `crm:P12i_was_present_at` | `crm:E5_Event1`|
| `crm:E22_Man-Made_Object1` | `crm:P1_is_identified_by` | `crm:E42_Identifier1`|
| `crm:E33_Linguistic_Object1` | `crm:P129_is_about` | `crm:E5_Event1`|
| `crm:E41_Appellation1` | `crm:P2_has_type` | `crm:E55_Type1`|
| `crm:E42_Identifier1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404621`|
| `crm:E55_Type1` | `skos:broadMatch` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `crm:E5_Event1` | `crm:P1_is_identified_by` | `crm:E41_Appellation1`|
| `crm:E5_Event1` | `crm:P4_has_time-span` | `crm:E52_Time-Span1`|
| `crm:E5_Event1` | `crm:P166i_had_presence` | `crm:E93_Presence1`|
| `crm:E5_Event1` | `crm:P48_has_preferred_identifier` | `crm:E42_Identifier2`|
| `crm:E93_Presence1` | `crm:P164_during` | `crm:E52_Time-Span2`|
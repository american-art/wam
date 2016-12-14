## WAM_XMLExport_AAC_Objects.xml

### PyTransforms
#### _ObjectLabel_
From column: _Root / ObjRecord / ObjectID_
``` python
return getValue("ObjectID")
```

#### _DuplicatePublicDescription_
From column: _Root / ObjRecord / PublicDescription_
``` python
return getValue("PublicDescription")
```

#### _ResourceURI_
From column: _Root / ObjRecord / ResourceURL_
``` python
return getValue("ResourceURL")

```

#### _ObjectID_URI_
From column: _Root / ObjRecord / ObjUnderJurisOf_
``` python
return "id/object/" + getValue("ObjectID")
```

#### _IdURI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "id/" + getValue("ObjectID")
```

#### _MediumURI_
From column: _Root / ObjRecord / PhysicalDescription / Medium_
``` python
return getValue("ObjectID_URI") + "/medium" 
```

#### _Classification_
From column: _Root / ObjRecord / Classification_
``` python
return getValue("Classification")
```

#### _ClassificationURI_
From column: _Root / ObjRecord / Classification_
``` python
return getValue("ObjectID_URI") + "/classification/" 
```

#### _CreditLineURI_
From column: _Root / ObjRecord / CreditLine_
``` python
return getValue("ObjectID_URI") + "/creditLine/"
```

#### _CurrentLocationURI_
From column: _Root / ObjRecord / CurrentLocation_
``` python
return getValue("ObjectID_URI") + "/currentLocation/"
```

#### _PublicDescriptionURI_
From column: _Root / ObjRecord / PublicDescription_
``` python
return getValue("ObjectID_URI") + "/publicDescription/"
```

#### _DateURI_
From column: _Root / ObjRecord / Dated_
``` python
return getValue("ObjectID_URI") + "/date/"
```

#### _TermURI_
From column: _Root / ObjRecord / PhysicalDescription / PhysicalDescriptionTerms / SourceTermID_
``` python
sourceId = getValue("SourceTermID")
if sourceId:
    return "http://vocab.getty.edu/aat/" + sourceId
else:
    return ""
```


### Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _AppellationURI_ | `uri` | `crm:E82_Actor_Appellation1`|
| _AppellationValue_ | `rdf:value` | `crm:E82_Actor_Appellation1`|
| _Biography_ | `rdf:value` | `crm:E33_Linguistic_Object1`|
| _Classification_ | `rdfs:label` | `crm:E55_Type1`|
| _ClassificationURI_ | `uri` | `crm:E17_Type_Assignment1`|
| _ClassificationURI_ | `uri` | `crm:E17_Type_Assignment1`|
| _ConstituentURI_ | `uri` | `crm:E39_Actor1`|
| _CreditLine_ | `rdf:value` | `crm:E33_Linguistic_Object3`|
| _CreditLine_ | `rdf:value` | `crm:E33_Linguistic_Object2`|
| _CreditLineURI_ | `uri` | `crm:E33_Linguistic_Object3`|
| _CreditLineURI_ | `uri` | `crm:E33_Linguistic_Object2`|
| _CurrentLocation_ | `rdfs:label` | `crm:E53_Place1`|
| _CurrentLocationURI_ | `uri` | `crm:E53_Place1`|
| _DateBegin_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span1`|
| _DateEnd_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span1`|
| _DateURI_ | `uri` | `crm:E12_Production1`|
| _Dated_ | `rdfs:label` | `crm:E52_Time-Span1`|
| _Dated_ | `rdfs:label` | `crm:E52_Time-Span1`|
| _DisplayName_ | `rdfs:label` | `crm:E39_Actor1`|
| _DuplicatePublicDescription_ | `dc:description` | `crm:E22_Man-Made_Object1`|
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
| _Medium_ | `rdf:value` | `crm:E33_Linguistic_Object3`|
| _Medium_ | `rdf:value` | `crm:E33_Linguistic_Object2`|
| _MediumURI_ | `uri` | `crm:E33_Linguistic_Object2`|
| _MediumURI_ | `uri` | `crm:E33_Linguistic_Object3`|
| _ObjectID_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectID_ | `rdf:value` | `crm:E42_Identifier1`|
| _ObjectID_ | `rdf:value` | `crm:E42_Identifier2`|
| _ObjectID_GeographyID_ | `uri` | `crm:E11_Modification1`|
| _ObjectID_URI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ObjectLabel_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectLabel_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ObjectURI_ | `uri` | `crm:E42_Identifier1`|
| _PlaceURI_ | `uri` | `crm:E53_Place1`|
| _PrimaryTitleType_ | `crm:P2_has_type` | `crm:E35_Title1`|
| _PrimaryTitleType_ | `crm:P2_has_type` | `crm:E42_Identifier2`|
| _PublicDescription_ | `rdf:value` | `crm:E33_Linguistic_Object1`|
| _PublicDescriptionURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _ResourceURI_ | `uri` | `foaf:Document1`|
| _ResourceURI_ | `uri` | `foaf:Document1`|
| _ResourceURL_ | `rdfs:label` | `foaf:Document1`|
| _ResourceURL_ | `rdfs:label` | `foaf:Document1`|
| _SpatialCoOrdinates_ | `rdfs:label` | `crm:E47_Spatial_Coordinates1`|
| _TGNTermID_ | `rdfs:label` | `crm:E42_Identifier3`|
| _TGNTermIDURI_ | `uri` | `crm:E42_Identifier3`|
| _TGN_Place_ | `skos:exactMatch` | `crm:E53_Place1`|
| _Term_ | `rdfs:label` | `owl:Thing1`|
| _TermURI_ | `uri` | `owl:Thing1`|
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
| _VenueDisplayName_ | `rdfs:label` | `crm:E93_Presence1`|
| _VenueEndDate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span2`|
| _birthPlace_ | `rdfs:label` | `crm:E53_Place1`|
| _productionURI_ | `uri` | `crm:E12_Production1`|


### Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E12_Production1` | `crm:P4_has_time-span` | `crm:E52_Time-Span1`|
| `crm:E17_Type_Assignment1` | `crm:P42_assigned` | `crm:E55_Type1`|
| `crm:E17_Type_Assignment1` | `crm:P21_had_general_purpose` | `xsd:http://vocab.getty.edu/aat/300179869`|
| `crm:E22_Man-Made_Object1` | `crm:P108i_was_produced_by` | `crm:E12_Production1`|
| `crm:E22_Man-Made_Object1` | `crm:P41i_was_classified_by` | `crm:E17_Type_Assignment1`|
| `crm:E22_Man-Made_Object1` | `crm:P129i_is_subject_of` | `crm:E33_Linguistic_Object1`|
| `crm:E22_Man-Made_Object1` | `crm:P67i_is_referred_to_by` | `crm:E33_Linguistic_Object2`|
| `crm:E22_Man-Made_Object1` | `crm:P67i_is_referred_to_by` | `crm:E33_Linguistic_Object3`|
| `crm:E22_Man-Made_Object1` | `crm:P1_is_identified_by` | `crm:E42_Identifier1`|
| `crm:E22_Man-Made_Object1` | `crm:P55_has_current_location` | `crm:E53_Place1`|
| `crm:E22_Man-Made_Object1` | `crm:P62_depicts` | `owl:Thing1`|
| `crm:E22_Man-Made_Object1` | `foaf:homepage` | `foaf:Document1`|
| `crm:E22_Man-Made_Object1` | `crm:P2_has_type` | `crm:E55_Type1`|
| `crm:E33_Linguistic_Object1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `crm:E33_Linguistic_Object1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300080091`|
| `crm:E33_Linguistic_Object2` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300026687`|
| `crm:E33_Linguistic_Object3` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300264237`|
| `crm:E42_Identifier1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404621`|

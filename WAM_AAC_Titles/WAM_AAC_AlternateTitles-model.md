## WAM_AAC_Titles.xml

### PyTransforms
#### _ObjectURI_
From column: _Root / ObjRecord / ObjectURI_
``` python
return "object/" + getValue("ObjectID")
```


### Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _ExhBeginISODate_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span1`|
| _ExhEndISODate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span1`|
| _ExhTitle_ | `rdfs:label` | `crm:E41_Appellation1`|
| _ExhVenueURI_ | `uri` | `crm:E93_Presence1`|
| _ExhibCitation_ | `crm:P3_has_note` | `crm:E33_Linguistic_Object1`|
| _ExhibCitationURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _ExhibitionTimeSpanURI_ | `uri` | `crm:E52_Time-Span1`|
| _ExhibitionTitleURI_ | `uri` | `crm:E41_Appellation1`|
| _ExhibitionURI_ | `uri` | `crm:E7_Activity1`|
| _GeographyID_ | `rdfs:label` | `crm:E42_Identifier2`|
| _GeographyTerm_ | `rdfs:label` | `crm:E48_Place_Name1`|
| _ObjectID_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectID_ | `rdf:value` | `crm:E42_Identifier2`|
| _ObjectID_ | `rdf:value` | `crm:E42_Identifier2`|
| _ObjectID_GeographyID_ | `uri` | `crm:E11_Modification1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ObjectURI_ | `uri` | `crm:E42_Identifier1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _PlaceURI_ | `uri` | `crm:E53_Place1`|
| _PrimaryTitleType_ | `crm:P2_has_type` | `crm:E35_Title1`|
| _PrimaryTitleType_ | `crm:P2_has_type` | `crm:E42_Identifier2`|
| _SpatialCoOrdinates_ | `rdfs:label` | `crm:E47_Spatial_Coordinates1`|
| _TGNTermID_ | `rdfs:label` | `crm:E42_Identifier3`|
| _TGNTermIDURI_ | `uri` | `crm:E42_Identifier3`|
| _Title_ | `rdfs:label` | `crm:E22_Man-Made_Object1`|
| _Title_ | `rdf:value` | `crm:E35_Title1`|
| _Title_ | `rdfs:label` | `crm:E35_Title1`|
| _Title_ | `rdf:value` | `crm:E35_Title1`|
| _TitleID_ | `rdf:value` | `crm:E42_Identifier1`|
| _TitleType_ | `skos:prefLabel` | `crm:E55_Type1`|
| _TitleType_ | `rdfs:label` | `crm:E55_Type1`|
| _TitleTypeURI_ | `uri` | `crm:E55_Type1`|
| _TitleURI_ | `uri` | `crm:E35_Title1`|
| _TitleURI_ | `uri` | `crm:E35_Title1`|
| _Type_UniqueId_ | `crm:P2_has_type` | `crm:E42_Identifier1`|
| _VenueBegDate_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span2`|
| _VenueDisplayName_ | `rdfs:label` | `crm:E93_Presence1`|
| _VenueEndDate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span2`|


### Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E22_Man-Made_Object1` | `crm:P102_has_title` | `crm:E35_Title1`|
| `crm:E22_Man-Made_Object1` | `crm:P48_has_preferred_identifier` | `crm:E42_Identifier2`|
| `crm:E35_Title1` | `crm:P2_has_type` | `crm:E55_Type1`|

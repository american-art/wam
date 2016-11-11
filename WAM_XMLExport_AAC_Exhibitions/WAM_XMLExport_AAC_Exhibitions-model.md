## WAM_XMLExport_AAC_Exhibitions.xml

### PyTransforms
#### _ExhibitionURI_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / ExhibitionURI_
``` python
exhibitID = getValue("ExhibitionID")
if exhibitID != "":
    return "exhibition/" + exhibitID
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
return "object/"+getValue("ObjectID")
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


### Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _ExhBeginISODate_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span1`|
| _ExhBeginISODate_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span1`|
| _ExhEndISODate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span1`|
| _ExhEndISODate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span1`|
| _ExhTitle_ | `rdfs:label` | `crm:E41_Appellation1`|
| _ExhTitle_ | `rdfs:label` | `crm:E41_Appellation1`|
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
| _ExhibitionURI_ | `uri` | `crm:E7_Activity1`|
| _ExhibitionURI_ | `uri` | `crm:E7_Activity1`|
| _GeographyID_ | `rdfs:label` | `crm:E42_Identifier2`|
| _GeographyTerm_ | `rdfs:label` | `crm:E48_Place_Name1`|
| _ObjectID_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectID_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectID_GeographyID_ | `uri` | `crm:E11_Modification1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ObjectURI_ | `uri` | `crm:E42_Identifier1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _PlaceURI_ | `uri` | `crm:E53_Place1`|
| _SpatialCoOrdinates_ | `rdfs:label` | `crm:E47_Spatial_Coordinates1`|
| _TGNTermID_ | `rdfs:label` | `crm:E42_Identifier3`|
| _TGNTermIDURI_ | `uri` | `crm:E42_Identifier3`|
| _Title_ | `rdfs:label` | `crm:E35_Title1`|
| _TitleType_ | `rdfs:label` | `crm:E55_Type1`|
| _TitleTypeURI_ | `uri` | `crm:E55_Type1`|
| _TitleURI_ | `uri` | `crm:E35_Title1`|
| _TitleURI_ | `uri` | `crm:E35_Title1`|
| _VenueBegDate_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span2`|
| _VenueDisplayName_ | `rdfs:label` | `crm:E93_Presence1`|
| _VenueEndDate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span2`|


### Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E22_Man-Made_Object1` | `crm:P12i_was_present_at` | `crm:E7_Activity1`|
| `crm:E22_Man-Made_Object1` | `crm:P48_has_preferred_identifier` | `crm:E42_Identifier1`|
| `crm:E33_Linguistic_Object1` | `crm:P129_is_about` | `crm:E7_Activity1`|
| `crm:E7_Activity1` | `crm:P1_is_identified_by` | `crm:E41_Appellation1`|
| `crm:E7_Activity1` | `crm:P4_has_time-span` | `crm:E52_Time-Span1`|
| `crm:E7_Activity1` | `crm:P166i_had_presence` | `crm:E93_Presence1`|
| `crm:E7_Activity1` | `crm:P48_has_preferred_identifier` | `crm:E42_Identifier2`|
| `crm:E93_Presence1` | `crm:P164_during` | `crm:E52_Time-Span2`|

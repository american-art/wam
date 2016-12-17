# WAM_XMLExport_AAC_Exhibitions.xml

## Add Column
#### _ExhibitionURI_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / ExhibitionID_
<br/>Value: ``

#### _ExhibitionAppellationURI_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / ExhTitle_
<br/>Value: ``

#### _ExhibitionTimeSpanURI_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / ExhEndISODate_
<br/>Value: ``

#### _ObjectURI_
From column: _Root / ObjRecord / ObjectID_
<br/>Value: ``

#### _ExhibCitationURI_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / ExhibCitation_
<br/>Value: ``

#### _ExhVenueURI_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / ExhVenues / ExhVenues / VenueDisplayName_
<br/>Value: ``

#### _Type_PreferredTerm_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / ExhibitionAppellationURI_
<br/>Value: `<http://vocab.getty.edu/aat/300404670>`

#### _PreferredLabel_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / Type_PreferredTerm_
<br/>Value: `Exhibition`

#### _Type_RepositryNo_
From column: _Root / ObjRecord / ObjectID_
<br/>Value: `<http://vocab.getty.edu/aat/300404621>`

#### _ObjectID_Val_
From column: _Root / ObjRecord / ObjectID_
<br/>Value: ``


## Add Node/Literal
#### Literal Node: `http://vocab.getty.edu/aat/300404621`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300404670`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _ExhibitionURI_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / ExhibitionURI_
``` python
exhibitID = getValue("ExhibitionID")
if exhibitID != "":
    return "exhibition/id/" + exhibitID
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
return "object/id/"+getValue("ObjectID")
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

#### _VenueDateURI_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / ExhVenues / ExhVenues / VenueEndDate_
``` python
begin = getValue("VenueBegDate")
if begin:
    return getValue("ExhVenueURI") + "/date/"
else:
    return ""
```


## Selections
#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Exhibitions / Exhibitions / ExhEndISODate_
<br>Operation: `Union`
``` python
return getValue("ExhibitionID") == ""
```


## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _ExhBeginISODate_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span1`|
| _ExhEndISODate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span1`|
| _ExhTitle_ | `rdf:value` | `crm:E41_Appellation1`|
| _ExhVenueURI_ | `uri` | `crm:E93_Presence1`|
| _ExhibCitation_ | `crm:P3_has_note` | `crm:E33_Linguistic_Object1`|
| _ExhibCitationURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _ExhibitionAppellationURI_ | `uri` | `crm:E41_Appellation1`|
| _ExhibitionID_ | `rdfs:label` | `crm:E42_Identifier2`|
| _ExhibitionTimeSpanURI_ | `uri` | `crm:E52_Time-Span1`|
| _ExhibitionURI_ | `uri` | `crm:E5_Event1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _PreferredLabel_ | `skos:prefLabel` | `crm:E55_Type1`|
| _VenueBegDate_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span2`|
| _VenueDateURI_ | `uri` | `crm:E52_Time-Span2`|
| _VenueDisplayName_ | `rdfs:label` | `crm:E93_Presence1`|
| _VenueEndDate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span2`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E22_Man-Made_Object1` | `crm:P12i_was_present_at` | `crm:E5_Event1`|
| `crm:E41_Appellation1` | `crm:P2_has_type` | `crm:E55_Type1`|
| `crm:E55_Type1` | `skos:broadMatch` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `crm:E5_Event1` | `crm:P129_is_about` | `crm:E33_Linguistic_Object1`|
| `crm:E5_Event1` | `crm:P1_is_identified_by` | `crm:E41_Appellation1`|
| `crm:E5_Event1` | `crm:P48_has_preferred_identifier` | `crm:E42_Identifier2`|
| `crm:E5_Event1` | `crm:P4_has_time-span` | `crm:E52_Time-Span1`|
| `crm:E5_Event1` | `crm:P166i_had_presence` | `crm:E93_Presence1`|
| `crm:E93_Presence1` | `crm:P164_during` | `crm:E52_Time-Span2`|

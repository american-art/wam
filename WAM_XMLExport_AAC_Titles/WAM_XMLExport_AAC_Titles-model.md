## WAM_XMLExport_AAC_Titles.xml

### PyTransforms
#### _TitleType_
From column: _Root / ObjRecord / Titles / Title / TitleType_
``` python
givenTitleType = getValue("TitleType")
if givenTitleType == "":
    titleType = "Alternate"
elif givenTitleType == "(not entered)":
    titleType = "Title"
else:
    titleType = givenTitleType
return titleType
```

#### _TitleTypeURI_
From column: _Root / ObjRecord / Titles / Title / TitleTypeURI_
``` python
def cleanURI(prefix, value):
    uri_value = value.lower().replace(' ', '_')
    return UM.uri_from_fields(prefix + uri_value)

titleTypePrefix = "thesauri/title_type/"
titleType = getValue("TitleType")
return cleanURI(titleTypePrefix, titleType)
```

#### _TitleIDURI_
From column: _Root / ObjRecord / Titles / Title / TitleIDURI_
``` python
def cleanURI(prefix, value):
    uri_value = value.lower().replace(' ', '_')
    return UM.uri_from_fields(prefix + uri_value)

titlePrefix = cleanURI("thesauri/", getValue("TitleType")) + "/"
titleID = getValue("TitleID")
return cleanURI(titlePrefix, titleID)
```

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
| _ExhibitionTimeSpanURI_ | `uri` | `crm:E52_Time-Span1`|
| _ExhibitionTitleURI_ | `uri` | `crm:E41_Appellation1`|
| _ExhibitionURI_ | `uri` | `crm:E7_Activity1`|
| _GeographyTerm_ | `rdfs:label` | `crm:E48_Place_Name1`|
| _ObjectID_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectID_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ObjectURI_ | `uri` | `crm:E42_Identifier1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _PlaceURI_ | `uri` | `crm:E53_Place1`|
| _SpatialCoOrdinates_ | `rdfs:label` | `crm:E47_Spatial_Coordinates1`|
| _Title_ | `rdfs:label` | `crm:E35_Title1`|
| _Title_ | `rdfs:label` | `crm:E35_Title1`|
| _TitleIDURI_ | `uri` | `crm:E35_Title1`|
| _TitleType_ | `rdfs:label` | `crm:E55_Type1`|
| _TitleType_ | `rdfs:label` | `crm:E55_Type1`|
| _TitleTypeURI_ | `uri` | `crm:E55_Type1`|
| _TitleTypeURI_ | `uri` | `crm:E55_Type1`|
| _TitleURI_ | `uri` | `crm:E35_Title1`|
| _TitleURI_ | `uri` | `crm:E35_Title1`|


### Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E22_Man-Made_Object1` | `crm:P102_has_title` | `crm:E35_Title1`|
| `crm:E22_Man-Made_Object1` | `crm:P48_has_preferred_identifier` | `crm:E42_Identifier1`|
| `crm:E35_Title1` | `crm:P2_has_type` | `crm:E55_Type1`|

# WAM_AAC_Titles_v2_11-2016.xml

## Add Column

## Add Node/Literal
#### Literal Node: `<http://vocab.getty.edu/aat/300404621>`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `<http://vocab.getty.edu/aat/300404012>`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300404621`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300404012`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `"http://vocab.getty.edu/aat/300404621"`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
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


## Selections
#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Titles / Title / Title_
<br>Operation: `Union`
``` python
titleType = getValue("TitleType")
return titleType == "Title" or titleType == ""
```


## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _IdURI_ | `uri` | `crm:E42_Identifier1`|
| _ObjectID_ | `rdf:value` | `crm:E42_Identifier1`|
| _ObjectLabel_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _Title_ | `rdf:value` | `crm:E35_Title1`|
| _TitleID_ | `rdf:value` | `crm:E42_Identifier2`|
| _TitleIDURI_ | `uri` | `crm:E35_Title1`|
| _TitleType_ | `skos:prefLabel` | `crm:E55_Type1`|
| _TitleTypeURI_ | `uri` | `crm:E55_Type1`|
| _Title_IDURI_ | `uri` | `crm:E42_Identifier2`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E22_Man-Made_Object1` | `crm:P102_has_title` | `crm:E35_Title1`|
| `crm:E22_Man-Made_Object1` | `crm:P1_is_identified_by` | `crm:E42_Identifier1`|
| `crm:E35_Title1` | `crm:P1_is_identified_by` | `crm:E42_Identifier2`|
| `crm:E35_Title1` | `crm:P2_has_type` | `crm:E55_Type1`|
| `crm:E42_Identifier1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404621`|
| `crm:E42_Identifier2` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404012`|

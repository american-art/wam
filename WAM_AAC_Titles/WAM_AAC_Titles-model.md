# WAM_AAC_Titles_v2_11-2016.xml

## Add Column

## Add Node/Literal
#### Literal Node: `http://vocab.getty.edu/aat/300404012`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300404670`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _ObjectLabel_
From column: _Root / ObjRecord / ObjectID_
``` python
return getValue("ObjectID")
```

#### _IdURI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "id/" + getValue("ObjectID")
```

#### _ObjectURI_
From column: _Root / ObjRecord / IdURI_
``` python
return "object/id/" + getValue("ObjectID")
```

#### _Title_IDURI_
From column: _Root / ObjRecord / Titles / Title / TitleID_
``` python
return getValue("TitleIDURI") + "/id/" + getValue("TitleID")
```

#### _TitleLabel_
From column: _Root / ObjRecord / Titles / Title / Title_
``` python
return getValue("Title")
```

#### _TitleIDURI_
From column: _Root / ObjRecord / Titles / Title / Title_IDURI_
``` python
return getValue("ObjectURI") + "/" + getValue("TitleType").lower()
```


## Selections
#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Titles / Title / Title_
<br>Operation: `Union`
``` python
return getValue("TitleType") != "Title"
```


## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _Title_ | `rdf:value` | `crm:E35_Title1`|
| _TitleID_ | `rdf:value` | `crm:E42_Identifier2`|
| _TitleIDURI_ | `uri` | `crm:E35_Title1`|
| _TitleLabel_ | `rdfs:label` | `crm:E22_Man-Made_Object1`|
| _Title_IDURI_ | `uri` | `crm:E42_Identifier2`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E22_Man-Made_Object1` | `crm:P102_has_title` | `crm:E35_Title1`|
| `crm:E35_Title1` | `crm:P1_is_identified_by` | `crm:E42_Identifier2`|
| `crm:E35_Title1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `crm:E42_Identifier2` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404012`|

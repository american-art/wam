# WAM_XMLExport_AAC_Titles_v2_11-2016.xml

## Add Column

## Add Node/Literal
#### Literal Node: `http://vocab.getty.edu/aat/300404670`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300404012`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _ObjectURI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "object/"+getValue("ObjectID")
```

#### _TitleLabel_
From column: _Root / ObjRecord / Titles / Title / Title_
``` python
return getValue("Title")
```

#### _TitleURI_
From column: _Root / ObjRecord / Titles / Title / Title_
``` python
return UM.uri_from_fields("thesauri/title/",getValue("Title"))
```

#### _TitleIdentifier_
From column: _Root / ObjRecord / Titles / Title / TitleDisplayOrder_
``` python
return getValue("ObjectURI")+"/title_identifier"
```


## Selections
#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Titles / Title / TitleType_
<br>Operation: `Union`
``` python
return getValue("TitleDisplayOrder")!='1'
```


## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _Title_ | `rdf:value` | `crm:E35_Title1`|
| _TitleID_ | `rdf:value` | `crm:E42_Identifier1`|
| _TitleIdentifier_ | `uri` | `crm:E42_Identifier1`|
| _TitleLabel_ | `rdfs:label` | `crm:E22_Man-Made_Object1`|
| _TitleURI_ | `uri` | `crm:E35_Title1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E22_Man-Made_Object1` | `crm:P102_has_title` | `crm:E35_Title1`|
| `crm:E35_Title1` | `crm:P1_is_identified_by` | `crm:E42_Identifier1`|
| `crm:E35_Title1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `crm:E42_Identifier1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404012`|

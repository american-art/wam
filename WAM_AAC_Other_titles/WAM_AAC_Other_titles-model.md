# WAM_XMLExport_AAC_Titles_v2_11-2016.xml

## Add Column

## Add Node/Literal

## PyTransforms
#### _ObjectURI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "object/"+getValue("ObjectID")
```

#### _TitleURI_
From column: _Root / ObjRecord / Titles / Title / Title_
``` python
return UM.uri_from_fields("thesauri/title/",getValue("Title"))
```

#### _TitleLabel_
From column: _Root / ObjRecord / Titles / Title / Title_
``` python
return getValue("Title")
```

#### _AlternateTitleType_
From column: _Root / ObjRecord / Titles / Title / TitleID_
``` python
if getValue("TitleType"):
    return getValue("TitleURI")+"/title_type"
else:
    return ""
```


## Selections
#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Titles / Title / TitleType_
<br>Operation: `Union`
``` python
return getValue("TitleDisplayOrder")=='1'
```


## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _AlternateTitleType_ | `uri` | `crm:E55_Type1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _Title_ | `rdf:value` | `crm:E35_Title1`|
| _TitleType_ | `skos:prefLabel` | `crm:E55_Type1`|
| _TitleURI_ | `uri` | `crm:E35_Title1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E22_Man-Made_Object1` | `crm:P102_has_title` | `crm:E35_Title1`|
| `crm:E35_Title1` | `crm:P2_has_type` | `crm:E55_Type1`|

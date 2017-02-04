# WAM_XMLExport_AAC_Constituents_V3.xml

## Add Column

## Add Node/Literal
#### Literal Node: `http://vocab.getty.edu/aat/300015646`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _ObjectURI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "object/"+getValue("ObjectID")
```

#### _CultureURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / CreatorULANID_
``` python
return getValue("ObjectURI")+"/culture"
```

#### _CultureNameURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / CultureURI_
``` python
return getValue("CultureURI")+"/name"
```


## Selections
#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentType_
<br>Operation: `Union`
``` python
return getValue("ConstituentType")!="Culture"
```


## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _CultureNameURI_ | `uri` | `crm:E55_Type1`|
| _CultureURI_ | `uri` | `crm:E17_Type_Assignment1`|
| _DisplayName_ | `rdfs:label` | `crm:E55_Type1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E17_Type_Assignment1` | `crm:P42_assigned` | `crm:E55_Type1`|
| `crm:E17_Type_Assignment1` | `crm:P21_had_general_purpose` | `xsd:http://vocab.getty.edu/aat/300015646`|
| `crm:E22_Man-Made_Object1` | `crm:P41i_was_classified_by` | `crm:E17_Type_Assignment1`|

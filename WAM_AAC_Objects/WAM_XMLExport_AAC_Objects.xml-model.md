# WAM_XMLExport_AAC_Objects.xml

## Add Column

## Add Node/Literal
#### Literal Node: `ttp://vocab.getty.edu/aat/300179869`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `ttp://vocab.getty.edu/aat/300026687`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _ObjectURI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "object/"+getValue("ObjectID")
```

#### _ClassificationURI_
From column: _Root / ObjRecord / Classification_
``` python
return getValue("ObjectURI")+"/classification_type"
```

#### _ClassificationEventURI_
From column: _Root / ObjRecord / Classification_
``` python
return getValue("ObjectURI")+"/classification"
```

#### _CreditLineURI_
From column: _Root / ObjRecord / CreditLine_
``` python
return getValue("ObjectURI")+"/credit_line"
```


## Selections

## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _Classification_ | `rdfs:label` | `crm:E55_Type1`|
| _ClassificationEventURI_ | `uri` | `crm:E17_Type_Assignment1`|
| _ClassificationURI_ | `uri` | `crm:E55_Type1`|
| _CreditLine_ | `rdf:value` | `crm:E33_Linguistic_Object1`|
| _CreditLineURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E17_Type_Assignment1` | `crm:P21_had_general_purpose` | `xsd:ttp://vocab.getty.edu/aat/300179869`|
| `crm:E22_Man-Made_Object1` | `crm:P41i_was_classified_by` | `crm:E17_Type_Assignment1`|
| `crm:E22_Man-Made_Object1` | `crm:P67i_is_referred_to_by` | `crm:E33_Linguistic_Object1`|
| `crm:E22_Man-Made_Object1` | `crm:P62_depicts` | `crm:E39_Actor2`|
| `crm:E22_Man-Made_Object1` | `crm:P129i_is_subject_of` | `crm:E33_Linguistic_Object1`|
| `crm:E33_Linguistic_Object1` | `crm:P2_has_type` | `xsd:ttp://vocab.getty.edu/aat/300026687`|
| `crm:E39_Actor2` | `crm:P2_has_type` | `crm:E55_Type1`|

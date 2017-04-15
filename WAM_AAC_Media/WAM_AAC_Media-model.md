# WAM_XMLExport_AAC_Media_v3.xml

## Add Column

## Add Node/Literal

## PyTransforms
#### _ObjectURI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "object/"+getValue("ObjectID")
```

#### _ImageURL_
From column: _Root / ObjRecord / ObjectRelatedMedia / Media / FullImageURL_
``` python
if getValue("MediaDispRank")=='1':
    return getValue("FullImageURL")
else:
    return ""
```

#### _CreditURI_
From column: _Root / ObjRecord / ObjectRelatedMedia / Media / ImageURL_
``` python
if getValue("ImageURL") and getValue("ImageCredit"):
    return getValue("ImageURL")+"/credit_line"
else:
    return ""
```


## Selections

## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _CreditURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _ImageCredit_ | `rdf:value` | `crm:E33_Linguistic_Object1`|
| _ImageURL_ | `uri` | `crm:E38_Image1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E22_Man-Made_Object1` | `crm:P138i_has_representation` | `crm:E38_Image1`|
| `crm:E38_Image1` | `crm:P67i_is_referred_to_by` | `crm:E33_Linguistic_Object1`|

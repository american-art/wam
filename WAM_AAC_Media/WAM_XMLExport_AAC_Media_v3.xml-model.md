# WAM_XMLExport_AAC_Media_v3.xml

## Add Column

## Add Node/Literal
#### Literal Node: `http://vocab.getty.edu/aat/300055547`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _ObjectID_URI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "object/id/" + getValue("ObjectID")
```

#### _ImageURI_
From column: _Root / ObjRecord / ObjectRelatedMedia / Media / MediaXrefID_
``` python
return getValue("ObjectID_URI") + "/" + getValue("MediaView").lower() + "/media/id/" + getValue("MediaXrefID")
```

#### _ImageRightsURI_
From column: _Root / ObjRecord / ObjectRelatedMedia / Media / ImageRights_
``` python
return getValue("ImageURI") + "/image_rights"
```


## Selections

## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _ImageRights_ | `rdf:value` | `crm:E33_Linguistic_Object1`|
| _ImageRightsURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _ImageURI_ | `uri` | `crm:E38_Image1`|
| _ObjectID_URI_ | `uri` | `crm:E22_Man-Made_Object1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E22_Man-Made_Object1` | `crm:P138i_has_representation` | `crm:E38_Image1`|
| `crm:E33_Linguistic_Object1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300055547`|
| `crm:E38_Image1` | `crm:P67i_is_referred_to_by` | `crm:E33_Linguistic_Object1`|

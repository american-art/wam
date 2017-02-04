# WAM_XMLExport_AAC_Constituents_V3.xml

## Add Column

## Add Node/Literal

## PyTransforms
#### _ConstituentURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentID_
``` python
if getValue("Role") in ['Painter','Artist','Sculptor','Designer','Goldsmith']:
    return "constituent/"+getValue("ConstituentID")
else:
    return ""
```

#### _ObjectURI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "object/"+getValue("ObjectID")
```

#### _ProductionURI_
From column: _Root / ObjRecord / DataDateStamp_
``` python
return getValue("ObjectURI")+"/production"
```


## Selections

## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _ConstituentURI_ | `uri` | `crm:E39_Actor1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ProductionURI_ | `uri` | `crm:E12_Production1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E12_Production1` | `crm:P14_carried_out_by` | `crm:E39_Actor1`|
| `crm:E22_Man-Made_Object1` | `crm:P108i_was_produced_by` | `crm:E12_Production1`|

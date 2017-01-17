# WAM_XMLExport_AAC_Dimensions.xml

## Add Column

## Add Node/Literal

## PyTransforms
#### _ObjectID_URI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "object/id/" + getValue("ObjectID")
```

#### _PhysicalThing_URI_
From column: _Root / ObjRecord / ObjectID_
``` python
return getValue("ObjectID_URI") + "/physical/"
```

#### _DimensionElement_
From column: _Root / ObjRecord / Dimensions / DimensionType / Element_
``` python
return getValue("Element")
```

#### _DimensionElementURI_
From column: _Root / ObjRecord / Dimensions / DimensionType / DimensionElement_
``` python
return getValue("PhysicalThing_URI") + getValue("Element").lower() + "/dimension/id/" + getValue("DimItemElemXrefID")
```

#### _DimensionTypeURI_
From column: _Root / ObjRecord / Dimensions / DimensionType / DimensionPart / DimensionType_
``` python
return getValue("DimensionElementURI") + "/type/" + getValue("DimensionType").lower()
```

#### _DimensionURI_
From column: _Root / ObjRecord / Dimensions / DimensionType / DimensionPart / DimRank_
``` python
return getValue("DimensionElementURI") + "/value/" + getValue("DimensionType").lower()
```

#### _DimensionCleaned_
From column: _Root / ObjRecord / Dimensions / DimensionType / DimensionPart / Dimension_
``` python
return str(int(float(getValue("Dimension"))*10)/10.0)
```


## Selections

## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _DimensionCleaned_ | `rdf:value` | `crm:E54_Dimension1`|
| _DimensionElement_ | `rdfs:label` | `crm:E55_Type1`|
| _DimensionElementURI_ | `uri` | `crm:E55_Type1`|
| _DimensionType_ | `skos:prefLabel` | `crm:E55_Type2`|
| _DimensionTypeURI_ | `uri` | `crm:E55_Type2`|
| _DimensionURI_ | `uri` | `crm:E54_Dimension1`|
| _Element_ | `rdfs:label` | `crm:E18_Physical_Thing1`|
| _ObjectID_URI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _PhysicalThing_URI_ | `uri` | `crm:E18_Physical_Thing1`|
| _UnitLabel_ | `crm:P91_has_unit` | `crm:E54_Dimension1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E18_Physical_Thing1` | `crm:P43_has_dimension` | `crm:E54_Dimension1`|
| `crm:E18_Physical_Thing1` | `crm:P2_has_type` | `crm:E55_Type1`|
| `crm:E22_Man-Made_Object1` | `crm:P46_is_composed_of` | `crm:E18_Physical_Thing1`|
| `crm:E54_Dimension1` | `crm:P2_has_type` | `crm:E55_Type2`|

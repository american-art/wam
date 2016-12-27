# WAM_XMLExport_AAC_Constituents_V3.xml

## Add Column

## Add Node/Literal
#### Literal Node: `http://vocab.getty.edu/aat/300387357`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _ObjectID_URI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "object/id/" + getValue("ObjectID")
```

#### _ProductionURI_
From column: _Root / ObjRecord / ObjectID_URI_
``` python
return getValue("ObjectID_URI") + "/production"
```

#### _ConstituentURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentID_
``` python
return getValue("ProductionURI") + "/" + getValue("ConstituentType").lower() + "/" + getValue("ConstituentID")
```

#### _WorkURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / ThesGeoType_
``` python
def cleanURI(prefix, value):
    uri_value = value.lower().replace(' ', '_')
    return UM.uri_from_fields(prefix + uri_value)
geoType = getValue("ThesGeoType")
if geoType:
    return getValue("ConstituentURI") + cleanURI("/", geoType)
else:
    return ""
```

#### _PlaceURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / WorkURI_
``` python
return getValue("WorkURI") + "/" + getValue("ConGeoTGNSourceTermID")
```


## Selections
#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / Gender_
<br>Operation: `Union`
``` python
return getValue("ConstituentType") != "Individual"
```

#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / ConGeoLatDirection_
<br>Operation: `Union`
``` python
return getValue("ThesGeoType") != "Work Location"
```


## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _ConstituentURI_ | `uri` | `crm:E39_Actor1`|
| _ObjectID_URI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _PlaceURI_ | `uri` | `crm:E53_Place1`|
| _ProductionURI_ | `uri` | `crm:E12_Production1`|
| _ThesGeographyTerm_ | `rdfs:label` | `crm:E53_Place1`|
| _WorkURI_ | `uri` | `crm:E9_Move1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E12_Production1` | `crm:P14_carried_out_by` | `crm:E39_Actor1`|
| `crm:E22_Man-Made_Object1` | `crm:P108i_was_produced_by` | `crm:E12_Production1`|
| `crm:E39_Actor1` | `crm:P25i_moved_by` | `crm:E9_Move1`|
| `crm:E9_Move1` | `crm:P21_had_general_purpose` | `xsd:http://vocab.getty.edu/aat/300387357`|
| `crm:E9_Move1` | `crm:P26_moved_to` | `crm:E53_Place1`|

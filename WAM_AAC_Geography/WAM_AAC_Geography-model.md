# WAM_XMLExport_AAC_Geography.xml

## Add Column

## Add Node/Literal
#### Literal Node: `http://vocab.getty.edu/aat/300387565`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300387567`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _ObjectURI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "object/"+getValue("ObjectID")
```

#### _NotInUse_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / GeoType_
``` python
return getValue("ObjectURI")+"/production"
```

#### _PlaceURI_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / GeographyID_
``` python
return getValue("ProductionURI")+"/place"
#return "object/"+getValue("ObjectID")
```

#### _LatitudeURI_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / LatitudeNumber_
``` python
return getValue("PlaceURI")+"/latitude"
```

#### _LatitudeValue_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / LatitudeNumber_
``` python
def format_latLong(str):
    deg = u"\u00b0"  # utf code for degree
    dim = str.split(' ')
    if len(dim) == 2:
        return dim[0].lstrip('0') + deg + dim[1] + "\'"
    else:
        return ""
lat = getValue("Latitude")
latDir = getValue("LatitudeDirection")
long = getValue("Longitude")
longDir = getValue("LongitudeDirection")
if longDir == "" or latDir == "" or long == "" or lat == "":
    return ""
else:
    return "\"" + format_latLong(lat)  + " " + latDir +  "\""
```

#### _LongitudeURI_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / LongitudeNumber_
``` python
return getValue("PlaceURI")+"/longitude"
```

#### _LongitudeValue_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / LongitudeNumber_
``` python
def format_latLong(str):
    deg = u"\u00b0"  # utf code for degree
    dim = str.split(' ')
    if len(dim) == 2:
        return dim[0].lstrip('0') + deg + dim[1] + "\'"
    else:
        return ""
lat = getValue("Latitude")
latDir = getValue("LatitudeDirection")
long = getValue("Longitude")
longDir = getValue("LongitudeDirection")
if longDir == "" or latDir == "" or long == "" or lat == "":
    return ""
else:
    return "\"" + format_latLong(long) + " " +longDir + "\""
```

#### _ProductionURI_
From column: _Root / ObjRecord / ObjectURI_
``` python
return getValue("ObjectURI")+"/production"
```


## Selections
#### _DEFAULT_TEST_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / LatitudeNumber_
<br>Operation: `Union`
``` python
return getValue("GeoType")!="Place of Origin"
```


## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _GeographyTerm_ | `rdfs:label` | `crm:E53_Place1`|
| _LatitudeURI_ | `uri` | `crm:E47_Spatial_Coordinates1`|
| _LatitudeValue_ | `rdf:value` | `crm:E47_Spatial_Coordinates1`|
| _LongitudeURI_ | `uri` | `crm:E47_Spatial_Coordinates2`|
| _LongitudeValue_ | `rdf:value` | `crm:E47_Spatial_Coordinates2`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _PlaceURI_ | `uri` | `crm:E53_Place1`|
| _ProductionURI_ | `uri` | `crm:E12_Production1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E12_Production1` | `crm:P7_took_place_at` | `crm:E53_Place1`|
| `crm:E22_Man-Made_Object1` | `crm:P108i_was_produced_by` | `crm:E12_Production1`|
| `crm:E47_Spatial_Coordinates1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300387565`|
| `crm:E47_Spatial_Coordinates2` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300387567`|
| `crm:E53_Place1` | `crm:P87_is_identified_by` | `crm:E47_Spatial_Coordinates1`|
| `crm:E53_Place1` | `crm:P87_is_identified_by` | `crm:E47_Spatial_Coordinates2`|

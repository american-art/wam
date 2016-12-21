# WAM_XMLExport_AAC_Geography.xml

## Add Column

## Add Node/Literal
#### Literal Node: `http://vocab.getty.edu/aat/300387567`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300387565`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _ObjectID_URI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "object/id/" + getValue("ObjectID")
```

#### _SchemaLatitude_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / Latitude_
``` python
return getValue("Latitude")
```

#### _ProductionURI_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / GeoType_
``` python
def cleanURI(prefix, value):
    uri_value = value.lower().replace(' ', '_')
    return UM.uri_from_fields(prefix + uri_value)
prefix = getValue("ObjectID_URI") + "/"
geoType = getValue("GeoType")
if geoType:
    return cleanURI(prefix, geoType)
else:
    return ""
```

#### _PlaceURI_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / GeographyID_
``` python
return getValue("ProductionURI") + "/geography/id/" + getValue("GeographyID")
```

#### _LatitudeURI_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / Latitude_
``` python
return getValue("PlaceURI") + "/latitude"
```

#### _LongitudeURI_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / Longitude_
``` python
return getValue("PlaceURI") + "/longitude"
```

#### _SpatialCoOrdinates_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / LatitudeDirection_
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
    return "\"" + format_latLong(lat)  + " " + latDir +  " " + format_latLong(long) + " " +longDir + "\""
```

#### _SpatialCoOrdinatesURI_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / SpatialCoOrdinates_
``` python
return getValue("PlaceURI") + "/lat_long"
```

#### _TGNTermPlace_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / TGNTermID_
``` python
tgnTermId = getValue("TGNTermID")
if tgnTermId:
    return "http://vocab.getty.edu/tgn/" + tgnTermId + "-place"
else:
    return ""
```


## Selections
#### _DEFAULT_TEST_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / LatitudeDirection_
<br>Operation: `Union`
``` python
return getValue("GeoType") != "Place of Origin"
```


## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _GeographyTerm_ | `rdfs:label` | `crm:E53_Place1`|
| _Latitude_ | `rdf:value` | `crm:E47_Spatial_Coordinates1`|
| _LatitudeURI_ | `uri` | `crm:E47_Spatial_Coordinates1`|
| _Longitude_ | `rdf:value` | `crm:E47_Spatial_Coordinates2`|
| _LongitudeURI_ | `uri` | `crm:E47_Spatial_Coordinates2`|
| _ObjectID_URI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _PlaceURI_ | `uri` | `crm:E53_Place1`|
| _ProductionURI_ | `uri` | `crm:E12_Production1`|
| _SpatialCoOrdinates_ | `rdf:value` | `crm:E47_Spatial_Coordinates3`|
| _SpatialCoOrdinatesURI_ | `uri` | `crm:E47_Spatial_Coordinates3`|
| _TGNTermID_ | `rdfs:label` | `crm:E42_Identifier1`|
| _TGNTermPlace_ | `uri` | `crm:E42_Identifier1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E12_Production1` | `crm:P7_took_place_at` | `crm:E53_Place1`|
| `crm:E22_Man-Made_Object1` | `crm:P108i_was_produced_by` | `crm:E12_Production1`|
| `crm:E47_Spatial_Coordinates1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300387565`|
| `crm:E47_Spatial_Coordinates2` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300387567`|
| `crm:E53_Place1` | `crm:P1_is_identified_by` | `crm:E42_Identifier1`|
| `crm:E53_Place1` | `crm:P87_is_identified_by` | `crm:E47_Spatial_Coordinates1`|
| `crm:E53_Place1` | `crm:P87_is_identified_by` | `crm:E47_Spatial_Coordinates2`|
| `crm:E53_Place1` | `crm:P87_is_identified_by` | `crm:E47_Spatial_Coordinates3`|

# WAM_AAC_Geography.xml

## Add Column
#### _ObjectURI_
From column: _Root / ObjRecord / ObjectID_
<br/>Value: ``

#### _GeoTypeURI_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / GeoType_
<br/>Value: ``

#### _GeographyID_URI_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / GeographyID_
<br/>Value: ``

#### _SpatialCoOrdinates_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / GeographyTerm_
<br/>Value: ``

#### _TGN_Place_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / TGNTermID_
<br/>Value: ``

#### _ObjectVal_
From column: _Root / ObjRecord / ObjectID_
<br/>Value: ``

#### _Type_Repositry_
From column: _Root / ObjRecord / ObjectVal_
<br/>Value: `<http://vocab.getty.edu/aat/300404621>`

#### _Type_Longitude_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / Longitude_
<br/>Value: `<http://vocab.getty.edu/aat/300387567>`

#### _Type_Latitude_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / Latitude_
<br/>Value: `<http://vocab.getty.edu/aat/300387565>`


## Add Node/Literal
#### Literal Node: `http://vocab.getty.edu/aat/300404621`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300387565`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300387567`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/tgn/7012149-place`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _ObjectURI_
From column: _Root / ObjRecord / ObjectURI_
``` python
return "id/object/" + getValue("ObjectID")
```

#### _GeoTypeURI_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / GeoTypeURI_
``` python
def cleanURI(prefix, value):
    uri_value = value.lower().replace(' ', '_')
    return UM.uri_from_fields(prefix + uri_value)

geoPrefix = "thesauri/geo_type/"
geoType = getValue("GeoType")
if geoType:
    return cleanURI(geoPrefix,geoType)
else:
    return ""
```

#### _GeographyID_URI_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / GeographyID_URI_
``` python
geoID = getValue("GeographyID")
if geoID:
    return "geography/"+geoID
else:
    return ""
```

#### _SpatialCoOrdinates_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / SpatialCoOrdinates_
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

#### _TGN_Place_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / TGN_Place_
``` python
tgnTermId = getValue("TGNTermID")
if tgnTermId:
    return "http://vocab.getty.edu/tgn/" + tgnTermId + "-place"
else:
    return ""
```

#### _ObjectVal_
From column: _Root / ObjRecord / ObjectVal_
``` python
return getValue("ObjectID")
```

#### _ObjectID_URI_
From column: _Root / ObjRecord / ObjectVal_
``` python
return getValue("ObjectURI")
```


## Selections
#### _DEFAULT_TEST_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / SpatialCoOrdinates_
<br>Operation: `Union`
``` python
return getValue("GeoType") != "Place Depicted"
```


## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _GeoType_ | `rdfs:label` | `crm:E55_Type1`|
| _GeoTypeURI_ | `uri` | `crm:E55_Type1`|
| _GeographyID_ | `rdfs:label` | `crm:E42_Identifier2`|
| _GeographyID_URI_ | `uri` | `crm:E53_Place1`|
| _GeographyTerm_ | `rdfs:label` | `crm:E48_Place_Name1`|
| _Latitude_ | `rdf:value` | `crm:E47_Spatial_Coordinates2`|
| _Longitude_ | `rdf:value` | `crm:E47_Spatial_Coordinates3`|
| _ObjectID_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectID_URI_ | `uri` | `crm:E42_Identifier1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ObjectVal_ | `rdf:value` | `crm:E42_Identifier1`|
| _SpatialCoOrdinates_ | `rdfs:label` | `crm:E47_Spatial_Coordinates1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E22_Man-Made_Object1` | `crm:P1_is_identified_by` | `crm:E42_Identifier1`|
| `crm:E22_Man-Made_Object1` | `crm:P62_depicts` | `crm:E53_Place1`|
| `crm:E42_Identifier1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404621`|
| `crm:E47_Spatial_Coordinates2` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300387565`|
| `crm:E47_Spatial_Coordinates3` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300387567`|
| `crm:E53_Place1` | `crm:P48_has_preferred_identifier` | `crm:E42_Identifier2`|
| `crm:E53_Place1` | `crm:P1_is_identified_by` | `crm:E47_Spatial_Coordinates1`|
| `crm:E53_Place1` | `crm:P87_is_identified_by` | `crm:E47_Spatial_Coordinates2`|
| `crm:E53_Place1` | `crm:P87_is_identified_by` | `crm:E47_Spatial_Coordinates3`|
| `crm:E53_Place1` | `crm:P1_is_identified_by` | `crm:E48_Place_Name1`|
| `crm:E53_Place1` | `crm:P2i_is_type_of` | `crm:E55_Type1`|
| `crm:E53_Place1` | `skos:exactMatch` | `xsd:http://vocab.getty.edu/tgn/7012149-place`|

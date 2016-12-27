# WAM_XMLExport_AAC_Constituents_V3.xml

## Add Column

## Add Node/Literal
#### Literal Node: `http://vocab.getty.edu/ulan`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300404670`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300055147`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300080102`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _ObjectID_URI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "object/id/" + getValue("ObjectID")
```

#### _Production_URI_
From column: _Root / ObjRecord / ObjectID_URI_
``` python
return getValue("ObjectID_URI") + "/production"
```

#### _ConstituentURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentID_
``` python
return getValue("Production_URI") + "/" + getValue("ConstituentType").lower() + "/" + getValue("ConstituentID")
```

#### _ULANID_URI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / CreatorULANID_
``` python
ulan_id = getValue("CreatorULANID")
if ulan_id:
    return "http://vocab.getty.edu/ulan/"+ ulan_id
else:
    return ""
```

#### _AppellationaName_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / DisplayName_
``` python
return getValue("DisplayName")
```

#### _AppellationURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / AppellationaName_
``` python
return getValue("ConstituentURI") + "/appellation"
```

#### _GenderURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / Gender_
``` python
return getValue("ConstituentURI") + "/gender"
```

#### _GenderTypeURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / GenderURI_
``` python
return getValue("ConstituentURI") + "/gender_type"
```

#### _BiographyURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / Biography_
``` python
return getValue("ConstituentURI") + "/biography"
```

#### _SpatialCoordinates_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / ConGeoLongitudeNumber_
``` python
def format_latLong(str):
    deg = u"\u00b0"  # utf code for degree
    dim = str.split(' ')
    if len(dim) == 2:
        return dim[0].lstrip('0') + deg + dim[1] + "\'"
    else:
        return ""
lat = getValue("ConGeoLatitude")
latDir = getValue("ConGeoLatDirection")
long = getValue("ConGeoLongitude")
longDir = getValue("ConGeoLongDirection")
if longDir == "" or latDir == "" or long == "" or lat == "":
    return ""
else:
    return "\"" + format_latLong(lat)  + " " + latDir +  " " + format_latLong(long) + " " +longDir + "\""
```

#### _ConGeoTGNSourceTermID_URL_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / ConGeoTGNSourceTermID_
``` python
conGeoTGNSourceTermID = getValue("ConGeoTGNSourceTermID")
if conGeoTGNSourceTermID:
    return "http://vocab.getty.edu/tgn/" + conGeoTGNSourceTermID
else:
    return ""
```

#### _BirthURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / ThesGeographyTerm_
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
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / ThesGeographyTerm_
``` python
return getValue("BirthURI") + "/" + getValue("ConGeoTGNSourceTermID")
```

#### _ConGeoTGNSourceTermID_URI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / ConGeoTGNSourceTermID_URL_
``` python
conGeoTGNSourceTermID = getValue("ConGeoTGNSourceTermID")
if conGeoTGNSourceTermID:
    return getValue("PlaceURI") + "/tgn_term"
else:
    return ""
```

#### _SpatialCoordinatesURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / SpatialCoordinates_
``` python
lat_long = getValue("SpatialCoordinates")
if lat_long:
    return getValue("PlaceURI") + "/lat_long"
else:
    return ""
```


## Selections
#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / Gender_
<br>Operation: `Union`
``` python
return getValue("ConstituentType") != "Individual"
```

#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / SpatialCoordinates_
<br>Operation: `Union`
``` python
return getValue("ThesGeoType") != "Birth Location"
```


## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _AppellationURI_ | `uri` | `crm:E82_Actor_Appellation1`|
| _AppellationaName_ | `rdf:value` | `crm:E82_Actor_Appellation1`|
| _Biography_ | `rdf:value` | `crm:E33_Linguistic_Object1`|
| _BiographyURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _BirthURI_ | `uri` | `crm:E63_Beginning_of_Existence1`|
| _ConGeoTGNSourceTermID_URI_ | `uri` | `crm:E42_Identifier1`|
| _ConGeoTGNSourceTermID_URL_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ConstituentURI_ | `uri` | `crm:E39_Actor1`|
| _CreatorULANID_ | `rdfs:label` | `skos:Concept1`|
| _DisplayName_ | `rdfs:label` | `crm:E39_Actor1`|
| _Gender_ | `rdfs:label` | `crm:E55_Type1`|
| _GenderTypeURI_ | `uri` | `crm:E55_Type2`|
| _GenderURI_ | `uri` | `crm:E55_Type1`|
| _ObjectID_URI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _PlaceURI_ | `uri` | `crm:E53_Place1`|
| _Production_URI_ | `uri` | `crm:E12_Production1`|
| _SpatialCoordinates_ | `rdfs:label` | `crm:E47_Spatial_Coordinates1`|
| _SpatialCoordinatesURI_ | `uri` | `crm:E47_Spatial_Coordinates1`|
| _ThesGeographyTerm_ | `rdfs:label` | `crm:E53_Place1`|
| _ULANID_URI_ | `uri` | `skos:Concept1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E12_Production1` | `crm:P14_carried_out_by` | `crm:E39_Actor1`|
| `crm:E22_Man-Made_Object1` | `crm:P108i_was_produced_by` | `crm:E12_Production1`|
| `crm:E33_Linguistic_Object1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300080102`|
| `crm:E33_Linguistic_Object1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `crm:E39_Actor1` | `crm:P129i_is_subject_of` | `crm:E33_Linguistic_Object1`|
| `crm:E39_Actor1` | `crm:P131_is_identified_by` | `crm:E82_Actor_Appellation1`|
| `crm:E39_Actor1` | `crm:P2_has_type` | `crm:E55_Type1`|
| `crm:E39_Actor1` | `crm:P92i_was_brought_into_existence_by` | `crm:E63_Beginning_of_Existence1`|
| `crm:E39_Actor1` | `skos:exactMatch` | `skos:Concept1`|
| `crm:E53_Place1` | `crm:P1_is_identified_by` | `crm:E47_Spatial_Coordinates1`|
| `crm:E53_Place1` | `crm:P48_has_preferred_identifier` | `crm:E42_Identifier1`|
| `crm:E55_Type1` | `crm:P2_has_type` | `crm:E55_Type2`|
| `crm:E55_Type2` | `skos:broadMatch` | `xsd:http://vocab.getty.edu/aat/300055147`|
| `crm:E63_Beginning_of_Existence1` | `crm:P7_took_place_at` | `crm:E53_Place1`|
| `crm:E82_Actor_Appellation1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `skos:Concept1` | `skos:inScheme` | `xsd:http://vocab.getty.edu/ulan`|

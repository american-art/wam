# WAM_XMLExport_AAC_Constituents_V3.xml

## Add Column

## Add Node/Literal
#### Literal Node: `http://vocab.getty.edu/aat/300404621`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300404670`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300080102`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300055147`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/ulan`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300387357`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _IdURI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "id/" + getValue("ObjectID")
```

#### _ObjectLabel_
From column: _Root / ObjRecord / ObjectID_
``` python
return getValue("ObjectID")
```

#### _ObjectID_URI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "id/object/" + getValue("ObjectID")
```

#### _ConstituentURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentID_
``` python
constituentType = getValue("ConstituentType")
if constituentType == "Institution":
    return "person-institution/"+getValue("ConstituentID")
else:
    return ""
```

#### _AppellationValue_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / DisplayName_
``` python
return getValue("DisplayName")
```

#### _AppellationURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / AppellationValue_
``` python
return getValue("ConstituentURI") + "/appellation/"
```

#### _GenderURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / Gender_
``` python
gender = getValue("Gender")
if gender:
    return "gender/" + gender
else:
    return ""
```

#### _BiographyURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / Biography_
``` python
bio = getValue("Biography")
if bio:
    return getValue("ConstituentURI") + "/biography/"
else:
    return ""
```

#### _SpatialCoOrdinates_
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

#### _ConGeoTGNSourceTermID_URI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / ConGeoTGNSourceTermID_
``` python
conGeoTGNSourceTermID = getValue("ConGeoTGNSourceTermID")
if conGeoTGNSourceTermID:
    return "http://vocab.getty.edu/tgn/" + conGeoTGNSourceTermID
else:
    return ""
```

#### _PlaceURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / ConGeoTGNSourceTermID_
``` python
return getValue("ConGeoTGNSourceTermID")
```

#### _workPlace_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / ThesGeographyTerm_
``` python
return getValue("ThesGeographyTerm")
```

#### _workPlaceURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / workPlace_
``` python
conGeoTGNSrcTermID = getValue("ConGeoTGNSourceTermID")
if conGeoTGNSrcTermID:
    return getValue("ConstituentURI")+"/work/"
else:
    return ""
```

#### _productionURI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "id/object/" + getValue("ObjectID") +"/production/"
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


## Selections
#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / Gender_
<br>Operation: `Union`
``` python
return getValue("ConstituentType") != "Institution"
```

#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / Gender_
<br>Operation: `Union`
``` python
return getValue("ConstituentType") != "Institution"
```

#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / values_
<br>Operation: `Union`
``` python
return getValue("ThesGeoType") != "Work Location"
```


## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _AppellationURI_ | `uri` | `crm:E82_Actor_Appellation1`|
| _AppellationValue_ | `rdf:value` | `crm:E82_Actor_Appellation1`|
| _Biography_ | `rdf:value` | `crm:E33_Linguistic_Object1`|
| _BiographyURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _ConGeoTGNSourceTermID_ | `rdfs:label` | `crm:E42_Identifier2`|
| _ConGeoTGNSourceTermID_URI_ | `uri` | `crm:E42_Identifier2`|
| _ConstituentURI_ | `uri` | `crm:E39_Actor1`|
| _CreatorULANID_ | `rdfs:label` | `skos:Concept1`|
| _DisplayName_ | `rdfs:label` | `crm:E39_Actor1`|
| _IdURI_ | `uri` | `crm:E42_Identifier1`|
| _ObjectID_ | `rdf:value` | `crm:E42_Identifier1`|
| _ObjectID_URI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ObjectLabel_ | `rdfs:label` | `crm:E42_Identifier1`|
| _PlaceURI_ | `uri` | `crm:E53_Place1`|
| _SpatialCoOrdinates_ | `rdfs:label` | `crm:E47_Spatial_Coordinates1`|
| _ThesGeographyTerm_ | `rdfs:label` | `crm:E48_Place_Name1`|
| _ULANID_URI_ | `uri` | `skos:Concept1`|
| _productionURI_ | `uri` | `crm:E12_Production1`|
| _workPlace_ | `rdfs:label` | `crm:E53_Place1`|
| _workPlaceURI_ | `uri` | `crm:E9_Move1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E12_Production1` | `crm:P14_carried_out_by` | `crm:E39_Actor1`|
| `crm:E22_Man-Made_Object1` | `crm:P108i_was_produced_by` | `crm:E12_Production1`|
| `crm:E22_Man-Made_Object1` | `crm:P1_is_identified_by` | `crm:E42_Identifier1`|
| `crm:E33_Linguistic_Object1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `crm:E33_Linguistic_Object1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300080102`|
| `crm:E39_Actor1` | `crm:P129i_is_subject_of` | `crm:E33_Linguistic_Object1`|
| `crm:E39_Actor1` | `crm:P131_is_identified_by` | `crm:E82_Actor_Appellation1`|
| `crm:E39_Actor1` | `crm:P25i_moved_by` | `crm:E9_Move1`|
| `crm:E39_Actor1` | `skos:exactMatch` | `skos:Concept1`|
| `crm:E42_Identifier1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404621`|
| `crm:E53_Place1` | `crm:P48_has_preferred_identifier` | `crm:E42_Identifier2`|
| `crm:E53_Place1` | `crm:P1_is_identified_by` | `crm:E47_Spatial_Coordinates1`|
| `crm:E53_Place1` | `crm:P1_is_identified_by` | `crm:E48_Place_Name1`|
| `crm:E82_Actor_Appellation1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `crm:E9_Move1` | `crm:P26_moved_to` | `crm:E53_Place1`|
| `crm:E9_Move1` | `crm:P21_had_general_purpose` | `xsd:http://vocab.getty.edu/aat/300387357`|
| `skos:Concept1` | `skos:inScheme` | `xsd:http://vocab.getty.edu/ulan`|

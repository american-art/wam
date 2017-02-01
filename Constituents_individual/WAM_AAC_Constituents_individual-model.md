# WAM_XMLExport_AAC_Constituents_V3.xml

## Add Column

## Add Node/Literal
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

#### Literal Node: `http://vocab.getty.edu/ulan`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _ConstituentURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentID_
``` python
return "constituent/"+getValue("ConstituentID")
```

#### _NameLabel_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / DisplayName_
``` python
return getValue("DisplayName")
```

#### _NameURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / CreatorULANID_
``` python
return getValue("ConstituentURI")+"/name"
```

#### _GenderURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / Gender_
``` python
return getValue("ConstituentURI")+"/gender"
```

#### _GenderTypeURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / Gender_
``` python
return getValue("GenderURI")+"/gender_type"
```

#### _BiographyURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / Role_
``` python
if getValue("Biography"):
    return getValue("Biography")
else:
    return ""
```

#### _UlanURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / CreatorULANID_
``` python
if getValue("Creator ULAN"):
    return "http://vocab.getty.edu/ulan/"+getValue("Creator ULAN")
else:
    return ""
```


## Selections
#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentType_
<br>Operation: `Union`
``` python
return getValue("ConstituentType")!="Individual"
```


## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _Biography_ | `rdf:value` | `crm:E33_Linguistic_Object1`|
| _BiographyURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _ConstituentURI_ | `uri` | `crm:E39_Actor1`|
| _DisplayName_ | `rdf:value` | `crm:E82_Actor_Appellation1`|
| _Gender_ | `rdfs:label` | `crm:E55_Type1`|
| _GenderTypeURI_ | `uri` | `crm:E55_Type2`|
| _GenderURI_ | `uri` | `crm:E55_Type1`|
| _NameLabel_ | `rdfs:label` | `crm:E39_Actor1`|
| _NameURI_ | `uri` | `crm:E82_Actor_Appellation1`|
| _UlanURI_ | `uri` | `skos:Concept1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E33_Linguistic_Object1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `crm:E33_Linguistic_Object1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300080102`|
| `crm:E39_Actor1` | `crm:P129i_is_subject_of` | `crm:E33_Linguistic_Object1`|
| `crm:E39_Actor1` | `crm:P2_has_type` | `crm:E55_Type1`|
| `crm:E39_Actor1` | `crm:P131_is_identified_by` | `crm:E82_Actor_Appellation1`|
| `crm:E39_Actor1` | `skos:exactMatch` | `skos:Concept1`|
| `crm:E55_Type1` | `crm:P2_has_type` | `crm:E55_Type2`|
| `crm:E55_Type2` | `skos:broadMatch` | `xsd:http://vocab.getty.edu/aat/300055147`|
| `crm:E82_Actor_Appellation1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `skos:Concept1` | `skos:inScheme` | `xsd:http://vocab.getty.edu/ulan`|

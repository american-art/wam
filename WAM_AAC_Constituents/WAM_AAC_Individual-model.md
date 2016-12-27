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

#### _ULANID_URI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / CreatorULANID_
``` python
ulan_id = getValue("CreatorULANID")
if ulan_id:
    return "http://vocab.getty.edu/ulan/"+ ulan_id
else:
    return ""
```

#### _AppellationName_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / DisplayName_
``` python
return getValue("DisplayName")
```

#### _AppellationURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / AppellationName_
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


## Selections
#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / Gender_
<br>Operation: `Union`
``` python
return getValue("ConstituentType") != "Individual"
```


## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _AppellationURI_ | `uri` | `crm:E82_Actor_Appellation1`|
| _AppellationaName_ | `rdf:value` | `crm:E82_Actor_Appellation1`|
| _Biography_ | `rdf:value` | `crm:E33_Linguistic_Object1`|
| _BiographyURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _ConstituentURI_ | `uri` | `crm:E39_Actor1`|
| _CreatorULANID_ | `rdfs:label` | `skos:Concept1`|
| _DisplayName_ | `rdfs:label` | `crm:E39_Actor1`|
| _Gender_ | `rdfs:label` | `crm:E55_Type1`|
| _GenderTypeURI_ | `uri` | `crm:E55_Type2`|
| _GenderURI_ | `uri` | `crm:E55_Type1`|
| _ObjectID_URI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ProductionURI_ | `uri` | `crm:E12_Production1`|
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
| `crm:E39_Actor1` | `skos:exactMatch` | `skos:Concept1`|
| `crm:E55_Type1` | `crm:P2_has_type` | `crm:E55_Type2`|
| `crm:E55_Type2` | `skos:broadMatch` | `xsd:http://vocab.getty.edu/aat/300055147`|
| `crm:E82_Actor_Appellation1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `skos:Concept1` | `skos:inScheme` | `xsd:http://vocab.getty.edu/ulan`|

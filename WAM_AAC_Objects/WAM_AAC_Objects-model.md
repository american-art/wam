# WAM_XMLExport_AAC_Objects.xml

## Add Column

## Add Node/Literal
#### Literal Node: `ttp://vocab.getty.edu/aat/300179869`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `ttp://vocab.getty.edu/aat/300026687`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300264237`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300080091`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300404670`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300026687`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300179869`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _ObjectURI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "object/"+getValue("ObjectID")
```

#### _ClassificationURI_
From column: _Root / ObjRecord / Classification_
``` python
return getValue("ObjectURI")+"/classification_type"
```

#### _ClassificationEventURI_
From column: _Root / ObjRecord / Classification_
``` python
return getValue("ObjectURI")+"/classification"
```

#### _CreditLineURI_
From column: _Root / ObjRecord / CreditLine_
``` python
return getValue("ObjectURI")+"/credit_line"
```

#### _ProductionURI_
From column: _Root / ObjRecord / DataDateStamp_
``` python
return getValue("ObjectURI")+"/production"
```

#### _ProductionTimespanURI_
From column: _Root / ObjRecord / ProductionURI_
``` python
return getValue("ProductionURI")+"/timespan"
```

#### _MediumURI_
From column: _Root / ObjRecord / PhysicalDescription / Medium_
``` python
return getValue("ObjectURI")+"/medium_text"
```

#### _MediumTermURI_
From column: _Root / ObjRecord / PhysicalDescription / PhysicalDescriptionTerms / SourceTermID_
``` python
if getValue("SourceTermID"):
    return UM.uri_from_fields("material/",getValue("Term"))
else:
    return ""
```

#### _MediumLodTerm_
From column: _Root / ObjRecord / PhysicalDescription / PhysicalDescriptionTerms / Term_
``` python
return "http://vocab.getty.edu/aat/"+getValue("SourceTermID")
```

#### _DescriptionURI_
From column: _Root / ObjRecord / Provenance_
``` python
return getValue("ObjectURI")+"/description"
```

#### _UrlURI_
From column: _Root / ObjRecord / PublicDescription_
``` python
return getValue("ResourceURL")
```

#### _CurrentOwnerURI_
From column: _Root / ObjRecord / Inscription_
``` python
return getValue("ObjectURI")+"/current_owner"
```


## Selections

## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _Classification_ | `rdfs:label` | `crm:E55_Type1`|
| _ClassificationEventURI_ | `uri` | `crm:E17_Type_Assignment1`|
| _ClassificationURI_ | `uri` | `crm:E55_Type1`|
| _CreditLine_ | `rdf:value` | `crm:E33_Linguistic_Object1`|
| _CreditLineURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _CurrentOwnerURI_ | `uri` | `crm:E40_Legal_Body1`|
| _DateBegin_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span1`|
| _DateEnd_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span1`|
| _Dated_ | `rdfs:label` | `crm:E52_Time-Span1`|
| _DescriptionURI_ | `uri` | `crm:E33_Linguistic_Object3`|
| _Medium_ | `rdf:value` | `crm:E33_Linguistic_Object2`|
| _MediumLodTerm_ | `uri` | `owl:Thing1`|
| _MediumTermURI_ | `uri` | `crm:E57_Material1`|
| _MediumURI_ | `uri` | `crm:E33_Linguistic_Object2`|
| _ObjUnderJurisOf_ | `rdfs:label` | `crm:E40_Legal_Body1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ProductionTimespanURI_ | `uri` | `crm:E52_Time-Span1`|
| _ProductionURI_ | `uri` | `crm:E12_Production1`|
| _PublicDescription_ | `rdf:value` | `crm:E33_Linguistic_Object3`|
| _ResourceURL_ | `rdfs:label` | `foaf:Document1`|
| _Term_ | `skos:prefLabel` | `crm:E57_Material1`|
| _UrlURI_ | `uri` | `foaf:Document1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E12_Production1` | `crm:P4_has_time-span` | `crm:E52_Time-Span1`|
| `crm:E17_Type_Assignment1` | `crm:P42_assigned` | `crm:E55_Type1`|
| `crm:E17_Type_Assignment1` | `crm:P21_had_general_purpose` | `xsd:http://vocab.getty.edu/aat/300179869`|
| `crm:E22_Man-Made_Object1` | `crm:P108i_was_produced_by` | `crm:E12_Production1`|
| `crm:E22_Man-Made_Object1` | `crm:P41i_was_classified_by` | `crm:E17_Type_Assignment1`|
| `crm:E22_Man-Made_Object1` | `crm:P67i_is_referred_to_by` | `crm:E33_Linguistic_Object1`|
| `crm:E22_Man-Made_Object1` | `crm:P129i_is_subject_of` | `crm:E33_Linguistic_Object2`|
| `crm:E22_Man-Made_Object1` | `crm:P129i_is_subject_of` | `crm:E33_Linguistic_Object3`|
| `crm:E22_Man-Made_Object1` | `crm:P52_has_current_owner` | `crm:E40_Legal_Body1`|
| `crm:E22_Man-Made_Object1` | `crm:P45_consists_of` | `crm:E57_Material1`|
| `crm:E22_Man-Made_Object1` | `foaf:homepage` | `foaf:Document1`|
| `crm:E22_Man-Made_Object1` | `crm:P2_has_type` | `crm:E55_Type1`|
| `crm:E22_Man-Made_Object1` | `crm:P67i_is_referred_to_by` | `crm:E33_Linguistic_Object2`|
| `crm:E33_Linguistic_Object1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300026687`|
| `crm:E33_Linguistic_Object2` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300264237`|
| `crm:E33_Linguistic_Object3` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300080091`|
| `crm:E33_Linguistic_Object3` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `crm:E57_Material1` | `skos:broadMatch` | `owl:Thing1`|

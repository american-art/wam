# WAM_XMLExport_AAC_Objects.xml

## Add Column

## Add Node/Literal
#### Literal Node: `http://vocab.getty.edu/aat/300404621`
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

#### Literal Node: `http://vocab.getty.edu/aat/300264237`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _ObjectLabel_
From column: _Root / ObjRecord / ObjectID_
``` python
return getValue("ObjectID")
```

#### _DuplicatePublicDescription_
From column: _Root / ObjRecord / PublicDescription_
``` python
return getValue("PublicDescription")
```

#### _ResourceURI_
From column: _Root / ObjRecord / ResourceURL_
``` python
return getValue("ResourceURL")

```

#### _ObjectID_URI_
From column: _Root / ObjRecord / ObjUnderJurisOf_
``` python
return "object/id/" + getValue("ObjectID")
```

#### _IdURI_
From column: _Root / ObjRecord / ObjectID_
``` python
return "id/" + getValue("ObjectID")
```

#### _MediumURI_
From column: _Root / ObjRecord / PhysicalDescription / Medium_
``` python
return getValue("ObjectID_URI") + "/medium" 
```

#### _Classification_
From column: _Root / ObjRecord / Classification_
``` python
return getValue("Classification")
```

#### _ClassificationEventURI_
From column: _Root / ObjRecord / Classification_
``` python
return getValue("ObjectID_URI") + "/classification/event" 
```

#### _CreditLineURI_
From column: _Root / ObjRecord / CreditLine_
``` python
return getValue("ObjectID_URI") + "/credit_line"
```

#### _CurrentLocationURI_
From column: _Root / ObjRecord / CurrentLocation_
``` python
return getValue("ObjectID_URI") + "/current_location"
```

#### _PublicDescriptionURI_
From column: _Root / ObjRecord / PublicDescription_
``` python
return getValue("ObjectID_URI") + "/public_description"
```

#### _ProductionURI_
From column: _Root / ObjRecord / Dated_
``` python
return getValue("ObjectID_URI") + "/production"
```

#### _TermURI_
From column: _Root / ObjRecord / PhysicalDescription / PhysicalDescriptionTerms / SourceTermID_
``` python
sourceId = getValue("SourceTermID")
if sourceId:
    return "http://vocab.getty.edu/aat/" + sourceId
else:
    return ""
```

#### _ClassificationURI_
From column: _Root / ObjRecord / Classification_
``` python
return getValue("ObjectID_URI") + "/classification/type" 
```

#### _TimeSpanURI_
From column: _Root / ObjRecord / Dated_
``` python
return getValue("ProductionURI") + "/time"
```


## Selections

## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _Classification_ | `rdfs:label` | `crm:E55_Type1`|
| _ClassificationEventURI_ | `uri` | `crm:E17_Type_Assignment1`|
| _ClassificationURI_ | `uri` | `crm:E55_Type1`|
| _CreditLine_ | `rdf:value` | `crm:E33_Linguistic_Object2`|
| _CreditLineURI_ | `uri` | `crm:E33_Linguistic_Object2`|
| _CurrentLocation_ | `rdfs:label` | `crm:E53_Place1`|
| _CurrentLocationURI_ | `uri` | `crm:E53_Place1`|
| _DateBegin_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span1`|
| _DateEnd_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span1`|
| _Dated_ | `rdfs:label` | `crm:E52_Time-Span1`|
| _DuplicatePublicDescription_ | `dc:description` | `crm:E22_Man-Made_Object1`|
| _IdURI_ | `uri` | `crm:E42_Identifier1`|
| _Medium_ | `rdf:value` | `crm:E33_Linguistic_Object3`|
| _MediumURI_ | `uri` | `crm:E33_Linguistic_Object3`|
| _ObjectID_ | `rdf:value` | `crm:E42_Identifier1`|
| _ObjectID_URI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ObjectLabel_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ProductionURI_ | `uri` | `crm:E12_Production1`|
| _PublicDescription_ | `rdf:value` | `crm:E33_Linguistic_Object1`|
| _PublicDescriptionURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _ResourceURI_ | `uri` | `foaf:Document1`|
| _ResourceURL_ | `rdfs:label` | `foaf:Document1`|
| _Term_ | `rdfs:label` | `owl:Thing1`|
| _TermURI_ | `uri` | `owl:Thing1`|
| _TimeSpanURI_ | `uri` | `crm:E52_Time-Span1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E12_Production1` | `crm:P4_has_time-span` | `crm:E52_Time-Span1`|
| `crm:E17_Type_Assignment1` | `crm:P21_had_general_purpose` | `xsd:http://vocab.getty.edu/aat/300179869`|
| `crm:E17_Type_Assignment1` | `crm:P42_assigned` | `crm:E55_Type1`|
| `crm:E22_Man-Made_Object1` | `crm:P108i_was_produced_by` | `crm:E12_Production1`|
| `crm:E22_Man-Made_Object1` | `crm:P129i_is_subject_of` | `crm:E33_Linguistic_Object1`|
| `crm:E22_Man-Made_Object1` | `crm:P1_is_identified_by` | `crm:E42_Identifier1`|
| `crm:E22_Man-Made_Object1` | `crm:P41i_was_classified_by` | `crm:E17_Type_Assignment1`|
| `crm:E22_Man-Made_Object1` | `crm:P55_has_current_location` | `crm:E53_Place1`|
| `crm:E22_Man-Made_Object1` | `crm:P62_depicts` | `owl:Thing1`|
| `crm:E22_Man-Made_Object1` | `crm:P67i_is_referred_to_by` | `crm:E33_Linguistic_Object2`|
| `crm:E22_Man-Made_Object1` | `crm:P67i_is_referred_to_by` | `crm:E33_Linguistic_Object3`|
| `crm:E22_Man-Made_Object1` | `foaf:homepage` | `foaf:Document1`|
| `crm:E22_Man-Made_Object1` | `crm:P2_has_type` | `crm:E55_Type1`|
| `crm:E33_Linguistic_Object1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300080091`|
| `crm:E33_Linguistic_Object1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `crm:E33_Linguistic_Object2` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300026687`|
| `crm:E33_Linguistic_Object3` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300264237`|
| `crm:E42_Identifier1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404621`|

# NMWA_Data.csv

## Add Column
#### _ObjectURI_
From column: _ObjectID_
<br/>Value: ``

#### _ObjectNumberURI_
From column: _ObjectURI_
<br/>Value: ``

#### _ObjectNumberType_
From column: _Object Number_
<br/>Value: ``

#### _CreditURI_
From column: _Column_1_
<br/>Value: ``

#### _CreditType_
From column: _Credit_
<br/>Value: ``

#### _DepartmentURI_
From column: _CreditType_
<br/>Value: ``

#### _ClassificationTypeURI_
From column: _Department_
<br/>Value: ``

#### _CultureURI_
From column: _Classification_
<br/>Value: ``

#### _ProductionURI_
From column: _Column_3_
<br/>Value: ``

#### _ActorURI_
From column: _ProductionURI_
<br/>Value: ``

#### _PrimaryTitle_
From column: _Title_
<br/>Value: ``

#### _PrimaryTitleURI_
From column: _Title_
<br/>Value: ``

#### _PrimaryTitleType_
From column: _PrimaryTitle_
<br/>Value: ``

#### _TimespanURI_
From column: _Attribution_
<br/>Value: ``

#### _DateValid_
From column: _Dated_
<br/>Value: ``

#### _BeginDateValid_
From column: _DateValid_
<br/>Value: ``

#### _MaterialURI_
From column: _PrimaryTitleType_
<br/>Value: ``

#### _DimensionURI_
From column: _Medium_
<br/>Value: ``

#### _DescriptionURI_
From column: _Dimensions_
<br/>Value: ``

#### _ObjectURL_
From column: _Object Details Web Page/ Link to Object on Website_
<br/>Value: ``


## Add Node/Literal
#### Literal Node: `aat:300404621`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `aat:300026687`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `aat:300403012`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `aat:300266036`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `false`

#### Literal Node: `aat:300080091`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300404621`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300026687`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300080091`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300403012`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300266036`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300015646`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300179869`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/30080091`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300404670`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`

#### Literal Node: `http://vocab.getty.edu/aat/300404672`
Literal Type: ``
<br/>Language: ``
<br/>isUri: `true`


## PyTransforms
#### _ObjectURI_
From column: _ObjectURI_
``` python
return "object/"+getValue("ObjectID")
```

#### _ObjectNumberURI_
From column: _ObjectNumberURI_
``` python
return getValue("ObjectURI")+"/object_number"
```

#### _ObjectNumberType_
From column: _ObjectNumberType_
``` python
return "aat:300404621"
```

#### _CreditURI_
From column: _CreditURI_
``` python
return getValue("ObjectURI")+"/credit"
```

#### _CreditType_
From column: _CreditType_
``` python
return "aat:300026687"
```

#### _ClassificationTypeURI_
From column: _ClassificationTypeURI_
``` python
return getValue("ObjectURI")+"/classification"
```

#### _CultureURI_
From column: _CultureURI_
``` python
if getValue("Culture"):
    return UM.uri_from_fields("thesauri/culture/",getValue("Culture"))
else:
    return ""
```

#### _PrimaryTitle_
From column: _PrimaryTitle_
``` python
return getValue("Title")
```

#### _PrimaryTitleURI_
From column: _PrimaryTitleURI_
``` python
return UM.uri_from_fields("thesauri/title/",getValue("Title"))
```

#### _PrimaryTitleType_
From column: _PrimaryTitleType_
``` python
return "aat:300404012"
```

#### _ProductionURI_
From column: _ProductionURI_
``` python
return getValue("ObjectURI")+"/production"
```

#### _ActorURI_
From column: _ActorURI_
``` python
return "constituent/"+SM.fingerprint_string(getValue("Display Name"))
```

#### _TimespanURI_
From column: _TimespanURI_
``` python
return getValue("ObjectURI")+"/timespan"
```

#### _DateValid_
From column: _DateValid_
``` python
if getValue("Dated")!="NA" and getValue("Dated")!="N/A" and getValue("Dated")!="n.d.":
    return getValue("Dated")
else:
    return ""
```

#### _BeginDateValid_
From column: _BeginDateValid_
``` python
if getValue("Begin Date")!='0': 
    return getValue("Begin Date")
else:
    return ""
```

#### _MaterialURI_
From column: _MaterialURI_
``` python
return UM.uri_from_fields("material/",getValue("Medium"))
```

#### _DimensionURI_
From column: _DimensionURI_
``` python
return getValue("ObjectURI")+"/dimension"
```

#### _DescriptionURI_
From column: _DescriptionURI_
``` python
return getValue("ObjectURI")+"/description"
```

#### _ObjectURL1_
From column: _Object Details Web Page/ Link to Object on Website_
``` python
if getValue("Object Details Web Page/ Link to Object on Website") == "None":
    return ""
else:
     return getValue("Object Details Web Page/ Link to Object on Website")
```

#### _ObjectURLLabel_
From column: _ObjectURL1_
``` python
return getValue("ObjectURL1")
```

#### _ObjectNumberValue_
From column: _Object Number_
``` python
return getValue("Object Number")
```

#### _PrimaryTitleLabel_
From column: _PrimaryTitleURI_
``` python
return getValue("PrimaryTitle")
```

#### _ImageURI_
From column: _ObjectURL_
``` python
if getValue("Image Full Size URL"):
    return getValue("ObjectURL")
else:
    return ""
```

#### _ClassificationURI_
From column: _Department_
``` python
if getValue("Classification"):
    return UM.uri_from_fields("thesauri/classification/",getValue("Classification"))
else:
    return ""
```

#### _CultureTypeURI_
From column: _CultureURI_
``` python
if getValue("Culture"):
    return getValue("ObjectURI")+"/culture_type"
else:
    return ""
```

#### _NameLabel_
From column: _ActorURI_
``` python
return getValue("Display Name")
```


## Selections

## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _ActorURI_ | `uri` | `crm:E39_Actor1`|
| _BeginDateValid_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span1`|
| _Classification_ | `rdfs:label` | `crm:E55_Type3`|
| _ClassificationTypeURI_ | `uri` | `crm:E55_Type3`|
| _ClassificationURI_ | `uri` | `crm:E17_Type_Assignment2`|
| _Credit_ | `rdf:value` | `crm:E33_Linguistic_Object1`|
| _CreditURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _Culture_ | `rdfs:label` | `crm:E55_Type4`|
| _CultureTypeURI_ | `uri` | `crm:E55_Type4`|
| _CultureURI_ | `uri` | `crm:E17_Type_Assignment1`|
| _DateValid_ | `rdfs:label` | `crm:E52_Time-Span1`|
| _Description_ | `rdf:value` | `crm:E33_Linguistic_Object3`|
| _DescriptionURI_ | `uri` | `crm:E33_Linguistic_Object3`|
| _DimensionURI_ | `uri` | `crm:E33_Linguistic_Object2`|
| _Dimensions_ | `rdf:value` | `crm:E33_Linguistic_Object2`|
| _ImageURI_ | `uri` | `crm:E38_Image1`|
| _MaterialURI_ | `uri` | `crm:E57_Material1`|
| _Medium_ | `skos:prefLabel` | `crm:E57_Material1`|
| _Object Number_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectNumberURI_ | `uri` | `crm:E42_Identifier1`|
| _ObjectNumberValue_ | `rdf:value` | `crm:E42_Identifier1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ObjectURL1_ | `uri` | `foaf:Document1`|
| _ObjectURLLabel_ | `rdfs:label` | `foaf:Document1`|
| _PrimaryTitle_ | `rdf:value` | `crm:E35_Title1`|
| _PrimaryTitleLabel_ | `rdfs:label` | `crm:E22_Man-Made_Object1`|
| _PrimaryTitleURI_ | `uri` | `crm:E35_Title1`|
| _ProductionURI_ | `uri` | `crm:E12_Production1`|
| _TimespanURI_ | `uri` | `crm:E52_Time-Span1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E12_Production1` | `crm:P14_carried_out_by` | `crm:E39_Actor1`|
| `crm:E12_Production1` | `crm:P4_has_time-span` | `crm:E52_Time-Span1`|
| `crm:E17_Type_Assignment1` | `crm:P42_assigned` | `crm:E55_Type4`|
| `crm:E17_Type_Assignment1` | `crm:P21_had_general_purpose` | `xsd:http://vocab.getty.edu/aat/300015646`|
| `crm:E17_Type_Assignment2` | `crm:P42_assigned` | `crm:E55_Type3`|
| `crm:E17_Type_Assignment2` | `crm:P21_had_general_purpose` | `xsd:http://vocab.getty.edu/aat/300179869`|
| `crm:E22_Man-Made_Object1` | `crm:P108i_was_produced_by` | `crm:E12_Production1`|
| `crm:E22_Man-Made_Object1` | `crm:P41i_was_classified_by` | `crm:E17_Type_Assignment1`|
| `crm:E22_Man-Made_Object1` | `crm:P41i_was_classified_by` | `crm:E17_Type_Assignment2`|
| `crm:E22_Man-Made_Object1` | `crm:P67i_is_referred_to_by` | `crm:E33_Linguistic_Object1`|
| `crm:E22_Man-Made_Object1` | `crm:P67i_is_referred_to_by` | `crm:E33_Linguistic_Object2`|
| `crm:E22_Man-Made_Object1` | `crm:P129i_is_subject_of` | `crm:E33_Linguistic_Object3`|
| `crm:E22_Man-Made_Object1` | `crm:P102_has_title` | `crm:E35_Title1`|
| `crm:E22_Man-Made_Object1` | `crm:P138i_has_representation` | `crm:E38_Image1`|
| `crm:E22_Man-Made_Object1` | `crm:P1_is_identified_by` | `crm:E42_Identifier1`|
| `crm:E22_Man-Made_Object1` | `crm:P45_consists_of` | `crm:E57_Material1`|
| `crm:E22_Man-Made_Object1` | `foaf:homepage` | `foaf:Document1`|
| `crm:E22_Man-Made_Object1` | `crm:P2_has_type` | `crm:E55_Type3`|
| `crm:E33_Linguistic_Object1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300026687`|
| `crm:E33_Linguistic_Object2` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300266036`|
| `crm:E33_Linguistic_Object3` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300080091`|
| `crm:E33_Linguistic_Object3` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `crm:E35_Title1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404670`|
| `crm:E42_Identifier1` | `crm:P2_has_type` | `xsd:http://vocab.getty.edu/aat/300404621`|

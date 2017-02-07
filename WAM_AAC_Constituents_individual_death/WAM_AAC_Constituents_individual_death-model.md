# WAM_XMLExport_AAC_Constituents_V3.xml

## Add Column

## Add Node/Literal

## PyTransforms
#### _ConstituentURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentID_
``` python
if getValue("ConstituentType"):
    return "constituent/"+getValue("ConstituentID")
else:
    ""
```

#### _NotInUse1_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentType_
``` python
if getValue("ThesGeographyTerm"):
    return getValue("ConstituentURI")+"/death"
else:
    return ""
```

#### _NotInUse_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentType_
``` python
if getValue("ThesGeographyTerm"):
    return getValue("DeathURI")+"/location"
else:
    return ""
```

#### _DeathURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / ThesGeographyTerm_
``` python
if getValue("ThesGeographyTerm"):
    return getValue("ConstituentURI")+"/death"
else:
    return ""
```

#### _DeathLocationURI_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / ThesGeographyTerm_
``` python
if getValue("ThesGeographyTerm"):
    return getValue("DeathURI")+"/location"
else:
    return ""
```


## Selections
#### _DEFAULT_TEST_
From column: _Root / ObjRecord / Constituents / ObjectRelatedConstituent / ConstituentGeography / ConstituentGeography / ThesGeographyTerm_
<br>Operation: `Union`
``` python
return getValue("ThesGeoType")!='Death Location'
```


## Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _ConstituentURI_ | `uri` | `crm:E39_Actor1`|
| _DeathLocationURI_ | `uri` | `crm:E53_Place1`|
| _DeathURI_ | `uri` | `crm:E64_End_of_Existence1`|
| _ThesGeographyTerm_ | `rdfs:label` | `crm:E53_Place1`|


## Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E39_Actor1` | `crm:P93i_was_taken_out_of_existence_by` | `crm:E64_End_of_Existence1`|
| `crm:E64_End_of_Existence1` | `crm:P7_took_place_at` | `crm:E53_Place1`|

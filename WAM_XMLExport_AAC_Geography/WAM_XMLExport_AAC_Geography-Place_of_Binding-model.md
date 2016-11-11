## WAM_XMLExport_AAC_Geography.xml

### PyTransforms
#### _ObjectURI_
From column: _Root / ObjRecord / ObjectURI_
``` python
return "object/" + getValue("ObjectID")
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

#### _TGNTermID_URI_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / TGNTermID_URI_
``` python
tgnTermId = getValue("TGNTermID")
if tgnTermId:
    return "http://vocab.getty.edu/tgn/" + tgnTermId + "-place"
else:
    return ""
```

#### _ObjectID_GeographyID_
From column: _Root / ObjRecord / ObjectRelatedGeography / Geography / ObjectID_GeographyID_
``` python
return "object_boundAt/" + getValue("ObjectID") + "_" + getValue("GeographyID")
```


### Semantic Types
| Column | Property | Class |
|  ----- | -------- | ----- |
| _ExhBeginISODate_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span1`|
| _ExhEndISODate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span1`|
| _ExhTitle_ | `rdfs:label` | `crm:E41_Appellation1`|
| _ExhVenueURI_ | `uri` | `crm:E93_Presence1`|
| _ExhibCitation_ | `crm:P3_has_note` | `crm:E33_Linguistic_Object1`|
| _ExhibCitationURI_ | `uri` | `crm:E33_Linguistic_Object1`|
| _ExhibitionTimeSpanURI_ | `uri` | `crm:E52_Time-Span1`|
| _ExhibitionTitleURI_ | `uri` | `crm:E41_Appellation1`|
| _ExhibitionURI_ | `uri` | `crm:E7_Activity1`|
| _GeoType_ | `rdfs:label` | `crm:E55_Type1`|
| _GeoTypeURI_ | `uri` | `crm:E55_Type1`|
| _GeographyID_ | `rdfs:label` | `crm:E42_Identifier2`|
| _GeographyID_ | `rdfs:label` | `crm:E42_Identifier2`|
| _GeographyID_URI_ | `uri` | `crm:E53_Place1`|
| _GeographyTerm_ | `rdfs:label` | `crm:E48_Place_Name1`|
| _GeographyTerm_ | `rdfs:label` | `crm:E48_Place_Name1`|
| _ObjectID_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectID_ | `rdfs:label` | `crm:E42_Identifier1`|
| _ObjectID_GeographyID_ | `uri` | `crm:E11_Modification1`|
| _ObjectID_GeographyID_ | `uri` | `crm:E11_Modification1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _ObjectURI_ | `uri` | `crm:E42_Identifier1`|
| _ObjectURI_ | `uri` | `crm:E22_Man-Made_Object1`|
| _PlaceURI_ | `uri` | `crm:E53_Place1`|
| _SpatialCoOrdinates_ | `rdfs:label` | `crm:E47_Spatial_Coordinates1`|
| _SpatialCoOrdinates_ | `rdfs:label` | `crm:E47_Spatial_Coordinates1`|
| _TGNTermID_ | `rdfs:label` | `crm:E42_Identifier3`|
| _TGNTermID_ | `rdfs:label` | `crm:E42_Identifier3`|
| _TGNTermIDURI_ | `uri` | `crm:E42_Identifier3`|
| _TGNTermID_URI_ | `uri` | `crm:E42_Identifier3`|
| _Title_ | `rdfs:label` | `crm:E35_Title1`|
| _TitleType_ | `rdfs:label` | `crm:E55_Type1`|
| _TitleTypeURI_ | `uri` | `crm:E55_Type1`|
| _TitleURI_ | `uri` | `crm:E35_Title1`|
| _TitleURI_ | `uri` | `crm:E35_Title1`|
| _VenueBegDate_ | `crm:P82a_begin_of_the_begin` | `crm:E52_Time-Span2`|
| _VenueDisplayName_ | `rdfs:label` | `crm:E93_Presence1`|
| _VenueEndDate_ | `crm:P82b_end_of_the_end` | `crm:E52_Time-Span2`|


### Links
| From | Property | To |
|  --- | -------- | ---|
| `crm:E11_Modification1` | `crm:P7_took_place_at` | `crm:E53_Place1`|
| `crm:E22_Man-Made_Object1` | `crm:P31i_was_modified_by` | `crm:E11_Modification1`|
| `crm:E22_Man-Made_Object1` | `crm:P48_has_preferred_identifier` | `crm:E42_Identifier1`|
| `crm:E53_Place1` | `crm:P48_has_preferred_identifier` | `crm:E42_Identifier2`|
| `crm:E53_Place1` | `crm:P1_is_identified_by` | `crm:E42_Identifier3`|
| `crm:E53_Place1` | `crm:P1_is_identified_by` | `crm:E47_Spatial_Coordinates1`|
| `crm:E53_Place1` | `crm:P1_is_identified_by` | `crm:E48_Place_Name1`|
| `crm:E53_Place1` | `crm:P2i_is_type_of` | `crm:E55_Type1`|

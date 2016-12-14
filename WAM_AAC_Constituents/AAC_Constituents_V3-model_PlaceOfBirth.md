@prefix dct: <http://purl.org/dc/terms/> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix dc: <http://purl.org/dc/elements/1.1/> .
@prefix vs: <http://www.w3.org/2003/06/sw-vocab-status/ns#> .
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .
@prefix dcam: <http://purl.org/dc/dcam/> .
@prefix skos: <http://www.w3.org/2004/02/skos/core#> .
@prefix wot: <http://xmlns.com/wot/0.1/> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix foaf: <http://xmlns.com/foaf/0.1/> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
@prefix rr: <http://www.w3.org/ns/r2rml#> .
@prefix km-dev: <http://isi.edu/integration/karma/dev#> .

_:node1b3thi6ccx1 a km-dev:R2RMLMapping ;
	km-dev:sourceName "WAM_XMLExport_AAC_Constituents_V3.xml" ;
	km-dev:modelPublicationTime "1481681475980"^^xsd:long ;
	km-dev:modelVersion "1.7" ;
	km-dev:hasInputColumns "[[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"ObjectID\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"Biography\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConGeoLatDirection\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentID\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ThesGeographyTerm\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConGeoTGNSourceTermID\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConGeoLongitude\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"DisplayName\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConGeoLongDirection\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConGeoLatitude\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"Gender\"}]]" ;
	km-dev:hasOutputColumns "[[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"BiographyURI\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"birthPlaceURI\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"ObjectID_URI\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"GenderURI\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"ObjectLabel\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"SpatialCoOrdinates\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConGeoTGNSourceTermID_URI\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"PlaceURI\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentURI\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"IdURI\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"AppellationURI\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"birthPlace\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"ObjectID\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"Biography\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ThesGeoType\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"AppellationValue\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ThesGeographyTerm\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConstituentGeography\"},{\"columnName\":\"ConGeoTGNSourceTermID\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"ConstituentType\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"DisplayName\"}],[{\"columnName\":\"Root\"},{\"columnName\":\"ObjRecord\"},{\"columnName\":\"Constituents\"},{\"columnName\":\"ObjectRelatedConstituent\"},{\"columnName\":\"Gender\"}]]" ;
	km-dev:hasModelLabel "WAM_XMLExport_AAC_Constituents_V3.xml" ;
	km-dev:hasBaseURI "http://localhost:8080/source/" ;
	km-dev:hasWorksheetHistory """[
    {
        \"commandName\": \"SubmitPythonTransformationCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"ObjectID\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"newColumnName\",
                \"type\": \"other\",
                \"value\": \"IdURI\"
            },
            {
                \"name\": \"transformationCode\",
                \"type\": \"other\",
                \"value\": \"return \\\"id/\\\" + getValue(\\\"ObjectID\\\")\"
            },
            {
                \"name\": \"errorDefaultValue\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"isJSONOutput\",
                \"type\": \"other\",
                \"value\": \"false\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"ObjectID\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"IdURI\\\"}]}]\"
            }
        ],
        \"tags\": [\"Transformation\"]
    },
    {
        \"commandName\": \"SubmitPythonTransformationCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"ObjectID\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"newColumnName\",
                \"type\": \"other\",
                \"value\": \"ObjectLabel\"
            },
            {
                \"name\": \"transformationCode\",
                \"type\": \"other\",
                \"value\": \"return getValue(\\\"ObjectID\\\")\"
            },
            {
                \"name\": \"errorDefaultValue\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"isJSONOutput\",
                \"type\": \"other\",
                \"value\": \"false\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"ObjectID\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"ObjectLabel\\\"}]}]\"
            }
        ],
        \"tags\": [\"Transformation\"]
    },
    {
        \"commandName\": \"SubmitPythonTransformationCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"ObjectID\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"newColumnName\",
                \"type\": \"other\",
                \"value\": \"ObjectID_URI\"
            },
            {
                \"name\": \"transformationCode\",
                \"type\": \"other\",
                \"value\": \"return \\\"id/object/\\\" + getValue(\\\"ObjectID\\\")\"
            },
            {
                \"name\": \"errorDefaultValue\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"isJSONOutput\",
                \"type\": \"other\",
                \"value\": \"false\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"ObjectID\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"ObjectID_URI\\\"}]}]\"
            }
        ],
        \"tags\": [\"Transformation\"]
    },
    {
        \"commandName\": \"SubmitPythonTransformationCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"ConstituentID\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"newColumnName\",
                \"type\": \"other\",
                \"value\": \"ConstituentURI\"
            },
            {
                \"name\": \"transformationCode\",
                \"type\": \"other\",
                \"value\": \"return \\\"person-institution/\\\"+getValue(\\\"ConstituentID\\\")\"
            },
            {
                \"name\": \"errorDefaultValue\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"isJSONOutput\",
                \"type\": \"other\",
                \"value\": \"false\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentID\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentURI\\\"}]}]\"
            }
        ],
        \"tags\": [\"Transformation\"]
    },
    {
        \"commandName\": \"SubmitPythonTransformationCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"DisplayName\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"newColumnName\",
                \"type\": \"other\",
                \"value\": \"AppellationValue\"
            },
            {
                \"name\": \"transformationCode\",
                \"type\": \"other\",
                \"value\": \"return getValue(\\\"DisplayName\\\")\"
            },
            {
                \"name\": \"errorDefaultValue\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"isJSONOutput\",
                \"type\": \"other\",
                \"value\": \"false\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"DisplayName\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"AppellationValue\\\"}]}]\"
            }
        ],
        \"tags\": [\"Transformation\"]
    },
    {
        \"commandName\": \"SubmitPythonTransformationCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"AppellationValue\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"newColumnName\",
                \"type\": \"other\",
                \"value\": \"AppellationURI\"
            },
            {
                \"name\": \"transformationCode\",
                \"type\": \"other\",
                \"value\": \"return getValue(\\\"ConstituentURI\\\") + \\\"/appellation/\\\"\"
            },
            {
                \"name\": \"errorDefaultValue\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"isJSONOutput\",
                \"type\": \"other\",
                \"value\": \"false\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentURI\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"AppellationURI\\\"}]}]\"
            }
        ],
        \"tags\": [\"Transformation\"]
    },
    {
        \"commandName\": \"SubmitPythonTransformationCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"Gender\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"newColumnName\",
                \"type\": \"other\",
                \"value\": \"GenderURI\"
            },
            {
                \"name\": \"transformationCode\",
                \"type\": \"other\",
                \"value\": \"gender = getValue(\\\"Gender\\\")\\nif gender:\\n    return \\\"gender/\\\" + gender\\nelse:\\n    return \\\"\\\"\"
            },
            {
                \"name\": \"errorDefaultValue\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"isJSONOutput\",
                \"type\": \"other\",
                \"value\": \"false\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"Gender\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"GenderURI\\\"}]}]\"
            }
        ],
        \"tags\": [\"Transformation\"]
    },
    {
        \"commandName\": \"SubmitPythonTransformationCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"Biography\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"newColumnName\",
                \"type\": \"other\",
                \"value\": \"BiographyURI\"
            },
            {
                \"name\": \"transformationCode\",
                \"type\": \"other\",
                \"value\": \"return getValue(\\\"ConstituentURI\\\") + \\\"/biography/\\\"\"
            },
            {
                \"name\": \"errorDefaultValue\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"isJSONOutput\",
                \"type\": \"other\",
                \"value\": \"false\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentURI\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"BiographyURI\\\"}]}]\"
            }
        ],
        \"tags\": [\"Transformation\"]
    },
    {
        \"commandName\": \"SubmitPythonTransformationCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConGeoLongitudeNumber\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"newColumnName\",
                \"type\": \"other\",
                \"value\": \"SpatialCoOrdinates\"
            },
            {
                \"name\": \"transformationCode\",
                \"type\": \"other\",
                \"value\": \"def format_latLong(str):\\r\\n    deg = u\\\"\\\\u00b0\\\"  # utf code for degree\\r\\n    dim = str.split(' ')\\r\\n    if len(dim) == 2:\\r\\n        return dim[0].lstrip('0') + deg + dim[1] + \\\"\\\\'\\\"\\r\\n    else:\\r\\n        return \\\"\\\"\\r\\nlat = getValue(\\\"ConGeoLatitude\\\")\\r\\nlatDir = getValue(\\\"ConGeoLatDirection\\\")\\r\\nlong = getValue(\\\"ConGeoLongitude\\\")\\r\\nlongDir = getValue(\\\"ConGeoLongDirection\\\")\\r\\nif longDir == \\\"\\\" or latDir == \\\"\\\" or long == \\\"\\\" or lat == \\\"\\\":\\r\\n    return \\\"\\\"\\r\\nelse:\\r\\n    return \\\"\\\\\\\"\\\" + format_latLong(lat)  + \\\" \\\" + latDir +  \\\" \\\" + format_latLong(long) + \\\" \\\" +longDir + \\\"\\\\\\\"\\\"\"
            },
            {
                \"name\": \"errorDefaultValue\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"isJSONOutput\",
                \"type\": \"other\",
                \"value\": \"false\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConGeoLatDirection\\\"}]},{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConGeoLongitude\\\"}]},{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConGeoLongDirection\\\"}]},{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConGeoLatitude\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"SpatialCoOrdinates\\\"}]}]\"
            }
        ],
        \"tags\": [\"Transformation\"]
    },
    {
        \"commandName\": \"SubmitPythonTransformationCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConGeoTGNSourceTermID\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"newColumnName\",
                \"type\": \"other\",
                \"value\": \"ConGeoTGNSourceTermID_URI\"
            },
            {
                \"name\": \"transformationCode\",
                \"type\": \"other\",
                \"value\": \"conGeoTGNSourceTermID = getValue(\\\"ConGeoTGNSourceTermID\\\")\\nif conGeoTGNSourceTermID:\\n    return \\\"http://vocab.getty.edu/tgn/\\\" + conGeoTGNSourceTermID\\nelse:\\n    return \\\"\\\"\"
            },
            {
                \"name\": \"errorDefaultValue\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"isJSONOutput\",
                \"type\": \"other\",
                \"value\": \"false\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConGeoTGNSourceTermID\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConGeoTGNSourceTermID_URI\\\"}]}]\"
            }
        ],
        \"tags\": [\"Transformation\"]
    },
    {
        \"commandName\": \"SubmitPythonTransformationCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConGeoTGNSourceTermID\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"newColumnName\",
                \"type\": \"other\",
                \"value\": \"PlaceURI\"
            },
            {
                \"name\": \"transformationCode\",
                \"type\": \"other\",
                \"value\": \"return getValue(\\\"ConGeoTGNSourceTermID\\\")\"
            },
            {
                \"name\": \"errorDefaultValue\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"isJSONOutput\",
                \"type\": \"other\",
                \"value\": \"false\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConGeoTGNSourceTermID\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"PlaceURI\\\"}]}]\"
            }
        ],
        \"tags\": [\"Transformation\"]
    },
    {
        \"commandName\": \"SubmitPythonTransformationCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ThesGeographyTerm\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"newColumnName\",
                \"type\": \"other\",
                \"value\": \"birthPlace\"
            },
            {
                \"name\": \"transformationCode\",
                \"type\": \"other\",
                \"value\": \"return getValue(\\\"ThesGeographyTerm\\\")\"
            },
            {
                \"name\": \"errorDefaultValue\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"isJSONOutput\",
                \"type\": \"other\",
                \"value\": \"false\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ThesGeographyTerm\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"birthPlace\\\"}]}]\"
            }
        ],
        \"tags\": [\"Transformation\"]
    },
    {
        \"commandName\": \"SubmitPythonTransformationCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"birthPlace\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"newColumnName\",
                \"type\": \"other\",
                \"value\": \"birthPlaceURI\"
            },
            {
                \"name\": \"transformationCode\",
                \"type\": \"other\",
                \"value\": \"conGeoTGNSrcTermID = getValue(\\\"ConGeoTGNSourceTermID\\\")\\r\\nif conGeoTGNSrcTermID:\\r\\n    return getValue(\\\"ConstituentURI\\\")+\\\"/birth/\\\"\\r\\nelse:\\r\\n    return \\\"\\\"\"
            },
            {
                \"name\": \"errorDefaultValue\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"isJSONOutput\",
                \"type\": \"other\",
                \"value\": \"false\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConGeoTGNSourceTermID\\\"}]},{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentURI\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"birthPlaceURI\\\"}]}]\"
            }
        ],
        \"tags\": [\"Transformation\"]
    },
    {
        \"commandName\": \"OperateSelectionCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"Gender\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"pythonCode\",
                \"type\": \"other\",
                \"value\": \"return getValue(\\\"ConstituentType\\\") == \\\"Institution\\\"\"
            },
            {
                \"name\": \"operation\",
                \"type\": \"other\",
                \"value\": \"Union\"
            },
            {
                \"name\": \"onError\",
                \"type\": \"other\",
                \"value\": \"true\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentType\\\"}]}]\"
            }
        ],
        \"tags\": [\"Selection\"]
    },
    {
        \"commandName\": \"OperateSelectionCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"values\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"pythonCode\",
                \"type\": \"other\",
                \"value\": \"return getValue(\\\"ThesGeoType\\\") != \\\"Birth Location\\\"\"
            },
            {
                \"name\": \"operation\",
                \"type\": \"other\",
                \"value\": \"Union\"
            },
            {
                \"name\": \"onError\",
                \"type\": \"other\",
                \"value\": \"true\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ThesGeoType\\\"}]}]\"
            }
        ],
        \"tags\": [\"Selection\"]
    },
    {
        \"commandName\": \"SetSemanticTypeCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"ObjectID\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://www.w3.org/1999/02/22-rdf-syntax-ns#value\",
                    \"DomainLabel\": \"crm:E42_Identifier1 (add)\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"ObjectID\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"ObjectID\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetSemanticTypeCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"ObjectLabel\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://www.w3.org/2000/01/rdf-schema#label\",
                    \"DomainLabel\": \"crm:E42_Identifier1\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"ObjectLabel\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"ObjectLabel\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetMetaPropertyCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"IdURI\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"metaPropertyName\",
                \"type\": \"other\",
                \"value\": \"isUriOfClass\"
            },
            {
                \"name\": \"metaPropertyUri\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier\"
            },
            {
                \"name\": \"metaPropertyId\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier1\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://isi.edu/integration/karma/dev#classLink\",
                    \"DomainLabel\": \"crm:E42_Identifier1\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"IdURI\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"IdURI\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetMetaPropertyCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"ObjectID_URI\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"metaPropertyName\",
                \"type\": \"other\",
                \"value\": \"isUriOfClass\"
            },
            {
                \"name\": \"metaPropertyUri\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object\"
            },
            {
                \"name\": \"metaPropertyId\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://isi.edu/integration/karma/dev#classLink\",
                    \"DomainLabel\": \"crm:E22_Man-Made_Object1 (add)\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"ObjectID_URI\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"ObjectID_URI\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"AddLiteralNodeCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"literalValue\",
                \"type\": \"other\",
                \"value\": \"http://vocab.getty.edu/aat/300404621\"
            },
            {
                \"name\": \"literalType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"isUri\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetMetaPropertyCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"ConstituentURI\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"metaPropertyName\",
                \"type\": \"other\",
                \"value\": \"isUriOfClass\"
            },
            {
                \"name\": \"metaPropertyUri\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor\"
            },
            {
                \"name\": \"metaPropertyId\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor1\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://isi.edu/integration/karma/dev#classLink\",
                    \"DomainLabel\": \"crm:E39_Actor1 (add)\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentURI\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentURI\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetSemanticTypeCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"DisplayName\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://www.w3.org/2000/01/rdf-schema#label\",
                    \"DomainLabel\": \"crm:E39_Actor1\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"DisplayName\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"DisplayName\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetSemanticTypeCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"AppellationValue\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E82_Actor_Appellation\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E82_Actor_Appellation1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://www.w3.org/1999/02/22-rdf-syntax-ns#value\",
                    \"DomainLabel\": \"crm:E82_Actor_Appellation1 (add)\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"AppellationValue\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"AppellationValue\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetMetaPropertyCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"AppellationURI\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"metaPropertyName\",
                \"type\": \"other\",
                \"value\": \"isUriOfClass\"
            },
            {
                \"name\": \"metaPropertyUri\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E82_Actor_Appellation\"
            },
            {
                \"name\": \"metaPropertyId\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E82_Actor_Appellation1\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E82_Actor_Appellation\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E82_Actor_Appellation1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://isi.edu/integration/karma/dev#classLink\",
                    \"DomainLabel\": \"crm:E82_Actor_Appellation1\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"AppellationURI\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"AppellationURI\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetMetaPropertyCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"GenderURI\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"metaPropertyName\",
                \"type\": \"other\",
                \"value\": \"isUriOfClass\"
            },
            {
                \"name\": \"metaPropertyUri\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type\"
            },
            {
                \"name\": \"metaPropertyId\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type1\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://isi.edu/integration/karma/dev#classLink\",
                    \"DomainLabel\": \"crm:E55_Type1 (add)\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"GenderURI\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"GenderURI\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetSemanticTypeCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"Gender\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://www.w3.org/2000/01/rdf-schema#label\",
                    \"DomainLabel\": \"crm:E55_Type1\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"Gender\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"Gender\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetSemanticTypeCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"Biography\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E33_Linguistic_Object\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E33_Linguistic_Object1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://www.w3.org/1999/02/22-rdf-syntax-ns#value\",
                    \"DomainLabel\": \"crm:E33_Linguistic_Object1 (add)\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"Biography\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"Biography\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetMetaPropertyCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"BiographyURI\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"metaPropertyName\",
                \"type\": \"other\",
                \"value\": \"isUriOfClass\"
            },
            {
                \"name\": \"metaPropertyUri\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E33_Linguistic_Object\"
            },
            {
                \"name\": \"metaPropertyId\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E33_Linguistic_Object1\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E33_Linguistic_Object\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E33_Linguistic_Object1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://isi.edu/integration/karma/dev#classLink\",
                    \"DomainLabel\": \"crm:E33_Linguistic_Object1\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"BiographyURI\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"BiographyURI\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"AddLiteralNodeCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"literalValue\",
                \"type\": \"other\",
                \"value\": \"http://vocab.getty.edu/aat/300404670\"
            },
            {
                \"name\": \"literalType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"isUri\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"AddLiteralNodeCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"literalValue\",
                \"type\": \"other\",
                \"value\": \"http://vocab.getty.edu/aat/300080102\"
            },
            {
                \"name\": \"literalType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"isUri\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"AddLiteralNodeCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"literalValue\",
                \"type\": \"other\",
                \"value\": \"http://vocab.getty.edu/aat/300055147\"
            },
            {
                \"name\": \"literalType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"isUri\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"AddLiteralNodeCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"literalValue\",
                \"type\": \"other\",
                \"value\": \"http://vocab.getty.edu/aat/300404670\"
            },
            {
                \"name\": \"literalType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"isUri\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetSemanticTypeCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"SpatialCoOrdinates\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E47_Spatial_Coordinates\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E47_Spatial_Coordinates1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://www.w3.org/2000/01/rdf-schema#label\",
                    \"DomainLabel\": \"crm:E47_Spatial_Coordinates1 (add)\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"SpatialCoOrdinates\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"SpatialCoOrdinates\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetSemanticTypeCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConGeoTGNSourceTermID\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier2\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://www.w3.org/2000/01/rdf-schema#label\",
                    \"DomainLabel\": \"crm:E42_Identifier2 (add)\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConGeoTGNSourceTermID\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConGeoTGNSourceTermID\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetMetaPropertyCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConGeoTGNSourceTermID_URI\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"metaPropertyName\",
                \"type\": \"other\",
                \"value\": \"isUriOfClass\"
            },
            {
                \"name\": \"metaPropertyUri\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier\"
            },
            {
                \"name\": \"metaPropertyId\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier2\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier2\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://isi.edu/integration/karma/dev#classLink\",
                    \"DomainLabel\": \"crm:E42_Identifier2\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConGeoTGNSourceTermID_URI\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConGeoTGNSourceTermID_URI\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetMetaPropertyCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"PlaceURI\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"metaPropertyName\",
                \"type\": \"other\",
                \"value\": \"isUriOfClass\"
            },
            {
                \"name\": \"metaPropertyUri\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place\"
            },
            {
                \"name\": \"metaPropertyId\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place1\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://isi.edu/integration/karma/dev#classLink\",
                    \"DomainLabel\": \"crm:E53_Place1\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"PlaceURI\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"PlaceURI\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetSemanticTypeCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ThesGeographyTerm\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E48_Place_Name\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E48_Place_Name1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://www.w3.org/2000/01/rdf-schema#label\",
                    \"DomainLabel\": \"crm:E48_Place_Name1 (add)\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ThesGeographyTerm\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ThesGeographyTerm\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetSemanticTypeCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"birthPlace\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://www.w3.org/2000/01/rdf-schema#label\",
                    \"DomainLabel\": \"crm:E53_Place1\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"birthPlace\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"birthPlace\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"SetMetaPropertyCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"hNodeId\",
                \"type\": \"hNodeId\",
                \"value\": [
                    {\"columnName\": \"Root\"},
                    {\"columnName\": \"ObjRecord\"},
                    {\"columnName\": \"Constituents\"},
                    {\"columnName\": \"ObjectRelatedConstituent\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"ConstituentGeography\"},
                    {\"columnName\": \"birthPlaceURI\"}
                ]
            },
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"metaPropertyName\",
                \"type\": \"other\",
                \"value\": \"isUriOfClass\"
            },
            {
                \"name\": \"metaPropertyUri\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E63_Beginning_of_Existence\"
            },
            {
                \"name\": \"metaPropertyId\",
                \"type\": \"other\",
                \"value\": \"http://www.cidoc-crm.org/cidoc-crm/E63_Beginning_of_Existence1\"
            },
            {
                \"name\": \"SemanticTypesArray\",
                \"type\": \"other\",
                \"value\": [{
                    \"DomainUri\": \"http://www.cidoc-crm.org/cidoc-crm/E63_Beginning_of_Existence\",
                    \"DomainId\": \"http://www.cidoc-crm.org/cidoc-crm/E63_Beginning_of_Existence1\",
                    \"isPrimary\": true,
                    \"FullType\": \"http://isi.edu/integration/karma/dev#classLink\",
                    \"DomainLabel\": \"crm:E63_Beginning_of_Existence1\"
                }]
            },
            {
                \"name\": \"trainAndShowUpdates\",
                \"type\": \"other\",
                \"value\": true
            },
            {
                \"name\": \"rdfLiteralType\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"language\",
                \"type\": \"other\",
                \"value\": \"\"
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"birthPlaceURI\\\"}]}]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[{\\\"value\\\":[{\\\"columnName\\\":\\\"Root\\\"},{\\\"columnName\\\":\\\"ObjRecord\\\"},{\\\"columnName\\\":\\\"Constituents\\\"},{\\\"columnName\\\":\\\"ObjectRelatedConstituent\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"ConstituentGeography\\\"},{\\\"columnName\\\":\\\"birthPlaceURI\\\"}]}]\"
            }
        ],
        \"tags\": [\"SemanticType\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E35_Title1\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P102_has_title\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\"
                }]
            },
            {
                \"name\": \"alignmentId\",
                \"type\": \"other\",
                \"value\": \"WSP10:WS5AL\"
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"alignmentId\",
                \"type\": \"other\",
                \"value\": \"WSP10:WS5AL\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier1\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P48_has_preferred_identifier\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\"
                }]
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier1\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P1_is_identified_by\",
                    \"edgeTargetUri\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\",
                    \"edgeSourceUri\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object\"
                }]
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://vocab.getty.edu/aat/3004046211\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P2_has_type\",
                    \"edgeTargetUri\": \"http://vocab.getty.edu/aat/300404621\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier1\",
                    \"edgeSourceUri\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier\"
                }]
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place1\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P62_depicts\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\"
                }]
            },
            {
                \"name\": \"alignmentId\",
                \"type\": \"other\",
                \"value\": \"WSP10:WS5AL\"
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place1\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P53_has_former_or_current_location\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\"
                }]
            },
            {
                \"name\": \"alignmentId\",
                \"type\": \"other\",
                \"value\": \"WSP10:WS5AL\"
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type1\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P2i_is_type_of\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place1\"
                }]
            },
            {
                \"name\": \"alignmentId\",
                \"type\": \"other\",
                \"value\": \"WSP10:WS5AL\"
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type1\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P2_has_type\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\"
                }]
            },
            {
                \"name\": \"alignmentId\",
                \"type\": \"other\",
                \"value\": \"WSP10:WS5AL\"
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E5_Event1\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P129_is_about\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E33_Linguistic_Object1\"
                }]
            },
            {
                \"name\": \"alignmentId\",
                \"type\": \"other\",
                \"value\": \"WSP10:WS5AL\"
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://vocab.getty.edu/aat/3004046701\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P2_has_type\",
                    \"edgeTargetUri\": \"http://vocab.getty.edu/aat/300404670\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E33_Linguistic_Object1\",
                    \"edgeSourceUri\": \"http://www.cidoc-crm.org/cidoc-crm/E33_Linguistic_Object\"
                }]
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://vocab.getty.edu/aat/3000801021\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P2_has_type\",
                    \"edgeTargetUri\": \"http://vocab.getty.edu/aat/300080102\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E33_Linguistic_Object1\",
                    \"edgeSourceUri\": \"http://www.cidoc-crm.org/cidoc-crm/E33_Linguistic_Object\"
                }]
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"alignmentId\",
                \"type\": \"other\",
                \"value\": \"WSP10:WS5AL\"
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type2\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P2_has_type\",
                    \"edgeTargetUri\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type1\",
                    \"edgeSourceUri\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type\"
                }]
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://vocab.getty.edu/aat/3000551471\",
                    \"edgeId\": \"http://www.w3.org/2004/02/skos/core#broadMatch\",
                    \"edgeTargetUri\": \"http://vocab.getty.edu/aat/300055147\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type2\",
                    \"edgeSourceUri\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type\"
                }]
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://vocab.getty.edu/aat/3004046702\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P2_has_type\",
                    \"edgeTargetUri\": \"http://vocab.getty.edu/aat/300404670\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E82_Actor_Appellation1\",
                    \"edgeSourceUri\": \"http://www.cidoc-crm.org/cidoc-crm/E82_Actor_Appellation\"
                }]
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place1\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P7_took_place_at\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E11_Modification1\"
                }]
            },
            {
                \"name\": \"alignmentId\",
                \"type\": \"other\",
                \"value\": \"WSP10:WS5AL\"
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E5_Event1\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P12i_was_present_at\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\"
                }]
            },
            {
                \"name\": \"alignmentId\",
                \"type\": \"other\",
                \"value\": \"WSP10:WS5AL\"
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": [
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier2\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P48_has_preferred_identifier\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P14_carried_out_by\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E12_Production1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E12_Production1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P108i_was_produced_by\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E47_Spatial_Coordinates1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P1_is_identified_by\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P2_has_type\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E48_Place_Name1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P1_is_identified_by\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P31_has_modified\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E11_Modification1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E82_Actor_Appellation1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P131_is_identified_by\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P7_took_place_at\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E63_Beginning_of_Existence1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E33_Linguistic_Object1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P129i_is_subject_of\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E63_Beginning_of_Existence1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P92i_was_brought_into_existence_by\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor1\"
                    }
                ]
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": [
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E42_Identifier2\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P48_has_preferred_identifier\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P14_carried_out_by\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E12_Production1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E12_Production1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P108i_was_produced_by\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E47_Spatial_Coordinates1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P1_is_identified_by\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E55_Type1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P2_has_type\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E48_Place_Name1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P1_is_identified_by\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P31_has_modified\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E11_Modification1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E82_Actor_Appellation1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P131_is_identified_by\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E53_Place1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P7_took_place_at\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E63_Beginning_of_Existence1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E33_Linguistic_Object1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P129i_is_subject_of\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\"
                    },
                    {
                        \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E63_Beginning_of_Existence1\",
                        \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P92i_was_brought_into_existence_by\",
                        \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor1\"
                    }
                ]
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E63_Beginning_of_Existence1\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P92i_was_brought_into_existence_by\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor1\"
                }]
            },
            {
                \"name\": \"alignmentId\",
                \"type\": \"other\",
                \"value\": \"WSP10:WS13142AL\"
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"alignmentId\",
                \"type\": \"other\",
                \"value\": \"WSP10:WS13142AL\"
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E63_Beginning_of_Existence1\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P92i_was_brought_into_existence_by\",
                    \"edgeTargetUri\": \"http://www.cidoc-crm.org/cidoc-crm/E63_Beginning_of_Existence\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\",
                    \"edgeSourceUri\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object\"
                }]
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E63_Beginning_of_Existence1\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P92i_was_brought_into_existence_by\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\"
                }]
            },
            {
                \"name\": \"alignmentId\",
                \"type\": \"other\",
                \"value\": \"WSP10:WS13142AL\"
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"alignmentId\",
                \"type\": \"other\",
                \"value\": \"WSP10:WS13142AL\"
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E63_Beginning_of_Existence1\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P92i_was_brought_into_existence_by\",
                    \"edgeTargetUri\": \"http://www.cidoc-crm.org/cidoc-crm/E63_Beginning_of_Existence\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor1\",
                    \"edgeSourceUri\": \"http://www.cidoc-crm.org/cidoc-crm/E39_Actor\"
                }]
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    },
    {
        \"commandName\": \"ChangeInternalNodeLinksCommand\",
        \"model\": \"new\",
        \"inputParameters\": [
            {
                \"name\": \"worksheetId\",
                \"type\": \"worksheetId\",
                \"value\": \"W\"
            },
            {
                \"name\": \"selectionName\",
                \"type\": \"other\",
                \"value\": \"DEFAULT_TEST\"
            },
            {
                \"name\": \"initialEdges\",
                \"type\": \"other\",
                \"value\": [{
                    \"edgeTargetId\": \"http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1\",
                    \"edgeId\": \"http://www.cidoc-crm.org/cidoc-crm/P31_has_modified\",
                    \"edgeSourceId\": \"http://www.cidoc-crm.org/cidoc-crm/E11_Modification1\"
                }]
            },
            {
                \"name\": \"alignmentId\",
                \"type\": \"other\",
                \"value\": \"WSP10:WS13142AL\"
            },
            {
                \"name\": \"newEdges\",
                \"type\": \"other\",
                \"value\": []
            },
            {
                \"name\": \"inputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            },
            {
                \"name\": \"outputColumns\",
                \"type\": \"hNodeIdList\",
                \"value\": \"[]\"
            }
        ],
        \"tags\": [\"Modeling\"]
    }
]""" .

km-dev:TriplesMap_10c3e6ef-ca86-484f-a5ed-9fa1952e63dc a rr:TriplesMap .

_:node1b3thi6ccx1 km-dev:hasTriplesMap km-dev:TriplesMap_10c3e6ef-ca86-484f-a5ed-9fa1952e63dc .

km-dev:TriplesMap_10c3e6ef-ca86-484f-a5ed-9fa1952e63dc km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx2 rr:tableName "WAM_XMLExport_AAC_Constituents_V3.xml" ;
	a rr:LogicalTable ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasLogicalTable _:node1b3thi6ccx2 .

km-dev:TriplesMap_10c3e6ef-ca86-484f-a5ed-9fa1952e63dc rr:logicalTable _:node1b3thi6ccx2 ;
	rr:subjectMap _:node1b3thi6ccx3 .

_:node1b3thi6ccx1 km-dev:hasSubjectMap _:node1b3thi6ccx3 .

_:node1b3thi6ccx3 km-dev:isPartOfMapping _:node1b3thi6ccx1 ;
	a rr:SubjectMap ;
	km-dev:alignmentNodeId "http://www.cidoc-crm.org/cidoc-crm/E12_Production1" ;
	rr:class crm:E12_Production ;
	rr:termType rr:BlankNode ;
	km-dev:namePrefix "crm:E12_Production1" .

km-dev:PredicateObjectMap_3155d415-3923-4c3e-aebf-70614cb58c9f rr:predicate crm:P14_carried_out_by .

km-dev:RefObjectMap_7e676689-6dad-4de6-aaf9-852e64bbe8cb a rr:RefObjectMap , rr:ObjectMap ;
	rr:parentTriplesMap km-dev:TriplesMap_1d080cdd-2a30-4cf0-853f-53f8328e405e ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap km-dev:RefObjectMap_7e676689-6dad-4de6-aaf9-852e64bbe8cb .

km-dev:PredicateObjectMap_3155d415-3923-4c3e-aebf-70614cb58c9f rr:objectMap km-dev:RefObjectMap_7e676689-6dad-4de6-aaf9-852e64bbe8cb .

km-dev:TriplesMap_10c3e6ef-ca86-484f-a5ed-9fa1952e63dc rr:predicateObjectMap km-dev:PredicateObjectMap_3155d415-3923-4c3e-aebf-70614cb58c9f .

km-dev:PredicateObjectMap_3155d415-3923-4c3e-aebf-70614cb58c9f a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_3155d415-3923-4c3e-aebf-70614cb58c9f .

km-dev:TriplesMap_1d080cdd-2a30-4cf0-853f-53f8328e405e a rr:TriplesMap .

_:node1b3thi6ccx1 km-dev:hasTriplesMap km-dev:TriplesMap_1d080cdd-2a30-4cf0-853f-53f8328e405e .

km-dev:TriplesMap_1d080cdd-2a30-4cf0-853f-53f8328e405e km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx4 rr:tableName "WAM_XMLExport_AAC_Constituents_V3.xml" ;
	a rr:LogicalTable ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasLogicalTable _:node1b3thi6ccx4 .

km-dev:TriplesMap_1d080cdd-2a30-4cf0-853f-53f8328e405e rr:logicalTable _:node1b3thi6ccx4 ;
	rr:subjectMap _:node1b3thi6ccx5 .

_:node1b3thi6ccx1 km-dev:hasSubjectMap _:node1b3thi6ccx5 .

_:node1b3thi6ccx5 km-dev:isPartOfMapping _:node1b3thi6ccx1 ;
	a rr:SubjectMap ;
	km-dev:alignmentNodeId "http://www.cidoc-crm.org/cidoc-crm/E39_Actor1" ;
	rr:class crm:E39_Actor ;
	rr:template "person-institution/{[\"Root\",\"ObjRecord\",\"Constituents\",\"ObjectRelatedConstituent\",\"ConstituentID\"]}" .

km-dev:PredicateObjectMap_0599e86e-75a4-45b8-a534-c29ae3cbe223 rr:predicate crm:P2_has_type .

km-dev:RefObjectMap_1d8b4ace-453e-46a0-80ab-85d55bc11a15 a rr:RefObjectMap , rr:ObjectMap ;
	rr:parentTriplesMap km-dev:TriplesMap_fcfa2c95-ed04-48b5-ad79-813752aba33b ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap km-dev:RefObjectMap_1d8b4ace-453e-46a0-80ab-85d55bc11a15 .

km-dev:PredicateObjectMap_0599e86e-75a4-45b8-a534-c29ae3cbe223 rr:objectMap km-dev:RefObjectMap_1d8b4ace-453e-46a0-80ab-85d55bc11a15 .

km-dev:TriplesMap_1d080cdd-2a30-4cf0-853f-53f8328e405e rr:predicateObjectMap km-dev:PredicateObjectMap_0599e86e-75a4-45b8-a534-c29ae3cbe223 .

km-dev:PredicateObjectMap_0599e86e-75a4-45b8-a534-c29ae3cbe223 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_0599e86e-75a4-45b8-a534-c29ae3cbe223 .

km-dev:PredicateObjectMap_4c8fe1e6-5371-4a5b-8e34-9ef03e7e9c9f rr:predicate crm:P92i_was_brought_into_existence_by .

km-dev:RefObjectMap_64f986e0-20d9-49e2-a924-53048e813a03 a rr:RefObjectMap , rr:ObjectMap ;
	rr:parentTriplesMap km-dev:TriplesMap_78f38e81-b850-4868-a39c-08ed2117b2dd ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap km-dev:RefObjectMap_64f986e0-20d9-49e2-a924-53048e813a03 .

km-dev:PredicateObjectMap_4c8fe1e6-5371-4a5b-8e34-9ef03e7e9c9f rr:objectMap km-dev:RefObjectMap_64f986e0-20d9-49e2-a924-53048e813a03 .

km-dev:TriplesMap_1d080cdd-2a30-4cf0-853f-53f8328e405e rr:predicateObjectMap km-dev:PredicateObjectMap_4c8fe1e6-5371-4a5b-8e34-9ef03e7e9c9f .

km-dev:PredicateObjectMap_4c8fe1e6-5371-4a5b-8e34-9ef03e7e9c9f a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_4c8fe1e6-5371-4a5b-8e34-9ef03e7e9c9f .

km-dev:PredicateObjectMap_a425d48d-ea8a-4bb8-ad7c-b1bc554fcd97 rr:predicate crm:P131_is_identified_by .

km-dev:RefObjectMap_0d8a6cf0-d790-4454-b842-fd178bec5faf a rr:RefObjectMap , rr:ObjectMap ;
	rr:parentTriplesMap km-dev:TriplesMap_e223c382-0498-4dc9-a840-3ea21e0b1592 ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap km-dev:RefObjectMap_0d8a6cf0-d790-4454-b842-fd178bec5faf .

km-dev:PredicateObjectMap_a425d48d-ea8a-4bb8-ad7c-b1bc554fcd97 rr:objectMap km-dev:RefObjectMap_0d8a6cf0-d790-4454-b842-fd178bec5faf .

km-dev:TriplesMap_1d080cdd-2a30-4cf0-853f-53f8328e405e rr:predicateObjectMap km-dev:PredicateObjectMap_a425d48d-ea8a-4bb8-ad7c-b1bc554fcd97 .

km-dev:PredicateObjectMap_a425d48d-ea8a-4bb8-ad7c-b1bc554fcd97 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_a425d48d-ea8a-4bb8-ad7c-b1bc554fcd97 .

km-dev:PredicateObjectMap_b5c3e587-d4c0-4021-ab5f-d1f5d04a48d8 rr:predicate rdfs:label .

_:node1b3thi6ccx6 rr:column "[\"Root\",\"ObjRecord\",\"Constituents\",\"ObjectRelatedConstituent\",\"DisplayName\"]" ;
	a rr:ObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap _:node1b3thi6ccx6 .

km-dev:PredicateObjectMap_b5c3e587-d4c0-4021-ab5f-d1f5d04a48d8 rr:objectMap _:node1b3thi6ccx6 .

km-dev:TriplesMap_1d080cdd-2a30-4cf0-853f-53f8328e405e rr:predicateObjectMap km-dev:PredicateObjectMap_b5c3e587-d4c0-4021-ab5f-d1f5d04a48d8 .

km-dev:PredicateObjectMap_b5c3e587-d4c0-4021-ab5f-d1f5d04a48d8 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_b5c3e587-d4c0-4021-ab5f-d1f5d04a48d8 .

km-dev:TriplesMap_8d735aab-0250-4c99-87db-7e70989e6d88 a rr:TriplesMap .

_:node1b3thi6ccx1 km-dev:hasTriplesMap km-dev:TriplesMap_8d735aab-0250-4c99-87db-7e70989e6d88 .

km-dev:TriplesMap_8d735aab-0250-4c99-87db-7e70989e6d88 km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx7 rr:tableName "WAM_XMLExport_AAC_Constituents_V3.xml" ;
	a rr:LogicalTable ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasLogicalTable _:node1b3thi6ccx7 .

km-dev:TriplesMap_8d735aab-0250-4c99-87db-7e70989e6d88 rr:logicalTable _:node1b3thi6ccx7 ;
	rr:subjectMap _:node1b3thi6ccx8 .

_:node1b3thi6ccx1 km-dev:hasSubjectMap _:node1b3thi6ccx8 .

_:node1b3thi6ccx8 km-dev:isPartOfMapping _:node1b3thi6ccx1 ;
	a rr:SubjectMap ;
	km-dev:alignmentNodeId "http://www.cidoc-crm.org/cidoc-crm/E22_Man-Made_Object1" ;
	rr:class crm:E22_Man-Made_Object ;
	rr:template "id/object/{[\"Root\",\"ObjRecord\",\"ObjectID\"]}" ;
	a km-dev:steinerTreeRootNode .

km-dev:PredicateObjectMap_abeb7367-c55b-4c79-bfe0-8a89f5a706c7 rr:predicate crm:P108i_was_produced_by .

km-dev:RefObjectMap_18fb40f0-92e4-4c7b-b1b7-dc792c7c96ca a rr:RefObjectMap , rr:ObjectMap ;
	rr:parentTriplesMap km-dev:TriplesMap_10c3e6ef-ca86-484f-a5ed-9fa1952e63dc ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap km-dev:RefObjectMap_18fb40f0-92e4-4c7b-b1b7-dc792c7c96ca .

km-dev:PredicateObjectMap_abeb7367-c55b-4c79-bfe0-8a89f5a706c7 rr:objectMap km-dev:RefObjectMap_18fb40f0-92e4-4c7b-b1b7-dc792c7c96ca .

km-dev:TriplesMap_8d735aab-0250-4c99-87db-7e70989e6d88 rr:predicateObjectMap km-dev:PredicateObjectMap_abeb7367-c55b-4c79-bfe0-8a89f5a706c7 .

km-dev:PredicateObjectMap_abeb7367-c55b-4c79-bfe0-8a89f5a706c7 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_abeb7367-c55b-4c79-bfe0-8a89f5a706c7 .

km-dev:PredicateObjectMap_7bc86946-2598-47dd-8bdb-00b07cc18ad1 rr:predicate crm:P129i_is_subject_of .

km-dev:RefObjectMap_e79a787e-05d3-4647-83b6-57308fa1cd6f a rr:RefObjectMap , rr:ObjectMap ;
	rr:parentTriplesMap km-dev:TriplesMap_20633a83-e57e-401b-a7fe-fd4bc30519cd ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap km-dev:RefObjectMap_e79a787e-05d3-4647-83b6-57308fa1cd6f .

km-dev:PredicateObjectMap_7bc86946-2598-47dd-8bdb-00b07cc18ad1 rr:objectMap km-dev:RefObjectMap_e79a787e-05d3-4647-83b6-57308fa1cd6f .

km-dev:TriplesMap_8d735aab-0250-4c99-87db-7e70989e6d88 rr:predicateObjectMap km-dev:PredicateObjectMap_7bc86946-2598-47dd-8bdb-00b07cc18ad1 .

km-dev:PredicateObjectMap_7bc86946-2598-47dd-8bdb-00b07cc18ad1 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_7bc86946-2598-47dd-8bdb-00b07cc18ad1 .

km-dev:PredicateObjectMap_62416ba6-97e6-4236-bb53-11fa0265e4a9 rr:predicate crm:P1_is_identified_by .

km-dev:RefObjectMap_6b7a9817-5f23-47f8-a8f7-8a7e5256232a a rr:RefObjectMap , rr:ObjectMap ;
	rr:parentTriplesMap km-dev:TriplesMap_76865276-b8ad-4725-8a71-6ea110652a1a ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap km-dev:RefObjectMap_6b7a9817-5f23-47f8-a8f7-8a7e5256232a .

km-dev:PredicateObjectMap_62416ba6-97e6-4236-bb53-11fa0265e4a9 rr:objectMap km-dev:RefObjectMap_6b7a9817-5f23-47f8-a8f7-8a7e5256232a .

km-dev:TriplesMap_8d735aab-0250-4c99-87db-7e70989e6d88 rr:predicateObjectMap km-dev:PredicateObjectMap_62416ba6-97e6-4236-bb53-11fa0265e4a9 .

km-dev:PredicateObjectMap_62416ba6-97e6-4236-bb53-11fa0265e4a9 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_62416ba6-97e6-4236-bb53-11fa0265e4a9 .

km-dev:TriplesMap_20633a83-e57e-401b-a7fe-fd4bc30519cd a rr:TriplesMap .

_:node1b3thi6ccx1 km-dev:hasTriplesMap km-dev:TriplesMap_20633a83-e57e-401b-a7fe-fd4bc30519cd .

km-dev:TriplesMap_20633a83-e57e-401b-a7fe-fd4bc30519cd km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx9 rr:tableName "WAM_XMLExport_AAC_Constituents_V3.xml" ;
	a rr:LogicalTable ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasLogicalTable _:node1b3thi6ccx9 .

km-dev:TriplesMap_20633a83-e57e-401b-a7fe-fd4bc30519cd rr:logicalTable _:node1b3thi6ccx9 ;
	rr:subjectMap _:node1b3thi6ccx10 .

_:node1b3thi6ccx1 km-dev:hasSubjectMap _:node1b3thi6ccx10 .

_:node1b3thi6ccx10 km-dev:isPartOfMapping _:node1b3thi6ccx1 ;
	a rr:SubjectMap ;
	km-dev:alignmentNodeId "http://www.cidoc-crm.org/cidoc-crm/E33_Linguistic_Object1" ;
	rr:class crm:E33_Linguistic_Object ;
	rr:template "{[\"Root\",\"ObjRecord\",\"Constituents\",\"ObjectRelatedConstituent\",\"ConstituentURI\"]}/biography/" .

km-dev:PredicateObjectMap_5c13e3f8-6d82-416d-9192-0d884a10c56b rr:predicate rdf:value .

_:node1b3thi6ccx11 rr:column "[\"Root\",\"ObjRecord\",\"Constituents\",\"ObjectRelatedConstituent\",\"Biography\"]" ;
	a rr:ObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap _:node1b3thi6ccx11 .

km-dev:PredicateObjectMap_5c13e3f8-6d82-416d-9192-0d884a10c56b rr:objectMap _:node1b3thi6ccx11 .

km-dev:TriplesMap_20633a83-e57e-401b-a7fe-fd4bc30519cd rr:predicateObjectMap km-dev:PredicateObjectMap_5c13e3f8-6d82-416d-9192-0d884a10c56b .

km-dev:PredicateObjectMap_5c13e3f8-6d82-416d-9192-0d884a10c56b a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_5c13e3f8-6d82-416d-9192-0d884a10c56b .

km-dev:PredicateObjectMap_e5425691-0c00-425c-a17a-f8fa0df62cd4 rr:predicate crm:P2_has_type .

_:node1b3thi6ccx12 rr:constant <http://vocab.getty.edu/aat/300404670> ;
	a rr:ObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap _:node1b3thi6ccx12 .

km-dev:PredicateObjectMap_e5425691-0c00-425c-a17a-f8fa0df62cd4 rr:objectMap _:node1b3thi6ccx12 .

km-dev:TriplesMap_20633a83-e57e-401b-a7fe-fd4bc30519cd rr:predicateObjectMap km-dev:PredicateObjectMap_e5425691-0c00-425c-a17a-f8fa0df62cd4 .

km-dev:PredicateObjectMap_e5425691-0c00-425c-a17a-f8fa0df62cd4 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_e5425691-0c00-425c-a17a-f8fa0df62cd4 .

km-dev:PredicateObjectMap_a5831a9e-7956-4db1-8b52-ce41273e1f5b rr:predicate crm:P2_has_type .

_:node1b3thi6ccx13 rr:constant <http://vocab.getty.edu/aat/300080102> ;
	a rr:ObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap _:node1b3thi6ccx13 .

km-dev:PredicateObjectMap_a5831a9e-7956-4db1-8b52-ce41273e1f5b rr:objectMap _:node1b3thi6ccx13 .

km-dev:TriplesMap_20633a83-e57e-401b-a7fe-fd4bc30519cd rr:predicateObjectMap km-dev:PredicateObjectMap_a5831a9e-7956-4db1-8b52-ce41273e1f5b .

km-dev:PredicateObjectMap_a5831a9e-7956-4db1-8b52-ce41273e1f5b a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_a5831a9e-7956-4db1-8b52-ce41273e1f5b .

km-dev:TriplesMap_76865276-b8ad-4725-8a71-6ea110652a1a a rr:TriplesMap .

_:node1b3thi6ccx1 km-dev:hasTriplesMap km-dev:TriplesMap_76865276-b8ad-4725-8a71-6ea110652a1a .

km-dev:TriplesMap_76865276-b8ad-4725-8a71-6ea110652a1a km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx14 rr:tableName "WAM_XMLExport_AAC_Constituents_V3.xml" ;
	a rr:LogicalTable ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasLogicalTable _:node1b3thi6ccx14 .

km-dev:TriplesMap_76865276-b8ad-4725-8a71-6ea110652a1a rr:logicalTable _:node1b3thi6ccx14 ;
	rr:subjectMap _:node1b3thi6ccx15 .

_:node1b3thi6ccx1 km-dev:hasSubjectMap _:node1b3thi6ccx15 .

_:node1b3thi6ccx15 km-dev:isPartOfMapping _:node1b3thi6ccx1 ;
	a rr:SubjectMap ;
	km-dev:alignmentNodeId "http://www.cidoc-crm.org/cidoc-crm/E42_Identifier1" ;
	rr:class crm:E42_Identifier ;
	rr:template "id/{[\"Root\",\"ObjRecord\",\"ObjectID\"]}" .

km-dev:PredicateObjectMap_376dba58-eb5e-44f0-93cc-5b9153d14412 rr:predicate rdfs:label .

_:node1b3thi6ccx16 rr:column "[\"Root\",\"ObjRecord\",\"ObjectID\"]" ;
	a rr:ObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap _:node1b3thi6ccx16 .

km-dev:PredicateObjectMap_376dba58-eb5e-44f0-93cc-5b9153d14412 rr:objectMap _:node1b3thi6ccx16 .

km-dev:TriplesMap_76865276-b8ad-4725-8a71-6ea110652a1a rr:predicateObjectMap km-dev:PredicateObjectMap_376dba58-eb5e-44f0-93cc-5b9153d14412 .

km-dev:PredicateObjectMap_376dba58-eb5e-44f0-93cc-5b9153d14412 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_376dba58-eb5e-44f0-93cc-5b9153d14412 .

km-dev:PredicateObjectMap_b210ecc1-bfba-4be0-9d84-cdebd1b70364 rr:predicate rdf:value .

_:node1b3thi6ccx17 rr:column "[\"Root\",\"ObjRecord\",\"ObjectID\"]" ;
	a rr:ObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap _:node1b3thi6ccx17 .

km-dev:PredicateObjectMap_b210ecc1-bfba-4be0-9d84-cdebd1b70364 rr:objectMap _:node1b3thi6ccx17 .

km-dev:TriplesMap_76865276-b8ad-4725-8a71-6ea110652a1a rr:predicateObjectMap km-dev:PredicateObjectMap_b210ecc1-bfba-4be0-9d84-cdebd1b70364 .

km-dev:PredicateObjectMap_b210ecc1-bfba-4be0-9d84-cdebd1b70364 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_b210ecc1-bfba-4be0-9d84-cdebd1b70364 .

km-dev:PredicateObjectMap_83c4475c-84ca-4934-b586-71d9f511b1a6 rr:predicate crm:P2_has_type .

_:node1b3thi6ccx18 rr:constant <http://vocab.getty.edu/aat/300404621> ;
	a rr:ObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap _:node1b3thi6ccx18 .

km-dev:PredicateObjectMap_83c4475c-84ca-4934-b586-71d9f511b1a6 rr:objectMap _:node1b3thi6ccx18 .

km-dev:TriplesMap_76865276-b8ad-4725-8a71-6ea110652a1a rr:predicateObjectMap km-dev:PredicateObjectMap_83c4475c-84ca-4934-b586-71d9f511b1a6 .

km-dev:PredicateObjectMap_83c4475c-84ca-4934-b586-71d9f511b1a6 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_83c4475c-84ca-4934-b586-71d9f511b1a6 .

km-dev:TriplesMap_fcfa2c95-ed04-48b5-ad79-813752aba33b a rr:TriplesMap .

_:node1b3thi6ccx1 km-dev:hasTriplesMap km-dev:TriplesMap_fcfa2c95-ed04-48b5-ad79-813752aba33b .

km-dev:TriplesMap_fcfa2c95-ed04-48b5-ad79-813752aba33b km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx19 rr:tableName "WAM_XMLExport_AAC_Constituents_V3.xml" ;
	a rr:LogicalTable ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasLogicalTable _:node1b3thi6ccx19 .

km-dev:TriplesMap_fcfa2c95-ed04-48b5-ad79-813752aba33b rr:logicalTable _:node1b3thi6ccx19 ;
	rr:subjectMap _:node1b3thi6ccx20 .

_:node1b3thi6ccx1 km-dev:hasSubjectMap _:node1b3thi6ccx20 .

_:node1b3thi6ccx20 km-dev:isPartOfMapping _:node1b3thi6ccx1 ;
	a rr:SubjectMap ;
	km-dev:alignmentNodeId "http://www.cidoc-crm.org/cidoc-crm/E55_Type1" ;
	rr:class crm:E55_Type ;
	rr:template "{[\"Root\",\"ObjRecord\",\"Constituents\",\"ObjectRelatedConstituent\",\"GenderURI\"]}" .

km-dev:PredicateObjectMap_21c3f780-e55b-4896-92e2-dcca9c7aad9e rr:predicate crm:P2_has_type .

km-dev:RefObjectMap_a9fddfd4-eea6-46fc-b3b6-8c6e1db72c57 a rr:RefObjectMap , rr:ObjectMap ;
	rr:parentTriplesMap km-dev:TriplesMap_a023606a-58a4-4127-bcab-aa6ac4034568 ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap km-dev:RefObjectMap_a9fddfd4-eea6-46fc-b3b6-8c6e1db72c57 .

km-dev:PredicateObjectMap_21c3f780-e55b-4896-92e2-dcca9c7aad9e rr:objectMap km-dev:RefObjectMap_a9fddfd4-eea6-46fc-b3b6-8c6e1db72c57 .

km-dev:TriplesMap_fcfa2c95-ed04-48b5-ad79-813752aba33b rr:predicateObjectMap km-dev:PredicateObjectMap_21c3f780-e55b-4896-92e2-dcca9c7aad9e .

km-dev:PredicateObjectMap_21c3f780-e55b-4896-92e2-dcca9c7aad9e a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_21c3f780-e55b-4896-92e2-dcca9c7aad9e .

km-dev:PredicateObjectMap_f6a5b972-561a-460a-a324-da5ec21b6275 rr:predicate rdfs:label .

_:node1b3thi6ccx21 rr:column "[\"Root\",\"ObjRecord\",\"Constituents\",\"ObjectRelatedConstituent\",\"Gender\"]" ;
	a rr:ObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap _:node1b3thi6ccx21 .

km-dev:PredicateObjectMap_f6a5b972-561a-460a-a324-da5ec21b6275 rr:objectMap _:node1b3thi6ccx21 .

km-dev:TriplesMap_fcfa2c95-ed04-48b5-ad79-813752aba33b rr:predicateObjectMap km-dev:PredicateObjectMap_f6a5b972-561a-460a-a324-da5ec21b6275 .

km-dev:PredicateObjectMap_f6a5b972-561a-460a-a324-da5ec21b6275 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_f6a5b972-561a-460a-a324-da5ec21b6275 .

km-dev:TriplesMap_78f38e81-b850-4868-a39c-08ed2117b2dd a rr:TriplesMap .

_:node1b3thi6ccx1 km-dev:hasTriplesMap km-dev:TriplesMap_78f38e81-b850-4868-a39c-08ed2117b2dd .

km-dev:TriplesMap_78f38e81-b850-4868-a39c-08ed2117b2dd km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx22 rr:tableName "WAM_XMLExport_AAC_Constituents_V3.xml" ;
	a rr:LogicalTable ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasLogicalTable _:node1b3thi6ccx22 .

km-dev:TriplesMap_78f38e81-b850-4868-a39c-08ed2117b2dd rr:logicalTable _:node1b3thi6ccx22 ;
	rr:subjectMap _:node1b3thi6ccx23 .

_:node1b3thi6ccx1 km-dev:hasSubjectMap _:node1b3thi6ccx23 .

_:node1b3thi6ccx23 km-dev:isPartOfMapping _:node1b3thi6ccx1 ;
	a rr:SubjectMap ;
	km-dev:alignmentNodeId "http://www.cidoc-crm.org/cidoc-crm/E63_Beginning_of_Existence1" ;
	rr:class crm:E63_Beginning_of_Existence ;
	rr:template "{[\"Root\",\"ObjRecord\",\"Constituents\",\"ObjectRelatedConstituent\",\"ConstituentGeography\",\"ConstituentGeography\",\"birthPlaceURI\"]}" .

km-dev:PredicateObjectMap_3aa131f0-c2a2-43d7-be1b-4f7132aa4d60 rr:predicate crm:P7_took_place_at .

km-dev:RefObjectMap_2c94e3af-b438-4700-8713-9154952fd75b a rr:RefObjectMap , rr:ObjectMap ;
	rr:parentTriplesMap km-dev:TriplesMap_be2fe597-79df-48ca-8ae9-2efedf480b0d ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap km-dev:RefObjectMap_2c94e3af-b438-4700-8713-9154952fd75b .

km-dev:PredicateObjectMap_3aa131f0-c2a2-43d7-be1b-4f7132aa4d60 rr:objectMap km-dev:RefObjectMap_2c94e3af-b438-4700-8713-9154952fd75b .

km-dev:TriplesMap_78f38e81-b850-4868-a39c-08ed2117b2dd rr:predicateObjectMap km-dev:PredicateObjectMap_3aa131f0-c2a2-43d7-be1b-4f7132aa4d60 .

km-dev:PredicateObjectMap_3aa131f0-c2a2-43d7-be1b-4f7132aa4d60 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_3aa131f0-c2a2-43d7-be1b-4f7132aa4d60 .

km-dev:TriplesMap_e223c382-0498-4dc9-a840-3ea21e0b1592 a rr:TriplesMap .

_:node1b3thi6ccx1 km-dev:hasTriplesMap km-dev:TriplesMap_e223c382-0498-4dc9-a840-3ea21e0b1592 .

km-dev:TriplesMap_e223c382-0498-4dc9-a840-3ea21e0b1592 km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx24 rr:tableName "WAM_XMLExport_AAC_Constituents_V3.xml" ;
	a rr:LogicalTable ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasLogicalTable _:node1b3thi6ccx24 .

km-dev:TriplesMap_e223c382-0498-4dc9-a840-3ea21e0b1592 rr:logicalTable _:node1b3thi6ccx24 ;
	rr:subjectMap _:node1b3thi6ccx25 .

_:node1b3thi6ccx1 km-dev:hasSubjectMap _:node1b3thi6ccx25 .

_:node1b3thi6ccx25 km-dev:isPartOfMapping _:node1b3thi6ccx1 ;
	a rr:SubjectMap ;
	km-dev:alignmentNodeId "http://www.cidoc-crm.org/cidoc-crm/E82_Actor_Appellation1" ;
	rr:class crm:E82_Actor_Appellation ;
	rr:template "{[\"Root\",\"ObjRecord\",\"Constituents\",\"ObjectRelatedConstituent\",\"ConstituentURI\"]}/appellation/" .

km-dev:PredicateObjectMap_fd778803-9c04-43a5-8715-7c7d0587d1c6 rr:predicate rdf:value .

_:node1b3thi6ccx26 rr:column "[\"Root\",\"ObjRecord\",\"Constituents\",\"ObjectRelatedConstituent\",\"DisplayName\"]" ;
	a rr:ObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap _:node1b3thi6ccx26 .

km-dev:PredicateObjectMap_fd778803-9c04-43a5-8715-7c7d0587d1c6 rr:objectMap _:node1b3thi6ccx26 .

km-dev:TriplesMap_e223c382-0498-4dc9-a840-3ea21e0b1592 rr:predicateObjectMap km-dev:PredicateObjectMap_fd778803-9c04-43a5-8715-7c7d0587d1c6 .

km-dev:PredicateObjectMap_fd778803-9c04-43a5-8715-7c7d0587d1c6 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_fd778803-9c04-43a5-8715-7c7d0587d1c6 .

km-dev:PredicateObjectMap_f14fbb1d-7100-4ded-aec0-5e273478ea9f rr:predicate crm:P2_has_type .

_:node1b3thi6ccx27 rr:constant <http://vocab.getty.edu/aat/300404670> ;
	a rr:ObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap _:node1b3thi6ccx27 .

km-dev:PredicateObjectMap_f14fbb1d-7100-4ded-aec0-5e273478ea9f rr:objectMap _:node1b3thi6ccx27 .

km-dev:TriplesMap_e223c382-0498-4dc9-a840-3ea21e0b1592 rr:predicateObjectMap km-dev:PredicateObjectMap_f14fbb1d-7100-4ded-aec0-5e273478ea9f .

km-dev:PredicateObjectMap_f14fbb1d-7100-4ded-aec0-5e273478ea9f a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_f14fbb1d-7100-4ded-aec0-5e273478ea9f .

km-dev:TriplesMap_be2fe597-79df-48ca-8ae9-2efedf480b0d a rr:TriplesMap .

_:node1b3thi6ccx1 km-dev:hasTriplesMap km-dev:TriplesMap_be2fe597-79df-48ca-8ae9-2efedf480b0d .

km-dev:TriplesMap_be2fe597-79df-48ca-8ae9-2efedf480b0d km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx28 rr:tableName "WAM_XMLExport_AAC_Constituents_V3.xml" ;
	a rr:LogicalTable ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasLogicalTable _:node1b3thi6ccx28 .

km-dev:TriplesMap_be2fe597-79df-48ca-8ae9-2efedf480b0d rr:logicalTable _:node1b3thi6ccx28 ;
	rr:subjectMap _:node1b3thi6ccx29 .

_:node1b3thi6ccx1 km-dev:hasSubjectMap _:node1b3thi6ccx29 .

_:node1b3thi6ccx29 km-dev:isPartOfMapping _:node1b3thi6ccx1 ;
	a rr:SubjectMap ;
	km-dev:alignmentNodeId "http://www.cidoc-crm.org/cidoc-crm/E53_Place1" ;
	rr:class crm:E53_Place ;
	rr:template "{[\"Root\",\"ObjRecord\",\"Constituents\",\"ObjectRelatedConstituent\",\"ConstituentGeography\",\"ConstituentGeography\",\"ConGeoTGNSourceTermID\"]}" .

km-dev:PredicateObjectMap_a737babf-12ce-4bd6-8693-ae6718a20263 rr:predicate crm:P48_has_preferred_identifier .

km-dev:RefObjectMap_23025a0b-312f-4c9c-b5f2-3c253036ebae a rr:RefObjectMap , rr:ObjectMap ;
	rr:parentTriplesMap km-dev:TriplesMap_d657294e-a1dc-441e-872f-3ae46d50dcec ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap km-dev:RefObjectMap_23025a0b-312f-4c9c-b5f2-3c253036ebae .

km-dev:PredicateObjectMap_a737babf-12ce-4bd6-8693-ae6718a20263 rr:objectMap km-dev:RefObjectMap_23025a0b-312f-4c9c-b5f2-3c253036ebae .

km-dev:TriplesMap_be2fe597-79df-48ca-8ae9-2efedf480b0d rr:predicateObjectMap km-dev:PredicateObjectMap_a737babf-12ce-4bd6-8693-ae6718a20263 .

km-dev:PredicateObjectMap_a737babf-12ce-4bd6-8693-ae6718a20263 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_a737babf-12ce-4bd6-8693-ae6718a20263 .

km-dev:PredicateObjectMap_d22eac78-f95a-4004-9d59-1f738d917bde rr:predicate crm:P1_is_identified_by .

km-dev:RefObjectMap_b1c81d09-9305-4313-851a-f06e8f204e7c a rr:RefObjectMap , rr:ObjectMap ;
	rr:parentTriplesMap km-dev:TriplesMap_a456e368-93c8-43fd-957f-1bbb685b7465 ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap km-dev:RefObjectMap_b1c81d09-9305-4313-851a-f06e8f204e7c .

km-dev:PredicateObjectMap_d22eac78-f95a-4004-9d59-1f738d917bde rr:objectMap km-dev:RefObjectMap_b1c81d09-9305-4313-851a-f06e8f204e7c .

km-dev:TriplesMap_be2fe597-79df-48ca-8ae9-2efedf480b0d rr:predicateObjectMap km-dev:PredicateObjectMap_d22eac78-f95a-4004-9d59-1f738d917bde .

km-dev:PredicateObjectMap_d22eac78-f95a-4004-9d59-1f738d917bde a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_d22eac78-f95a-4004-9d59-1f738d917bde .

km-dev:PredicateObjectMap_f4732cce-235f-40d3-9203-395e0fceeb06 rr:predicate crm:P1_is_identified_by .

km-dev:RefObjectMap_fd2993fc-1dca-485d-95ae-e924f0ee8b20 a rr:RefObjectMap , rr:ObjectMap ;
	rr:parentTriplesMap km-dev:TriplesMap_0a65ba30-cc2d-46b4-984b-1729f22a07b8 ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap km-dev:RefObjectMap_fd2993fc-1dca-485d-95ae-e924f0ee8b20 .

km-dev:PredicateObjectMap_f4732cce-235f-40d3-9203-395e0fceeb06 rr:objectMap km-dev:RefObjectMap_fd2993fc-1dca-485d-95ae-e924f0ee8b20 .

km-dev:TriplesMap_be2fe597-79df-48ca-8ae9-2efedf480b0d rr:predicateObjectMap km-dev:PredicateObjectMap_f4732cce-235f-40d3-9203-395e0fceeb06 .

km-dev:PredicateObjectMap_f4732cce-235f-40d3-9203-395e0fceeb06 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_f4732cce-235f-40d3-9203-395e0fceeb06 .

km-dev:PredicateObjectMap_db5687e2-a0a5-4f9c-bdcf-09104a710091 rr:predicate rdfs:label .

_:node1b3thi6ccx30 rr:column "[\"Root\",\"ObjRecord\",\"Constituents\",\"ObjectRelatedConstituent\",\"ConstituentGeography\",\"ConstituentGeography\",\"ThesGeographyTerm\"]" ;
	a rr:ObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap _:node1b3thi6ccx30 .

km-dev:PredicateObjectMap_db5687e2-a0a5-4f9c-bdcf-09104a710091 rr:objectMap _:node1b3thi6ccx30 .

km-dev:TriplesMap_be2fe597-79df-48ca-8ae9-2efedf480b0d rr:predicateObjectMap km-dev:PredicateObjectMap_db5687e2-a0a5-4f9c-bdcf-09104a710091 .

km-dev:PredicateObjectMap_db5687e2-a0a5-4f9c-bdcf-09104a710091 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_db5687e2-a0a5-4f9c-bdcf-09104a710091 .

km-dev:TriplesMap_d657294e-a1dc-441e-872f-3ae46d50dcec a rr:TriplesMap .

_:node1b3thi6ccx1 km-dev:hasTriplesMap km-dev:TriplesMap_d657294e-a1dc-441e-872f-3ae46d50dcec .

km-dev:TriplesMap_d657294e-a1dc-441e-872f-3ae46d50dcec km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx31 rr:tableName "WAM_XMLExport_AAC_Constituents_V3.xml" ;
	a rr:LogicalTable ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasLogicalTable _:node1b3thi6ccx31 .

km-dev:TriplesMap_d657294e-a1dc-441e-872f-3ae46d50dcec rr:logicalTable _:node1b3thi6ccx31 ;
	rr:subjectMap _:node1b3thi6ccx32 .

_:node1b3thi6ccx1 km-dev:hasSubjectMap _:node1b3thi6ccx32 .

_:node1b3thi6ccx32 km-dev:isPartOfMapping _:node1b3thi6ccx1 ;
	a rr:SubjectMap ;
	km-dev:alignmentNodeId "http://www.cidoc-crm.org/cidoc-crm/E42_Identifier2" ;
	rr:class crm:E42_Identifier ;
	rr:template "{[\"Root\",\"ObjRecord\",\"Constituents\",\"ObjectRelatedConstituent\",\"ConstituentGeography\",\"ConstituentGeography\",\"ConGeoTGNSourceTermID_URI\"]}" .

km-dev:PredicateObjectMap_62d8d81c-16f6-44bb-862b-f3fa58a567ce rr:predicate rdfs:label .

_:node1b3thi6ccx33 rr:column "[\"Root\",\"ObjRecord\",\"Constituents\",\"ObjectRelatedConstituent\",\"ConstituentGeography\",\"ConstituentGeography\",\"ConGeoTGNSourceTermID\"]" ;
	a rr:ObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap _:node1b3thi6ccx33 .

km-dev:PredicateObjectMap_62d8d81c-16f6-44bb-862b-f3fa58a567ce rr:objectMap _:node1b3thi6ccx33 .

km-dev:TriplesMap_d657294e-a1dc-441e-872f-3ae46d50dcec rr:predicateObjectMap km-dev:PredicateObjectMap_62d8d81c-16f6-44bb-862b-f3fa58a567ce .

km-dev:PredicateObjectMap_62d8d81c-16f6-44bb-862b-f3fa58a567ce a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_62d8d81c-16f6-44bb-862b-f3fa58a567ce .

km-dev:TriplesMap_a456e368-93c8-43fd-957f-1bbb685b7465 a rr:TriplesMap .

_:node1b3thi6ccx1 km-dev:hasTriplesMap km-dev:TriplesMap_a456e368-93c8-43fd-957f-1bbb685b7465 .

km-dev:TriplesMap_a456e368-93c8-43fd-957f-1bbb685b7465 km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx34 rr:tableName "WAM_XMLExport_AAC_Constituents_V3.xml" ;
	a rr:LogicalTable ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasLogicalTable _:node1b3thi6ccx34 .

km-dev:TriplesMap_a456e368-93c8-43fd-957f-1bbb685b7465 rr:logicalTable _:node1b3thi6ccx34 ;
	rr:subjectMap _:node1b3thi6ccx35 .

_:node1b3thi6ccx1 km-dev:hasSubjectMap _:node1b3thi6ccx35 .

_:node1b3thi6ccx35 km-dev:isPartOfMapping _:node1b3thi6ccx1 ;
	a rr:SubjectMap ;
	km-dev:alignmentNodeId "http://www.cidoc-crm.org/cidoc-crm/E47_Spatial_Coordinates1" ;
	rr:class crm:E47_Spatial_Coordinates ;
	rr:termType rr:BlankNode ;
	km-dev:namePrefix "crm:E47_Spatial_Coordinates1" .

km-dev:PredicateObjectMap_b1dae214-745b-4bd6-8db0-06452ae57879 rr:predicate rdfs:label .

_:node1b3thi6ccx36 rr:column "[\"Root\",\"ObjRecord\",\"Constituents\",\"ObjectRelatedConstituent\",\"ConstituentGeography\",\"ConstituentGeography\",\"SpatialCoOrdinates\"]" ;
	a rr:ObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap _:node1b3thi6ccx36 .

km-dev:PredicateObjectMap_b1dae214-745b-4bd6-8db0-06452ae57879 rr:objectMap _:node1b3thi6ccx36 .

km-dev:TriplesMap_a456e368-93c8-43fd-957f-1bbb685b7465 rr:predicateObjectMap km-dev:PredicateObjectMap_b1dae214-745b-4bd6-8db0-06452ae57879 .

km-dev:PredicateObjectMap_b1dae214-745b-4bd6-8db0-06452ae57879 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_b1dae214-745b-4bd6-8db0-06452ae57879 .

km-dev:TriplesMap_0a65ba30-cc2d-46b4-984b-1729f22a07b8 a rr:TriplesMap .

_:node1b3thi6ccx1 km-dev:hasTriplesMap km-dev:TriplesMap_0a65ba30-cc2d-46b4-984b-1729f22a07b8 .

km-dev:TriplesMap_0a65ba30-cc2d-46b4-984b-1729f22a07b8 km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx37 rr:tableName "WAM_XMLExport_AAC_Constituents_V3.xml" ;
	a rr:LogicalTable ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasLogicalTable _:node1b3thi6ccx37 .

km-dev:TriplesMap_0a65ba30-cc2d-46b4-984b-1729f22a07b8 rr:logicalTable _:node1b3thi6ccx37 ;
	rr:subjectMap _:node1b3thi6ccx38 .

_:node1b3thi6ccx1 km-dev:hasSubjectMap _:node1b3thi6ccx38 .

_:node1b3thi6ccx38 km-dev:isPartOfMapping _:node1b3thi6ccx1 ;
	a rr:SubjectMap ;
	km-dev:alignmentNodeId "http://www.cidoc-crm.org/cidoc-crm/E48_Place_Name1" ;
	rr:class crm:E48_Place_Name ;
	rr:termType rr:BlankNode ;
	km-dev:namePrefix "crm:E48_Place_Name1" .

km-dev:PredicateObjectMap_d355c7f7-cdbe-4742-a4de-557be2bdd471 rr:predicate rdfs:label .

_:node1b3thi6ccx39 rr:column "[\"Root\",\"ObjRecord\",\"Constituents\",\"ObjectRelatedConstituent\",\"ConstituentGeography\",\"ConstituentGeography\",\"ThesGeographyTerm\"]" ;
	a rr:ObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap _:node1b3thi6ccx39 .

km-dev:PredicateObjectMap_d355c7f7-cdbe-4742-a4de-557be2bdd471 rr:objectMap _:node1b3thi6ccx39 .

km-dev:TriplesMap_0a65ba30-cc2d-46b4-984b-1729f22a07b8 rr:predicateObjectMap km-dev:PredicateObjectMap_d355c7f7-cdbe-4742-a4de-557be2bdd471 .

km-dev:PredicateObjectMap_d355c7f7-cdbe-4742-a4de-557be2bdd471 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_d355c7f7-cdbe-4742-a4de-557be2bdd471 .

km-dev:TriplesMap_a023606a-58a4-4127-bcab-aa6ac4034568 a rr:TriplesMap .

_:node1b3thi6ccx1 km-dev:hasTriplesMap km-dev:TriplesMap_a023606a-58a4-4127-bcab-aa6ac4034568 .

km-dev:TriplesMap_a023606a-58a4-4127-bcab-aa6ac4034568 km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx40 rr:tableName "WAM_XMLExport_AAC_Constituents_V3.xml" ;
	a rr:LogicalTable ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasLogicalTable _:node1b3thi6ccx40 .

km-dev:TriplesMap_a023606a-58a4-4127-bcab-aa6ac4034568 rr:logicalTable _:node1b3thi6ccx40 ;
	rr:subjectMap _:node1b3thi6ccx41 .

_:node1b3thi6ccx1 km-dev:hasSubjectMap _:node1b3thi6ccx41 .

_:node1b3thi6ccx41 km-dev:isPartOfMapping _:node1b3thi6ccx1 ;
	a rr:SubjectMap ;
	km-dev:alignmentNodeId "http://www.cidoc-crm.org/cidoc-crm/E55_Type2" ;
	rr:class crm:E55_Type ;
	rr:termType rr:BlankNode ;
	km-dev:namePrefix "crm:E55_Type2" .

km-dev:PredicateObjectMap_174fbe03-cdac-4efa-a416-022c0c3efa47 rr:predicate skos:broadMatch .

_:node1b3thi6ccx42 rr:constant <http://vocab.getty.edu/aat/300055147> ;
	a rr:ObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasObjectMap _:node1b3thi6ccx42 .

km-dev:PredicateObjectMap_174fbe03-cdac-4efa-a416-022c0c3efa47 rr:objectMap _:node1b3thi6ccx42 .

km-dev:TriplesMap_a023606a-58a4-4127-bcab-aa6ac4034568 rr:predicateObjectMap km-dev:PredicateObjectMap_174fbe03-cdac-4efa-a416-022c0c3efa47 .

km-dev:PredicateObjectMap_174fbe03-cdac-4efa-a416-022c0c3efa47 a rr:PredicateObjectMap ;
	km-dev:isPartOfMapping _:node1b3thi6ccx1 .

_:node1b3thi6ccx1 km-dev:hasPredicateObjectMap km-dev:PredicateObjectMap_174fbe03-cdac-4efa-a416-022c0c3efa47 .

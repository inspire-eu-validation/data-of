# Conformance class: Information accessibility, Oceanographic geographical features

Conformance class for the requirements related to the accessibility of referenced information, for example, information stored in registries (code lists, coordinate reference systems).

To be able to test this conformance class, the encoding of the data set must be known, i.e. this is a parameterized conformance class. The XPath expressions used in this test suite assume that the GML encoding is used. If used with the GML encoding this conformance class has an indirect dependency to the conformance class "GML application schemas, Oceanographic geographical features".

This conformance class is part of the [INSPIRE Data Specification on Oceanographic geographical features](../README.md).

## Standardization target type

INSPIRE spatial data set

## Dependencies

### Direct dependencies

A direct dependency is another conformance class whose requirements must be met by the data set, too.

| Specification | Conformance class | Parameters | 
| ------------- | ----------------- | ---------- |
| [TG DS Template](#ref_TG_DS_tmpl) | [Information accessibility](http://inspire.ec.europa.eu/id/ats/data/3.0rc3/information-accessibility) | n/a |

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [TG DS_OF](#ref_TG_DS_OF) | [GML application schemas, Oceanographic geographical features](../of-gml/README.md) | INSPIRE spatial data set encoded in GML, Oceanographic geographical features features | n/a |
 
## Feature types <a name="feature-types"></a>

The instantiable feature types in the application schema are:

* PointObservation
* PointTimeSeriesObservation
* MultiPointObservation
* GridObservation
* GridSeriesObservation
* PointObservationCollection

*Note*: When "features" or "spatial objects" are mentioned in the test cases, this refers only to instances of feature types of this application schema, not to any types specified in any other application schema.

## External document references

The following abbreviations are used in the test text for referring to external documents:

Abbreviation                     | Document name
-------------------------------- | --------------------------------------------------
TG DS_OF <a name="ref_TG_DS_OF"></a>   | [INSPIRE Data Specification on Oceanographic geographical features – Technical Guidelines version 3.0](http://inspire.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_OF_v3.0.pdf)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS_OF](#ref_TG_DS_OF)  |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Code lists](./code-list.md)  | ready for review  | A.5.1 |

## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
gml            | http://www.opengis.net/gml/3.2
of        	   | http://inspire.ec.europa.eu/schemas/of/4.0
omso		   |  http://inspire.ec.europa.eu/schemas/omso/3.0
omor           |  http://inspire.ec.europa.eu/schemas/omor/3.0
om  		   |  http://www.opengis.net/om/2.0


The following variables are used to refer to the corresponding Xpath expressions in all test descriptions:

Variable       | Value
-------------- | -------------------------------------------------
$features      |  //schema-element(omso:PointObservation) \| //schema-element(omso:PointTimeSeriesObservation)) \| //schema-element(omso:MultiPointObservation) \|  //schema-element(omso:GridObservation) \| //schema-element(omso:GridSeriesObservation) \| //schema-element(omso:PointObservationCollection)
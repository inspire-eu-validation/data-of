# Conformance class: Application schema, Oceanographic geographical features

Conformance class for the requirements associated with the application schema. 

To be able to test this conformance class, the encoding of the data set must be known, i.e. this is a parameterized conformance class. The XPath expressions used in this test suite assume that the GML encoding is used. If used with the GML encoding this conformance class has an indirect dependency to the conformance class "GML application schemas, Oceanographic geographical features".

This conformance class is part of the [INSPIRE Data Specification on Oceanographic geographical features](../README.md).

## Standardization target type

INSPIRE spatial data set

## Dependencies

### Direct dependencies

none

### Indirect dependencies

An indirect dependency is another conformance class whose requirements must be met by a related resource.

| Specification | Conformance class | Related resource | Parameters |
| ------------- | ----------------- | ---------------- | ---------- |
| [TG DS-OF](./README.md#ref_TG_DS_OF) | [GML application schemas, Oceanographic geographical features](../of-gml/README.md) | INSPIRE spatial data set encoded in GML, Oceanographic geographical features features | n/a |
 
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
TG DS-OF <a name="ref_TG_DS_OF"></a>   | [INSPIRE Data Specification on Oceanographic geographical features – Technical Guidelines version 3.0](http://inspire.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_OF_v3.0.pdf)
TG DS-OF-corr <a name="ref_TG_DS_OF_corr"></a>   | [Corrigenda to the INSPIRE Data Specification on Oceanographic geographical features – Technical Guidelines version 3.0](https://inspire.ec.europa.eu/file/1621/download?token=-VHxltJ_)
TG DS Template <a name="ref_TG_DS_tmpl"></a>   | [INSPIRE Data Specification Template version 3.0rc3](http://inspire.jrc.ec.europa.eu/documents/Data_Specifications/INSPIRE_DataSpecification_Template_v3.0rc3.pdf)
IR-ISDSS <a name="ref_IR-ISDSS"></a>   | [Commission Regulation (EU) No 1089/2010 of 23 November 2010 implementing Directive 2007/2/EC of the European Parliament and of the Council as regards interoperability of spatial data sets and services](https://eur-lex.europa.eu/eli/reg/2010/1089/2014-12-31)

## Test Cases

| Identifier                                                        | Status   | Test case in [TG DS-OF](#ref_TG_DS_OF)  |
| ----------------------------------------------------------------- | -------- | ------------ |
| [Specific requirements](./specific-req.md)  | Draft  | A.1.8  |


## XML namespace prefixes <a name="namespaces"></a>

The following prefixes are used to refer to the corresponding XML namespaces in all test descriptions:

Prefix         | Namespace
-------------- | -------------------------------------------------
of             | http://inspire.ec.europa.eu/schemas/of/4.0
omso		   |  http://inspire.ec.europa.eu/schemas/omso/3.0
omor           |  http://inspire.ec.europa.eu/schemas/omor/3.0
om  		   |  http://www.opengis.net/om/2.0
base           | http://inspire.ec.europa.eu/schemas/base/3.3
gml            | http://www.opengis.net/gml/3.2
wfs            | http://www.opengis.net/wfs/2.0
xsi            | http://www.w3.org/2001/XMLSchema-instance
xlink          | http://www.w3.org/1999/xlink
xml            | http://www.w3.org/XML/1998/namespace

# Oceanographic geographical features theme-specific requirements

**Purpose**: Verify that the features provided in the dataset adhere to the theme-specific requirements specified in the INSPIRE application schema.

The following check is performed for every feature in the dataset:

* Check whether the data related to the theme Oceanographic Geographical Features are made available using the [following types](#allowedFT) defined in the Specialised Observations package in Annex I ([IR-ISDSS](./README.md#ref_IR-ISDSS)): PointObservation, PointTimeSeriesObservation, MultiPointObservation, GridObservation, GridSeriesObservation, PointObservationCollection.

The following checks shall be performed manually for all features in the dataset:

* By way of derogation from the requirements of Section 2.2. of Annex II ([IR-ISDSS](./README.md#ref_IR-ISDSS)), gridded data related to the theme Oceanographic Geographical Features may be made available using any appropriate grid.

* Check that the [observed property](#observedProperty) of an OM_Observation is identified by an identifier from the [BODC P01 Parameter Usage](http://inspire.ec.europa.eu/codelist/BODC_P01ParameterUsageValue) or [Climate and Forecast Standard Names](http://inspire.ec.europa.eu/codelist/CFStandardNamesValue) vocabularies.


**Prerequisites**

**Test method**

Verify that the theme-specific requirements that are specified in the UML model of the application schema are met, i.e. validate features against the theme-specific requirements. For unmet theme-specific requirements report [constraintViolation](#constraintViolation).


**Reference(s)**: 

* [TG DS_OF](./README.md#ref_TG_DS_OF) Annex A - Part 1 - A.1.8; A.2.3; A.3.6
* [IR-ISDSS](./README.md#ref_IR-ISDSS) Annex IV, Section 14.3

**Test type**: Automatic + Manual

**Notes** 


## Messages

Identifier  |  Message text (parameters start with '$')
---------------------------------------------------------- | -------------------------------------------------------------------------
constraintViolation <a name="constraintViolation"/>  |  XML document '$filename', $featureType '$gmlid': The constraint '$constraint' is violated.


## Contextual XPath references

The namespace prefixes used as described in [README](./README.md#namespaces).

Abbreviation                   |  XPath expression                 |Multiplicity       |Voidable
------------------------------ | --------------------------------- | ------------------|----------
Allowed feature types <a name="allowedFT"></a> | //schema-element(omso:PointObservation) \| //schema-element(omso:PointTimeSeriesObservation)) \| //schema-element(omso:MultiPointObservation) \|  //schema-element(omso:GridObservation) \| //schema-element(omso:GridSeriesObservation) \| //schema-element(omso:PointObservationCollection) | Not applicable | Not applicable
Observed Property <a name="observedProperty"></a> | //schema-element(omso:PointObservation)/om:observedProperty/@xlink:href <br> //schema-element(omso:PointTimeSeriesObservation)/om:observedProperty/@xlink:href <br> //schema-element(omso:MultiPointObservation)/om:observedProperty/@xlink:href <br> //schema-element(omso:GridObservation)/om:observedProperty/@xlink:href <br> //schema-element(omso:GridSeriesObservation)/om:observedProperty/@xlink:href <br> //schema-element(omso:PointObservationCollection)/omor:member/omso:PointObservation/om:observedProperty/@xlink:href  | 1 | Yes
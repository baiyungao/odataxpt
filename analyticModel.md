# Analytic Model Schema #

## Summary ##

oDataXpt provides an innovative and creative schema to model data analytic process. Its unique modeling philosophy is very intuitive to domain expert.

an analytic model starts from collections, fields. which are similar to tables and columns in relation database term.

Next step is to define an indicator. An [indicator](indicator.md) is an element to tell Model engine how to access data fields from repository, it provides a projection to the data repository.

A [measurement](measurement.md)  contains a list of indicator, it defines how to retrieve and aggregate data from repository.

A  [Series](series.md) represents a list of measurements by a giving time scale. a series may have multiple children series. oDataXpt predefined 3 types of series, [Fiscal Year](fiscalYear.md), [Quarter](quarter.md) and [Month](month.md), a Fiscal Year contains 12 Month series and 4 Quauter series. a series can contains one or more measurements, each measurement return 2 types of results, one is result between its own start time and end time, another is from its parent start time and its own end time, such as **Year to Month** value, **Year to Quarter** value and **Year to Day** value etc.





## Details ##

  * Field Metadata
  * [Indicator](indicator.md)
  * [measurement](measurement.md)
  * [Series](series.md)
    * [Fiscal Year](fiscalYear.md)
    * [Quarter](quarter.md)
    * [Month](month.md)
  * [Model](model.md)
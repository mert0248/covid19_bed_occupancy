

## App

To start the app, start R in the `app/` folder and type:

```r
shiny::runApp("app.R")
```




## Model

This folder contains a
[reportfactory](https://github.com/reconhub/reportfactory) with reports
providing a proof of concept and implementation of the model used for
forecasting admissions and hospital beds.


### Initial setup

You will first need to install dependencies before compiling the documents in
this factory. We recommend using the latest version of R. Double-click on
`open.Rproj` (or just start R in the `model/` folder) and copy-paste the
following instructions:

```r

if (!require(reportfactory)) remotes::install_github("reconhub/reportfactory")

library(reportfactory)
rfh_load_scripts()
install_deps()

```



### Compiling the report

 To compile the report, double-click on `open.Rproj` (or just start R
in the `model/` folder) and type:

```r

reportfactory::update_reports(clean_report_sources = TRUE)

```

Dated and time-stamped outputs will be generated in `report_outputs`.
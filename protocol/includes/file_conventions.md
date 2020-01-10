#### General Notes

It is important that you comply precisely with the formatting specified below, in order to facilitate the analysis of your simulation results in the ISIMIP framework. Incorrect formatting can
seriously delay the analysis. The ISIMIP Team will be glad to assist with the preparation of these files if necessary.

For questions or clarifications, please contact info@isimip.org or the data manager directly (buechner@pik‐potsdam.de) before submitting files.

#### Time slices for individual files

For time slices holding global daily data, files should cover 10 years starting in the second year of a decade and end in the first year of the next decade (e.g. 1991-2000). If the time period starts after the second year of the decade, or ends before the first year of the new decade, the start or end year of the time period should be used as the start or end year of the file respectively. Data on a lower than daily temporal resolution or non-global data should be submitted for the entire simulation period in single files per variable.

*Examples of time slices for individual files with global daily data:*

Pre-industrial: 1661_1670, 1671_1680, ..., 1851_1860
Historical: 1861_1870, 1871_1880, ..., 2001_2005
Future: 2006_2010, 2011_2020, ..., 2081_2090, 2091_2099
Extended future: 2100_2100, 2101_2110, ..., 2281_2290, 2291_2299

*Time slices for individual files with non-global or non-daily data:*

Pre-industrial: 1661_1860
Historical: 1861_2005
Future: 2006_2099
Extended future: 2100_2299

#### File names

File names consist of a series of identifiers, separated by underscores; see examples below. Things to note:

* Report one variable per file
* In filenames, use lowercase letters only
* Use underscore ("_") to separate identifiers
* Variable names consist of a single word without hyphens or underscores
* Use hyphens (”-“) to separate strings within an identifier, e.g. in a model name
* NetCDF file extension is .nc4

The file name format is:

```
<modelname>_<climate-forcing>_<bias-correction>_<climate-scenario>_<soc‐scenario>_<co2sens‐scenarios>_<variable>_<region>_<timestep>_<start‐year>_<end‐year>.nc4
```

##### modelname



##### bias_correction

{{ definition(sector, 'bias_correction') }}

##### climate_scenario

{{ definition(sector, 'climate_scenario') }}

##### soc_scenario

{{ definition(sector, 'soc_scenario') }}

##### co2sens_scenario

{{ definition(sector, 'co2sens_scenario') }}

Note: even models in which CO2 has no effect should use the co2 identifier relevant to the
experiment.

##### variable

The variables are described in detail in the table above.

##### region

Region, basin or site names. Where simulations are provided for a single
station within a river basin, the tag should have the format [basin]-[station].

##### timestep

{{ definition(sector, 'timestep') }}

##### start‐year/end‐year

Files should be uploaded in 10-year pieces. For the transition from the historical to the future
period (2005-2006), files should be separated, i.e. the identifiers would be 2001_2005 and
2006_2010.

For the forest simulations, no time slices are needed and the full simulation period can be
covered in one file.

For further instructions on file naming and formatting, please also refer to our website:

<https://www.isimip.org/protocol/isimip2b-files/#file-formats-and-meta-data>
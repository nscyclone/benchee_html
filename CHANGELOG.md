## 0.5.0 (2018-02-11)

### Features

* y-axis doesn't always start at 0 anymore for raw run times so that the space can be used
* note benchee & html versions down in the footer
* option to inline all assets `inline_assets`
* Support for benche `0.12`'s tags and names that are now displayed correctly

### Bugfixes

* Through a change in `benchee_json` formatter generation won't fail any longer if you're using `poison` < 3

## 0.4.0 (2017-10-24)

### Features

* Benchee 0.10.0 compatibility
* uses the `unit_scaling` option from benchee and scales units accordingly
* automatically open the report in a web browser after creation is finished
* update plotly.js version
* hide the save and edit in cloud link from plotly graphs
* use a default file name so you don't HAVE to supply a file name
* New "System info" link at the top right to display system information like OS, CPU, RAM etc.
* You can now specify the formatter as just `Benchee.Formatters.HTML`

## 0.3.1 (2017-05-07)

### Bugfixes

* use new benchee_json release to circumvent faulty typespec

## 0.3.0 (2017-05-07)

Benchee 0.8.0 compatibility, typesepcs, just Elixir 1.3+ and add missing applications.

## 0.2.0 (2017-04-23)

This release splits up the resulting HTML into multiple files, so that it isn't just one long HTML file and also for performance as drawing the graphs with lots of data points seems to be quite taxing on the browser.

### Features

* Instead of one huge HTML multiple files are generated:
  * An index page
  * a job comparison page per input
  * a detail view page per job per input

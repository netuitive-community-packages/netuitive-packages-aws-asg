## Release History

### Version next

* Fix an attribute computed metric with the wrong syntax

### Version 1.6.0

* Convert computed metrics to new format
* Adjusted build to use metricly-cli for validation
* Added percent unit to highest cpu utilization widget

### Version 1.5.1

* Fix for network metrics match expression

### Version 1.5.0

* Update to AWS ASG Summary dashboard
* Improved Element Details dashboard

### Version 1.4.0

* Updated gridstack dashboard layouts

### Version 1.3.7

* Updated package compatibilities.

### Version 1.3.6

* Bug fix for the multi-metric widgets on the element detail page.

### Version 1.3.5

* Fixed bugs: elevated activity policies for disk and network were looking for any deviations, rather than upper deviations.

### Version 1.3.4

* Fixed bug with the Events widget on the Element Detail Page.

### Version 1.3.3

* Added a new computed metric for total instance count. This is currently available as an attribute, but making it a metric allows us to graph it over time. Customers with detailed monitoring enabled will already get this information in a collected metric (aws.autoscaling.grouptotalinstances), so this is primarily to benefit those customers without detailed monitoring.

### Version 1.3.2

* Re-enabled the ASG Summary dashboard and ASG-specific element detail summary page.

### Version 1.3.1

* Temporarily remove ASG Summary dashboard and ASG-specific element detail summary page. These were built to reference the metric names in the new AWS ingest code, which are different from the ones in the old code. The new code is not quite ready for production.

### Version 1.3.0

* Added ASG Summary dashboard.
* Updated computed metrics to work with the new metric names from the ASG collector.
* Updated policies to work with the new computed metrics.
* Improved the "AWS ASG - Elevated CPU Activity (Normal Network Activity)" policy; it will no longer fire if the CPU value is less than 20%.

### Version 1.2.0

* Added ASG-specific element detail page.
* Fixed policy that wasn't being enabled by default.

### Version 1.1.0

* Added units to metrics.

### Version 1.0.1

* Removed reference to obsolete metric.
* Fixed policy names.
* Fixed CPU policy to look for upper deviations in CPU, rather than any deviation.

### Version 1.0.0

* Initial production release of the package for monitoring AWS Auto Scaling Group (ASG) resources.

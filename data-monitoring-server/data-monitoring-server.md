### Data monitoring server

## Functional requirement
1. Count - monotonically increasing accumulator
2. Histogram - count of items over bucket
3. Gauge - numerical measure that can go up and down
4. Summary - calculate values over time window, such as count or rates
5. System metrics


## Non functional requirement
1. Near real time data
2. High availablity
3. Low latency
4. Highly scalable


## Services
1. Data retreival service
2. Data Storage service
3. Data query service
4. Alert manager

## Time series database
1. Sliding window - moves through table, one row at a time
2. Tumbling window - move entire window to next non overlaping window


# Design
![Image](https://github.com/impradeeparya/system-design-hld/blob/main/data-monitoring-server/data-monitoring-server.png)

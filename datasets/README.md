## Datasets for experiment

The naming convention of the dataset files is: ```srv-<serviceid>-<time series>-<granularity>.csv```

Time series included are:

* **art** - application response time (both avg and p99)
* **ntt** - network transport time
* **tc** - transaction count
* **ts** - transaction size
* **usr** -number of concurrent users

Information contained in the datasets:

* **art** - response time is measured in ms
    * **id** - id number
    * **timestamp** - timestamp of the start of the aggregation window
    * **min** - minimum of the observed response time values in the given aggregation window
    * **max** - maximum of the observed response time values in the given aggregation window
    * **avg** - average of the observed response time values in the given aggregation window
    * **p50** - value of the 50-th percentile of response time values in the given aggregation window
    * **p95** - value of the 95-th percentile of response time values in the given aggregation window
    * **p99** - value of the 99-th percentile of response time values in the given aggregation window
    * **sum** - sum of all values of response time values in the given aggregation window
* **ntt** - network transaction time is measured in ms
    * **id** - id number
    * **timestamp** - timestamp of the start of the aggregation window
    * **min** - minimum of the observed network transport time values in the given aggregation window
    * **max** - maximum of the observed network transport time values in the given aggregation window
    * **avg** - average of the observed network transport time values in the given aggregation window
    * **sum** - sum of all values of response time values in the given aggregation window
    * **cnt** - count of all transactions in a given aggregation window
* **tc**
    * **id** - id number
    * **timestamp** - timestamp of the start of the aggregation window
    * **cnt** - count of all transactions in a given aggregation window
    * **l1-l4** - number of transaction in cagetories of SLA (1: <SLA, 2: <2SLA, 3: < 3SLA, 4: >3SLA)
    * **APMI** - values of internal application performance index
* **ts** - transaction size is measured in bytes
    * **id** - id number
    * **timestamp** - timestamp of the start of the aggregation window
    * **min** - minimum of the observed transaction size values in the given aggregation window
    * **max** - maximum of the observed transaction size values in the given aggregation window
    * **avg** - average of the observed transaction size values in the given aggregation window
    * **sum** - sum of all values of response time values in the given aggregation window
    * **cnt** - count of all transactions in a given aggregation window
* **usr**
    * **id** - id number
    * **timestamp** - timestamp of the start of the aggregation window
    * **cnt** - count of concurrent users in the given aggregation window

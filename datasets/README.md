## Datasets for Experiment

### Measurement Setup

The technology behind data collection and exact meaning of the individual variables are nicely described in [blog post by Jay Botelho](https://www.lovemytool.com/blog/2012/02/measuring-and-reporting-application-response-time-art-by-jay-botelho.html).

The data were measured using [Flowmon Application Performance Monitor](https://www.flowmon.com/en/products/flowmon/application-performance-monitor).

We collected QoS attributes for two public web services. The first monitored service (SERV-1) is a portal for electronic information resources available at our university. This portal serves as a search engine for licensed resources for science, research, and teaching provided for our students. The second monitored service (SERV-2) is a web presentation of the Faculty of Science. While the first service is dynamic and interactive, the second one represents a static web presentation. 

Both services were monitored over a month period from **June 16th to July 15th, 2018**.

### Dataset Metadata

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

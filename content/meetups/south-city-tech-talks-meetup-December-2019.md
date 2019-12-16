---
id: 3
title: "South City Tech Talks Meetup December 2019"
date: 2019-11-25T10:56:52+05:30
draft: false
type: "meetup"
---

Agenda and material for our December 2019 session #{{< param id >}}

Happy to announce we are having another South City Tech Talks Meetup. This meetup is focussed on cloud native technologies like storage, containers, orchestrators etc.

<!--more-->

## Agenda

* Talks on cloud native technologies by participants
* Discuss use-cases
* Have fun! :)

### Time and Venue

|           |                             |
| --------- | --------------------------- |
| **Time**  | 14 December 2019, 3pm - 5pm |
| **Venue** | B7 204                      |

## Proposed Talks

| Talk                                       | Proposed By |
| ------------------------------------------ | ----------- |
| Google Big Query: Practical Use-cases      | Jitendra    |
| Getting Started with Docker and Kubernetes | Smriti      |

## Take Aways

### Docker and Kubernetes 101

{{< youtube 4ht22ReBjno >}}

#### Learn by Doing

* Getting started with Docker: Hands-on interactive learning
  * https://www.katacoda.com/courses/docker
* Getting started with Kubernetes: Hands-on interactive learning
  * https://www.katacoda.com/courses/kubernetes
* What is a container?
  * https://www.docker.com/resources/what-container
* What is container orchestration?
  * https://kubernetes.io/docs/concepts/overview/what-is-kubernetes/

### Google BigQuery

#### Quick Intro to Big Query

[https://cloud.google.com/bigquery/what-is-bigquery](https://cloud.google.com/bigquery/what-is-bigquery)

#### Technical Architecture of Big Query

[https://panoply.io/data-warehouse-guide/bigquery-architecture/](https://panoply.io/data-warehouse-guide/bigquery-architecture/)

#### Getting Started Guides

[https://cloud.google.com/bigquery/docs/quickstarts](https://cloud.google.com/bigquery/docs/quickstarts)

#### Commands

```
# Create a dataset
bq mk meetup
	
#Load data into the table with auto schema detection
bq load --schema_update_option ALLOW_FIELD_ADDITION --autodetect --source_format NEWLINE_DELIMITED_JSON --max_bad_records=1000000 meetup.awesome gs://mybucket/2019-12-05/data/*

# List tables of the dataset
bq ls --format=pretty meetup

#Show details of awesome table
bq show --format=pretty meetup.awesome

#Export the schema
bq show --schema --format=prettyjson meetup.awesome > bq.json

# If required, edit bq.json 

# Run a query on the table
bq query --nouse_legacy_sql 'select * from meetup.awesome limit 10'

# Delete the table
bq rm meetup.awesome

# Recreate the table with the schema and partitioning
bq mk -t --expiration 2592000 --schema bq.json --range_partitioning timestamp,0,2524608000000,86400000 --clustering_fields timestamp,service --description "This is exposed data tabke"  meetup.awesome
```
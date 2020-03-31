---
id: 4
title: "SC Tech Talk — Jan' 20"
date: 2020-01-03T09:17:07+05:30
draft: false
type: "meetup"
---

Agenda and material for our January 2020 session #{{< param id >}}

Happy to announce we are having another South City Tech Talks Meetup.

<!--more-->

## Agenda

* Talks on two topics by participants
* Discuss use-cases
* Have fun! :)

### Time and Venue

|           |                             |
| --------- | --------------------------- |
| **Time**  | January 25, 2020, 3pm - 5pm |
| **Venue** | B7 204                      |

## Proposed Talks

| Talk                                         | Proposed By |
| -------------------------------------------- | ----------- |
| Industrial automation with Computer Vision   | Anshul      |
| Hands-on Google Big Table and it's use-cases | Jitendra    |

## Take Aways

### Hands on Google Big Table and its use-cases

#### What is Big Tables?

Bigtable is a distributed storage system for managing structured data that is designed to scale to a very large size: petabytes of data across thousands of commodity servers. Many projects at Google store data in Bigtable, including web indexing, Google Earth, and Google Finance. 

##### Quick Start

* Account on Google Cloud Computing Platform
* Tutorials: https://codelabs.developers.google.com/codelabs/cloud-bigtable-intro-java/index.html
* Download Big Table Simulator / Setup Hbase database
* https://cloud.google.com/bigtable/docs/emulator
* Few Commands to Play with Big Table Simulator

```
gcloud beta emulators bigtable start --host-port=127.0.0.1:8622 &
$(gcloud beta emulators bigtable env-init)
Now use cbt to connect to the simulator
```

Quick Start with cbt command line tool
https://cloud.google.com/bigtable/docs/quickstart-cbt

Configure ~/.cbtrc

```
cbt. Commands 
 cbt createtable tech_talk
 cbt ls
 cbt ls tech_talk
 cbt createfamily tech_talk ad
 cbt ls tech_talk
 cbt set tech_talk "1#day1#talk1" ad:ak="Industrial Automation" ad:jc="Big Tables"
 cbt ls tech_talk ad
 cbt read tech_talk
 cbt read tech_talk prefix=1#da
 cbt set tech_talk "1#month#talk1" ad:ak="Industrial Automation" ad:jc="Big Tables"
 cbt read tech_talk prefix=1#da
 cbt read tech_talk prefix=1#
 cbt read tech_talk prefix=1# count=1
```

#### Architecture

https://cloud.google.com/bigtable/docs/overview
https://static.googleusercontent.com/media/research.google.com/en//archive/bigtable-osdi06.pdf

### Industrial automation with Computer Vision

| Resource                                                      | Description                                                                                                                         |
| ------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- |
| https://course.fast.ai/                                       | A good course to get started on artificial intelligence and deep learning                                                           |
| http://pyimagesearch.com/                                     | This website has a lot of useful tutorials and sample code to get started with image processing, computer vision, and deep learning |
| https://github.com/ChristosChristofidis/awesome-deep-learning | A curated list of awesome deep learning resources                                                                                   |
| https://opencv.org/about/                                     | Open CV: A library for building computer vision applications                                                                        |

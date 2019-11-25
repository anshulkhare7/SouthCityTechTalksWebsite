---
id: 2
title: "South City Tech Talks Special Session: All Day DevOps 2019 Viewing"
date: 2019-11-21T14:37:04+05:30
draft: false
type: "meetup"
---

Agenda and material for our special session #{{< param id >}}

Happy to announce we are having another South City Tech Talks Meetup. This time instead of us talking, we will watch folks from AllDayDevOps talk.

<!--more-->

## Agenda

* Get together and watch curated talks from [All Day DevOps 2019](https://www.alldaydevops.com/2019-live-schedule)
* Discuss use-cases around talks
* Have fun! :)

### Time and Venue

|           |                                     |
| --------- | ----------------------------------- |
| **Time**  | 23rd November 2019, 2:30pm - 4:30pm |
| **Venue** | B7 204                              |

## Shortlisted Talks

| Talk                                                                                | Video URL                                      |
| ----------------------------------------------------------------------------------- | ---------------------------------------------- |
| How to Run Smarter in Production: Getting Started with Site Reliability Engineering | [YouTube](https://youtu.be/ike3vQbE4zc?t=1798) |
| What You See Is What You Get For AWS Infrastructure                                 | [YouTube](https://youtu.be/xtNx1t6lxQE?t=3678) |
| ZeroTrustOps: Securing at Scale                                                     | [YouTube](https://youtu.be/6GO9h1VsXc4?t=68)   |
| GitOps FTW                                                                          | [YouTube](https://youtu.be/EXMND7WCiLc?t=3853) |

> Open for change during the actual viewing :)

Some more interesting talks:

| Talks                                | Video URL                                      |
| ------------------------------------ | ---------------------------------------------- |
| Modern Solution Delivery: IT As Code | [YouTube](https://youtu.be/6GO9h1VsXc4?t=5615) |

## Minutes from Discussion

### Infrastructure as Code

* Use software development workflow to manage cloud infra 
* Saw demo of
  * Design a network using visual tools in `Cloudcraft`
  * Generate `Terragrunt` code
  * Create infra in AWS by running `Terragrunt` code
* Discussed on Infrastructure as Code (IaC) and its use-cases using tools like
  * [Cloudcraft for AWS](https://cloudcraft.co/)
  * [Terraform](https://www.terraform.io/)
  * [Terragrunt](https://github.com/gruntwork-io/terragrunt)

> Terragrunt is a DRY wrapper over Terraform

### Site Reliability Engineering

* Watched a talk on Site Reliability Engineering
  * SRE Teams are special teams responsible for customer happiness
  * SRE Teams should be engaged only for mission critical apps
  * SRE Teams define `Service Level Objectives` (SLO) and build/manage tech to meet them
  * SRE Teams acts as a bridge between `Business Requirements` and `DevOps`
* Free resource on SRE - [Google Site Reliability Engineering](https://landing.google.com/sre/books/)

### ZeroTrustOps

* The idea of `ZeroTrust` is to ensure there is no difference of trust inside or outside perimeter
* The idea of trusting internal network has led to massive breaches
* Every request should be authenticated & authorized irrespective of where they originates
* Refer to [Google's Beyond Corp](https://cloud.google.com/beyondcorp/) as an example of `ZeroTrust` security model
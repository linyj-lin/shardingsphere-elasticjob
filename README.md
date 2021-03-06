# [ElasticJob - distributed scheduled job solution](http://shardingsphere.apache.org/elasticjob/)

**Official website: https://shardingsphere.apache.org/elasticjob/**

[![Stargazers over time](https://starchart.cc/apache/shardingsphere-elasticjob-lite.svg)](https://starchart.cc/apache/shardingsphere-elasticjob-lite)

ElasticJob is a distributed scheduling solution consisting of two separate projects, Lite and Cloud.

ElasticJob Lite is a lightweight, decentralized solution that provides distributed task sharding services;
ElasticJob Cloud is a Mesos framework which use Mesos + Docker(todo) to manage and isolate resources and processes.

Elasticjob uses a unified job API for each product. 
Developers only need code one time and can deploy at will.

ElasticJob became an [Apache ShardingSphere](https://shardingsphere.apache.org/) Sub-project on May 28 2020.

Welcome communicate with community via [mail list](mailto:dev@shardingsphere.apache.org).

[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)

[![GitHub release](https://img.shields.io/github/release/apache/shardingsphere-elasticjob-lite.svg)](https://github.com/apache/shardingsphere-elasticjob-lite/releases)

[![Maven Status](https://maven-badges.herokuapp.com/maven-central/com.dangdang/elastic-job/badge.svg)](https://maven-badges.herokuapp.com/maven-central/com.dangdang/elastic-job)
[![Build Status](https://secure.travis-ci.org/apache/shardingsphere-elasticjob-lite.png?branch=master)](https://travis-ci.org/apache/shardingsphere-elasticjob-lite)
[![Coverage Status](https://coveralls.io/repos/elasticjob/elastic-job/badge.svg?branch=master&service=github)](https://coveralls.io/github/elasticjob/elastic-job?branch=master)

## Architecture

### ElasticJob Lite

![ElasticJob Lite Architecture](https://shardingsphere.apache.org/elasticjob/current/img/architecture/elasticjob_lite.png)

### ElasticJob Cloud

![ElasticJob Lite Architecture](https://shardingsphere.apache.org/elasticjob/current/img/architecture/elasticjob_cloud.png)

## Features

- Elastic Schedule
  - Support job sharding and high availability in distributed system
  - Scale out for throughput and efficiency improvement
  - Job processing capacity is flexible and scalable with the allocation of resources

- Resource Assign
  - Execute job on suitable time and assigned resources
  - Aggregation same job to same job executor
  - Append resources to newly assigned jobs dynamically

- Job Governance
  - Failover
  - Misfired
  - Self diagnose and recover when distribute environment unstable

- Job Dependency (TODO)
  - DAG based job dependency
  - DAG based job item dependency

- Job Open Ecosystem
  - Unify job api for extension
  - Support rich job type lib, such as dataflow, script, HTTP, file, big data
  - Focus business SDK, can work with Spring IOC

- Admin Console
  - Job administration
  - Job event trace query
  - Registry center management

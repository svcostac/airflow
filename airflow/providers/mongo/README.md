<!--
 Licensed to the Apache Software Foundation (ASF) under one
 or more contributor license agreements.  See the NOTICE file
 distributed with this work for additional information
 regarding copyright ownership.  The ASF licenses this file
 to you under the Apache License, Version 2.0 (the
 "License"); you may not use this file except in compliance
 with the License.  You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing,
 software distributed under the License is distributed on an
 "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied.  See the License for the
 specific language governing permissions and limitations
 under the License.
 -->


# Package apache-airflow-backport-providers-mongo

Release: 2020.05.19

**Table of contents**

- [Backport package](#backport-package)
- [Installation](#installation)
- [Compatibility](#compatibility)
- [PIP requirements](#pip-requirements)
- [Provider class summary](#provider-class-summary)
    - [Sensors](#sensors)
        - [Moved sensors](#moved-sensors)
    - [Hooks](#hooks)
        - [Moved hooks](#moved-hooks)
- [Releases](#releases)
    - [Release 2020.05.19](#release-20200519)

## Backport package

This is a backport providers package for `mongo` provider. All classes for this provider package
are in `airflow.providers.mongo` python package.

## Installation

You can install this package on top of an existing airflow 1.10.* installation via
`pip install apache-airflow-backport-providers-mongo`

## Compatibility

For full compatibility and test status of the backport packages check
[Airflow Backport Package Compatibility](https://cwiki.apache.org/confluence/display/AIRFLOW/Backported+providers+packages+for+Airflow+1.10.*+series)

## PIP requirements

| PIP package   | Version required   |
|:--------------|:-------------------|
| dnspython     | &gt;=1.13.0,&lt;2.0.0    |
| pymongo       | &gt;=3.6.0            |

# Provider class summary

All classes in Airflow 2.0 are in `airflow.providers.mongo` package.




## Sensors



### Moved sensors

| Airflow 2.0 sensors: `airflow.providers.mongo` package                                                              | Airflow 1.10.* previous location (usually `airflow.contrib`)                                                                            |
|:--------------------------------------------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------|
| [sensors.mongo.MongoSensor](https://github.com/apache/airflow/blob/master/airflow/providers/mongo/sensors/mongo.py) | [contrib.sensors.mongo_sensor.MongoSensor](https://github.com/apache/airflow/blob/v1-10-stable/airflow/contrib/sensors/mongo_sensor.py) |



## Hooks



### Moved hooks

| Airflow 2.0 hooks: `airflow.providers.mongo` package                                                          | Airflow 1.10.* previous location (usually `airflow.contrib`)                                                                  |
|:--------------------------------------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| [hooks.mongo.MongoHook](https://github.com/apache/airflow/blob/master/airflow/providers/mongo/hooks/mongo.py) | [contrib.hooks.mongo_hook.MongoHook](https://github.com/apache/airflow/blob/v1-10-stable/airflow/contrib/hooks/mongo_hook.py) |






## Releases

### Release 2020.05.19

| Commit                                                                                         | Committed   | Subject                                                           |
|:-----------------------------------------------------------------------------------------------|:------------|:------------------------------------------------------------------|
| [05443c6dc](https://github.com/apache/airflow/commit/05443c6dc8100e791446bbcc0df04de6e34017bb) | 2020-03-23  | Add missing call to Super class in remaining providers (#7828)    |
| [97a429f9d](https://github.com/apache/airflow/commit/97a429f9d0cf740c5698060ad55f11e93cb57b55) | 2020-02-02  | [AIRFLOW-6714] Remove magic comments about UTF-8 (#7338)          |
| [059eda05f](https://github.com/apache/airflow/commit/059eda05f82fefce4410f44f761f945a27d83daf) | 2020-01-21  | [AIRFLOW-6610] Move software classes to providers package (#7231) |

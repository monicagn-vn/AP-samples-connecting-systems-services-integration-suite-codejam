# Connecting systems and services using SAP Integration Suite
<!--- Register repository https://api.reuse.software/register, then add REUSE badge:
[![REUSE status](https://api.reuse.software/badge/github.com/SAP-samples/REPO-NAME)](https://api.reuse.software/info/github.com/SAP-samples/REPO-NAME)
-->

⚠️ This is a work-in-progress.

In this SAP CodeJam we will look at different services, part of the SAP Integration Suite, and how we can use them to connect our systems and services.

## Integration Scenario

Let's imagine we work for a company, ITeLO. ITeLO uses an external platform to manage its Employee Benefits, through which its employees can select their benefits, e.g. discount gym membership, private health insurance, and dental. In addition, ITeLO is interested in expanding its adoption of the benefits platform to allow employees to include their dependants, e.g. spouse, child or other family members, as beneficiaries of the different offerings available on the platform. 

Currently, the benefits platform only has basic employee information, e.g. employee ID, personal email address, full name, and additional data will need to be shared to include dependants as beneficiaries. The employee dependant data exists within ITeLO's systems, and the benefits platform will need to communicate with these systems to retrieve employee dependant data. The employee dependant data is distributed across different geographies, Americas and the European Union (EU). The Americas server stores data for employees in the American continent, whilst the EU instance stores data for employees in the EU. 

We are in charge of building the integration scenario to allow the benefits platform access to the employee dependants' data.
  
The benefits platform will send us a request for an employee ID. We will need to validate the employee ID against our SAP S/4HANA Cloud system before requesting the employee dependant data from the servers hosting the data. 

## Prerequisites

The prerequisites to follow the exercises in this repository, including hardware and software, are detailed in the [prerequisites](prerequisites.md) file.

## Material organization

The material consists of a series of exercises. These exercises build on each other and should be completed in the given order. For example, we start by creating a simple integration flow, and we will extend it in the subsequent exercises.

## Exercises

During the CodeJam you will complete each exercise one at a time. At the end of each exercise, questions are included to help you think about the content just covered and are to be discussed with the entire CodeJam class, led by the instructor, when everyone has finished that exercise.

If you finish an exercise early, please resist the temptation to continue with the next one. Instead, explore what you've just done and see if you can learn more about the subject covered. That way, we all stay on track together and can benefit from some reflection via the questions (and answers).

See below for an overview of the exercises part of this CodeJam.

* Please ensure that you have completed all the [prerequisites](prerequisites.md).
* Exercises:
  * [Exercise 01 - Getting familiar with the SAP API Business Hub](./exercises/01-getting-familiar-api-business-hub/README.md)
  * [Exercise 02 - Exploring the mock services (Cloud Integration)](./exercises/02-exploring-the-mock-services/README.md)
  * [Exercise 03 - Build our first integration flow](./exercises/03-build-first-integration-flow/README.md)
  * Exercise 04 - Retrieve Business Partner dependant's information
  * Exercise 05 - Log service call in Google BigQuery (Open Connectors)
  * Exercise 06 - Add security to unsecure service (API Management)

## Known Issues

None

## Feedback

If you can spare a couple of minutes at the end of the session, please help us improve for next time by giving me some feedback.

Simply use this [Give Feedback](https://github.com/SAP-samples/connecting-systems-integration-suite-codejam/issues/new?assignees=&labels=feedback&template=session-feedback-template.md&title=Feedback) link to create a special "feedback" issue, and follow the instructions there.

Gracias/Thank you/Obrigado/Merçi/Danke!

## How to obtain support
Support for the content in this repository is available during CodeJam events, for which this content has been designed.

Alternatively, if you are completing this CodeJam on your own, outside of an event, you can [create an issue](https://github.com/SAP-samples/connecting-systems-integration-suite-codejam/) in this repository if you find a bug or have questions about it.
 
For additional support, [ask a question in SAP Community](https://answers.sap.com/questions/ask.html).

## Contributing
Please send a pull request if you wish to contribute code or offer fixes or improvements. Due to legal reasons, contributors will need to accept a DCO when they create the first pull request for this project. This happens in an automated fashion during the submission process. SAP uses [the standard DCO text of the Linux Foundation](https://developercertificate.org/).

## License
Copyright (c) 2022 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.

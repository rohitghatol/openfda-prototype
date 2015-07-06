# Visualizing data for Adverse Drug Reactions 

## Live Prototype
[Click here to view the prototype](http://mayuresh.github.io/openfda-prototype/index2.html)

## Description
This tool presents the top ten adverse reactions reported. While the reports to FDA do not require that a causal relationship between a product and event be proven, and reports do not always contain enough detail to properly evaluate an event, we have provided the drill down on each adverse reaction to reflect the occurrence of SUSPECT drug reported in the adverse action report.
Prototype built using data from https://open.fda.gov 

## Source code

The Source code for the prototype is hosted at https://github.com/mayuresh/openfda-prototype

All the source files, installation documentation, readme.md file, supporting documentation, license file, evidence, test results etc. are uploaded here.

## Container Image

The container image for the prototype can be found - https://registry.hub.docker.com/u/anilallewar/openfda-prototype/

## Approach (750 Word Limit):

In this phase we went through the available apis and interviewed sample users to come up with use case that would be helpful to our users. We came up with the usecase of finding top 10 list of "Adverse drug reactions" and "Drugs that could casue those reactions".

While building the prototype, we followed "US Digital Services Playbook" as our guide to ensure we deliver successful Agile Service prototype.

### Requirements
Our requirements began looking at the API of openFDA and understanding the capabilities of the system. This was followed by identifying a set of users and conducting the interviews. The data from the interviews and the research on the APIs lead us to requirements for "Visualizing data for adverse drug reactions". Next step was to identify the User Stories on an Internal Jira Server. These User Stories also recorded Functionality, Usability 508 compliance, Security and Technical considerations of the feature.

### User Experince Design
One of our experienced Team member analysed the end to end requirements, and proposed an high level flow of the Application. This was followed by quick picture based mockups and finally a working mockup in HTML5. Our overall design was inspired by industry UI Conventions by Twitter BootStrap and Zurb Foundation. 

One of the key requirements which was note was to ensure the UI is responsive and excessive by any Modern Smartphone browsers.

### Technical Design
We choose to keep the Design as Simple as Possible, using industry conventions for rapid development and low cost. 
Following Frameworks were used for building this Prototype

* [Twitter BootStrap](http://getbootstrap.com/) - For Responsive and Modern UI Design
* [Angular Js](https://angularjs.org/) - For JavaScript based Single Page Application
* [Zing Charts](http://www.zingchart.com/) - For Charts with export options
* [D3JS Visualization Framework] (http://d3js.org/) - For Data Visualization
* [Gulp](http://gulpjs.com/) - Build tool for Javascript world
* [Docker](https://www.docker.com/) - For Running the "Adverse Drug Reactions" Docker Image
 
### Deployment
Dockerfile was defined along with the Source Code. On the Development environment Docker Container was built and pushed to docker hub. On the Digital Ocean Production machine, a Docker Machine was procured and Container Image was pulled and run.











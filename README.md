
## Create pipelines as multi branch project
Pipelines should be created as [multibranch project](https://jenkins.io/doc/book/pipeline/multibranch/).

**Benefits:**
* Jenkins automatically discovers, manages and executes Pipelines for branches which contain a Jenkinsfile in source control. 

## Pipeline as code
Pipelines should be coded using a [Jenkinsfile](https://jenkins.io/doc/book/pipeline/jenkinsfile) and stored into the source code repository.

**Benefits:**
* Code review/iteration on the Pipeline.
* Audit trail for the Pipeline.
* Single source of truth for the Pipeline, which can be viewed and edited by multiple members of the project.
* History available thanks to the source code repository.
* Pipeline as code means pipeline as you want... Your dreams becomes reals!

## Pipeline as declarative
Pipeline should be coded as [declarative](https://jenkins.io/doc/book/pipeline/syntax).

**Benefits:**
* Pipeline as delarative is more human readable. 
* Declarative pipeline is maintained by Jenkins community. 

## Build as much in parallel as possible
Tasks without strong dependencies should be processed in parallel.

**Benefits:**
* Fails faster. For instance, pipelines, which builds two artifcacts, should be processed in parallel.  

## Monitor pipelines
Pipelines should be monitored using the following plugin: [Build Monitor Plugin](https://wiki.jenkins.io/display/JENKINS/Build+Monitor+Plugin)

**Benefits:**  
* Having a dashoard containing all pipelines status is a must have for minitoring daily.

## Build on commit!
Pipelines should be triggered for each commits into the source code repository.

**Benefits:**
* Fails fast. Commits are tested though the pipeline as soon as possible.   
* Pipeline status is up-to-date.

## Identical pipeline for all branches
Pipelines should be identical between branches. You should use the Jenkins variables for having a generic Jenkinsfile.

**Benefits:**
* Merge between branches is easier. 

## Add timeout for aborting pipeline
Pipelines should be aborted if too long.

**Benefits:**
* Fails fast. If a pipeline is too long, it is not a good practice and should be aborted.

## Add badges for version and duration
Badges should be added for monitoring versioning and duration.

**Benefits:**
* Monitor quickly pipelines duration and alert if too long. 
* Having the latest version for artifacts built by pipelines very quickly. 

## Avoid parameters as much as possible
Pipelines should avoid as musch as possible parameters.

**Benefits:**
* No expertise is needed for runnning a pipeline.

## Extend pipelines with shared librairies
Pipelines should be based on shared libraries.

**Benefits:**
* All pipelines will be processed using the sae implemetntation for common tasks (checkout, push, ...)

## Follow Sementic Versioning 
Pipelines should build deliveries using the sementic versioning.

**Benefits:**
* This is a well known standard for Github community.

## Dedicated source code repository per pipelines
Pipelines should be defined though a dedicated source code repository.

**Benefits:**
*  



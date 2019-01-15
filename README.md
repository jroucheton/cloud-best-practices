
## Creating pipelines as multi branch project
Pipelines should be created as [multibranch project](https://jenkins.io/doc/book/pipeline/multibranch/).

**Benefits:**
* Jenkins automatically discovers, manages and executes Pipelines for branches which contain a Jenkinsfile in source control. 

## Using pipelines as code
Pipelines should be coded using a [Jenkinsfile](https://jenkins.io/doc/book/pipeline/jenkinsfile) and stored into the source control.

**Benefits:**
* Code review/iteration on the Pipeline.
* Audit trail for the Pipeline.
* Single source of truth for the Pipeline, which can be viewed and edited by multiple members of the project.
* History available thanks to the source control.
* Pipeline as code means pipeline as you want... Your dreams becomes reals!

## Writing pipelines as declarative
Pipelines should be coded as [declarative](https://jenkins.io/doc/book/pipeline/syntax/#declarative-pipeline).

**Benefits:**
* Pipeline as delarative is more human readable. 
* Declarative pipeline is maintained by Jenkins community. 

## Working with stages
Pipelines should be define using [stages](https://jenkins.io/doc/pipeline/steps/pipeline-stage-step).

**Benefits:**
* Pipelines stages appears as pipelines steps. 

## Building as much in parallel as possible
Tasks without strong dependencies should be processed in [parallel](https://jenkins.io/doc/book/pipeline/syntax/#parallel).

**Benefits:**
* Fails faster. For instance, pipelines, which builds two artifcacts, should be processed in parallel.  

## Monitoring pipelines
Pipelines should be monitored using the following plugin: [Build Monitor Plugin](https://wiki.jenkins.io/display/JENKINS/Build+Monitor+Plugin)

**Benefits:**  
* Having a dashoard containing all pipelines status is a must have for minitoring daily.

## Building on commit
Pipelines should be triggered for each commits into the source control.

**Benefits:**
* Fails fast. Commits are tested though the pipeline as soon as possible.   
* Pipeline status is up-to-date.

## Working with the Environment
Jenkins exposes environment variables via the global variable env, which is available from anywhere within a Jenkinsfile.
The full list of environment variables accessible from within Jenkins Pipeline is documented at: JENKINS_URL/pipeline-syntax/globals#env
 
**Benefits:**
* Write a generic Jenkinsfile as much as possible.

## Handling failures with email
Declarative pipelines support robust failure handling by default via its post section which allows declaring a number of different "post conditions" such as: always, unstable, success, failure, and changed.

**Benefits:**
* Send an e-mail to your team.

## Adding timeout for aborting pipeline
Pipelines should be aborted if too long thank to a [timeout](https://jenkins.io/doc/book/pipeline/syntax/#options-example).

**Benefits:**
* Fails fast. If a pipeline is too long, it is not a good practice and should be aborted.

## Adding badges for version and duration
[Badges](https://jenkins.io/doc/pipeline/steps/badge) should be added for monitoring versioning and duration.

**Benefits:**
* Monitor quickly pipelines duration and alert if too long. 
* Having the latest version for artifacts built by pipelines very quickly. 

## Avoiding parameters as much as possible
Pipelines should avoid as musch as possible [parameters](https://jenkins.io/doc/book/pipeline/syntax/#parameters).

**Benefits:**
* No expertise is needed for runnning a pipeline.
* Only one click for running a pipeline!

## Extending pipelines with shared librairies
Pipelines should be based on [shared libraries](https://jenkins.io/doc/book/pipeline/shared-libraries).

**Benefits:**
* All pipelines will be processed using the sae implemetntation for common tasks (checkout, push, ...)

## Following Sementic Versioning 
Pipelines should build deliveries using the [sementic versioning](https://semver.org).

**Benefits:**
* This is a well known standard for Github community.



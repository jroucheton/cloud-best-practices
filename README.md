
## Pipeline as code
Pipelines should be coded through one file and stored into the source code repository.

> Create a jenkinsfile and store it into the source code repository.

**Benefits:**
* Configuration is located in a single place. 
* History is available thanks to the source code repository.

## Pipeline as declarative
Pipeline should be coded as much in a declarative way as possible.

**Benefits:**
* Configuration is more human readable. 
* Declarative pipeline is the type which is more maintained by Jenkins community. 

## Build as much in parallel as possible
Tasks without dependencies should be processes in parallel.

**Benefits:**
* Fails faster.

## Monitor pipelines
Pipelines status should be monitored. 

**Benefits:**  
* 

## Build on comit!
Pipilines should be triggered for each commits into the source code repository.

**Benefits:**
* Fails fast. 
* Pipeline status is up-to-date.

## Identical pipeline for all branches
Pipelines should be identical between branches.

**Benefits:**
* Merge between branches is easier. 

## Add timeout for aborting pipeline
Pipelines should be aborted if too long.

**Benefits:**
* Fails fast.

## Add badges for version and duration
Badges should be added for monitoring versioning and duration.

**Benefits:**
* Monitor quickly pipelines duration and alert if too long. 
* Having the latest version for artifacts built by pipelines very quickly. 

## Avoid parameters as much as possible
Pipelines should avoid as musch as possible parameters.

**Benefits:**
* No expertise is needed for runnning a pipeline.

## Use Jenkins env as much as possible


## Extend pipelines with shared librairies
Pipelines should be based on shared libraries.

**Benefits:**
* All pipelines will be processed using the sae implemetntation for common tasks (checkout, push, ...)

## Follow Sementic Versioning 
Pipelines should build deliveries using the sementic versioning.

**Benefits:**
* This standard is well know for Github community.

## Create pipelines as multi branch project
Pipelines should be created as multi branch project.

**Benefits:**
* A new pipeline is created automatically if a new banch is created.

## Only one Jenkinsfile per source code management
Pipelines should contain only configuration file per source code repository.

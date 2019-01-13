
### Pipeline as code
Pipelines should be coded through one file and stored into the source code repository.

> Jenkins tips
>
> Store jenkinsfile into the source code repository.

### Pipeline as declarative
Pipeline should be coded as much in a declarative way as possible.

### Build as much in parallel as possible
Tasks without dependencies should be processes in parallel.

### Monitor pipelines
Pipelines status should be monitored. 

### Build on comit!
Pipilines should be triggered for each commits into the source code repository.

### Identical pipeline for all branches
Pipelines should be identical between branches.

### Add timeout for aborting pipeline
Pipelines should be aborted if too long.

### Add badges for version and duration
Badges should be added for monitoring versioning and duration.

### Avoid parameters as much as possible
Pipelines should avoid as musch as possible parameters.

### Use Jenkins env as much as possible


### Extend pipelines with shared librairies
Pipelines should be based on shared libraries.

### Follow Sementic Versioning for deliveries 
Pipelines should build deliveries using the sementic versioning.

### Create pipelines as multi branch project
Pipelines should be created as multi branch project.

### Only one Jenkinsfile per source code management
Pipelines should contain only configuration file per source code repository.

[Lucidchart](https://lucid.app/lucidchart/dc9b75e2-8eb9-4329-81db-72627a4cf818/edit?page=0_0&invitationId=inv_77c71f7f-6b53-4db2-929e-2c40d0da53ec#)

# CIT BATCH

## Job
### Job (Batch Process)
- contains 1 or more Steps
### Job Parameters
- params for job
### Job Instance
- Job + JobParameters
### Job Execution
- A signle run of JobInstance
- tracks what happened during a run
	- current statuses
	- exit statuses
	- start time
	- end time
	- etc

### Job Launcher
- executes a job

### Job Repository 
- JobRepository is the mechanism in CIT Batch that makes all this persistence possible.
- provides CRUD op4,erations for JobLauncher, Job, and Step instantiations.
- Once a Job is launched, a JobExecution is obtained from the repository and, during the course of execution, StepExecution and JobExecution instances are persisted to the repository.


## Step
### Step
- ItemReader
- ItemProcessor
- ItemWriter

### StepExecution
- Single attempt to execute a step
- contains
	- current statuses
	- exit statuses
	- start time
	- end time
	- etc
- references to
	- corresponding step instance
	- JobExecution instance


## ExecutionContext
- set of key-value pairs, containing info that is scoped to either StepExecution or JobExecution.
- CIT Batch persists the ExecutionContext, which helps in cases where you want to restart a batch run (e.g., when a fatal error has occurred, etc.). All that is needed is to put any object to be shared between steps into the context and the framework will take care of the rest. After restart, the values from the prior ExecutionContext are restored from the database and applied.
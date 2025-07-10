# Exercise 1: Hello Workflow
During this exercise, you will
* Review the business logic of the provided Workflow Definition to understand its behavior
* Modify the Worker initialization code to specify a task queue name
* Run the Worker initialization code to start the Worker process
* Run code that submits a request to execute the Workflow, specifying your name as input

Make your changes to the code in the `practice` subdirectory (look for TODO 
comments that will guide you to where you should make changes to the code). 
If you need a hint or want to verify your changes, look at the complete version 
in the `solution` subdirectory.

## Part A: Review the Workflow Business Logic

1. Open the `greeting.go` file (located in the `practice` subdirectory) 
   in the editor
2. Review the input parameters, business logic, and return value. 

## Part B: Specify a Task Queue Name for the Worker

1. Open the `worker/main.go` file (located in the `practice` subdirectory) 
   in the editor
2. Specify `greeting-tasks` as the name of the task queue
3. Save your changes

## Part C1: Fetch the Dependencies

1. Open a terminal window in the environment and change to the 
   `practice` subdirectory for this exercise
2. Run the following command to download and install the Go packages 
   needed by the code, which will include the Temporal Go SDK

```
go mod tidy
```

## Part C2: Start the Worker

2. Run the following command in the terminal window to start the Worker

```
go run worker/main.go
```

## Part D: Start the Workflow

1. Open another terminal window in the environment and change to the 
   `practice` subdirectory for this exercise
2. Run the following command, replacing `Donna` with your own name. 

```
go run start/main.go Donna
```

This program starts the Workflow, waits for it to finish, and then 
displays the result. 

If you have time, continue with the optional part of the exercise 
below to see how to use the `temporal` command to display the result.

## Part E: Display the Result
Run the following command to display the result of a Workflow Execution: 

```bash
temporal workflow show --workflow-id my-first-workflow
```

It is also possible, and usually more convenient, to view this information 
using the Temporal Web UI. Do this now by opening your browser to
<http://localhost:8233>.


### This is the end of the exercise.





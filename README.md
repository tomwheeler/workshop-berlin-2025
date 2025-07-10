# workshop-berlin-2025
Code related to the "Introduction to Temporal" workshop that I am teaching
at the We Are Developers conference in Berlin (July 11, 2025).

## Prerequisites
To complete the hands-on exercises in this workshop, you need three things:
1. A clone of this repository to your laptop
2. A working installation of [Go](https://go.dev/dl/), version 1.23 or higher
3. A working installation of the `temporal` command-line tool, also known as
   the Temporal CLI. If you haven't installed this, follow the instructions
   in the [Install the Temporal CLI](https://docs.temporal.io/cli#install) 
   section of the Temporal documentation. 

Before beginning the first exercise, run `temporal server start-dev` to start
a local Temporal Service. Leave it running for the duration of the workshop,
since it's required for the second exercise too.



## Hands-On Exercises

Directory Name                | Exercise
:---------------------------- | :----------------------------
`exercises/hello-workflow`    | [Exercise 1](exercises/hello-workflow/README.md)
`exercises/farewell-workflow` | [Exercise 2](exercises/farewell-workflow/README.md)

Each of these exercise directories contains two subdirectories: 
1. `practice` - This is where you'll modify the code as instructed
2. `solution` - This is the completed version for comparison


## Reference
The following links provide additional information that you may find 
helpful as you work through this course.
* [General Temporal Documentation](https://docs.temporal.io/)
* [General Go Language Documentation](https://go.dev/doc/)
* [Temporal Go Developer Guide](https://docs.temporal.io/develop/go/)
* [Temporal Go SDK API Documentation](https://pkg.go.dev/go.temporal.io/sdk)

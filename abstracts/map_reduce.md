MapReduce is a programming model and an associated
implementation for processing and generating large
data sets. Users specify a map function that processes a
key/value pair to generate a set of intermediate key/value
pairs, and a reduce function that merges all intermediate
values associated with the same intermediate key. Many
real world tasks are expressible in this model, as shown
in the paper.

Programs written in this functional style are automatically
parallelized and executed on a large cluster of commodity
machines. The run-time system takes care of the details
of partitioning the input data, scheduling the program's
execution across a set of machines, handling machine
failures, and managing the required inter-machine
communication. This allows programmers without any
experience with parallel and distributed systems to easily
utilize the resources of a large distributed system.

Our implementation of MapReduce runs on a large cluster
of commodity machines and is highly scalable: a typical
MapReduce computation processes many terabytes of data on
thousands of machines. Programmers find the system easy to
use: hundreds of MapReduce programs have been implemented
and upwards of one thousand MapReduce jobs are executed
on Google's clusters every day.

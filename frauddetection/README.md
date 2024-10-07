## Notes

completed the FraudDetection tutorial : https://nightlies.apache.org/flink/flink-docs-release-1.20/docs/try-flink/datastream/

The main objective was to get a good introduction to the working of the DataStreamAPI

Other concepts introduced:

Job - defines the data flow pipeline
Process Function - defines an operator that takes in a class with business logic to be executed on the data
KeyedProcessFunction - uses a key to create a context for a specific key on which all operations on the data are filtered on that key. This is because the process of the process function is an object and does not create a new instance for every item in the stream. The key is used to provide this context.
ValueState is used to declare a context variable and retrieve the value of the data stored.
ValueDescriptor is used to define the name of the state and its type and add it to run time context
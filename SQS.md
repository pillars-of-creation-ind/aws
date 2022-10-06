# Simple Queue Service

Amazon Simple Queue Service (SQS) is managed queuing service used to send,
store and retrieve multiple messages of various sizes

It enables users to decouple individual microservices, distributed systems and serverless applications from one another and to scale them.
It delivers high-performance standards due to its ability to decouple the various components of each applications.

### How SQS is used ?

- To safely exchange messages between different software components
- Provides a standard web services (API) that users can access
- Supports tasks `asynchronously`, it sends a message into a queue, where it waits.

### Types of SQS Queues

- FIFO (First in, First out)

  1. Message strings remain in same order in which the original message were sent and received.
  2. Support upto 300 send, receive and delete messages per second.
  3. FIFO queues are designed for messaging between applications where the order of operartions and events is critical.
  4. Frequency of message: Messages are delivered exactly once

- Standard Queue

  1. Message strings remain in same order in which the original message were sent, but processing requirements may change the original order or sequence of message.
     eg: standard queue is used to batcg messages for future processing or allocate tasks to multiple worker nodes.
  2. Frequency of message: Messages are delivered least once.

### Features

- No of Messages: No limit on the number of messages that any individual SQS message queue can contain.
- Message Name: Name of the message queue can be no longer than 80 characters.
- Period: SQS messages retention period can be set from one minute to 14 days. Messages are automatically deleted once the message retention quota has been reached.
- Security: SQS delivers server-side encryption to safely send and receive confidential or sensitive data between applications.
- Pricing: 1 month SQS requests for free each month with free tier

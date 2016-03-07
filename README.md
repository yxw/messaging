# messaging
Readings/References for low latency messaging

## Messaging in different levels:
### inter-thread messaging:
[LMAX Disruptor](http://lmax-exchange.github.io/disruptor/)

### Node-to-node (cross network) messaging:
ZeroMQ, Netty (used by Apache Storm)

### Standalone distributed messaging system:
Apache Kafka
RabbitMQ

## Messaging in Apache Storm
- Inter-thread (Intra-worker) communication: LMAX Disruptor
- Node-to-node (Inter-worker) communication: ZeroMQ or Netty
- Inter-topology communication: nothing built into Storm, you must take care of this yourself.

See 1[1] for more details on messaging in Storm.

References:
1. [Understanding the Internal Message Buffers of Storm](http://www.michael-noll.com/blog/2013/06/21/understanding-storm-internal-message-buffers/)
2. [Integrating Kafka and Storm](http://www.michael-noll.com/blog/2014/05/27/kafka-storm-integration-example-tutorial/)
3. 

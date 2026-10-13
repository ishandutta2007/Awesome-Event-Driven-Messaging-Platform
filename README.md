# Awesome-Event-Driven-Messaging-Platform

## Top Event-Driven Messaging Platform Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Pub/Sub, Message Brokers & Real-Time Event Streaming*  

**Last updated: March 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Event-Driven Messaging Platforms**. These tools enable organizations to build decoupled, asynchronous architectures where producers publish events and consumers react in near real-time—supporting microservices communication, IoT telemetry, and distributed system coordination.



**Examples** include Salesforce Platform Events, AWS SNS, Azure Service Bus, Google Cloud Pub/Sub, Apache Pulsar Cloud, RabbitMQ Cloud, Confluent Cloud, Redpanda Cloud, Solace Cloud, and NATS Cloud (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, custom event routing, and open messaging infrastructure—ideal for platform engineers, architects, and developers seeking transparent, vendor-independent event-driven messaging.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Salesforce Platform Events](https://developer.salesforce.com/docs/platform/platform-events/guide/platform-events-intro-emp.html)**

  Enterprise messaging platform based on publish-subscribe model. Publishers and subscribers communicate through events without knowing each other. One or more subscribers can listen to the same event and carry out actions. Custom platform events are defined like custom objects. High-volume platform events publish asynchronously with at-least-once delivery. Standard-volume custom events retire in Summer '27. Event Relay provides no-code delivery to Amazon EventBridge .



- **[AWS SNS](https://aws.amazon.com/sns/)**

  Fully managed pub/sub messaging for Application-to-Application (A2A) and Application-to-Person (A2P). Supports standard and FIFO topics. Messages not persisted—delivered in real-time to subscribers. At-least-once delivery for HTTP/S, exactly-once for Lambda and SQS. Supports HTTP/S endpoints, email, SMS, mobile push, Lambda, and SQS queues. Subscription filter policies enable selective message delivery .



- **[Azure Service Bus](https://azure.microsoft.com/en-us/products/service-bus/)**

  Fully managed enterprise message broker with queues and publish-subscribe topics. Queues for point-to-point; topics for pub/sub with multiple independent subscriptions. Messages persisted in triple-redundant storage across availability zones. Pull-based delivery. Features sessions for FIFO, auto-forwarding, transactions, and dead-letter queues. Serverless PaaS—no hardware patching or backup management .



- **[Google Cloud Pub/Sub](https://cloud.google.com/pubsub)**

  Asynchronous messaging service decoupling senders and receivers. Core concepts: publisher, message, topic, schema, subscription, subscriber. Messages written to storage then delivered to all attached subscriptions. Acknowledged messages deleted after all subscriptions ack. Unacknowledged messages redelivered until retention expires. Supports fan-in, load-balanced, and fan-out patterns .



- **[Apache Pulsar Cloud](https://pulsar.apache.org/)**

  Cloud-native distributed messaging and streaming. Proven at scale serving millions of messages per second. Layered architecture separates compute (brokers) from storage (BookKeeper). Features multi-tenancy, geo-replication, tiered storage, and low latency (<10ms). Supports up to 1M topics. Six official client languages. Serverless Functions and 3rd party connectors .



- **[Confluent Cloud](https://www.confluent.io/confluent-cloud/)**

  Fully managed Apache Kafka service built on Kora cloud-native engine. Autoscaling clusters right-size infrastructure automatically. 99.99% uptime SLA. 120+ pre-built and 80+ fully managed connectors. Features Cluster Linking for multi-region sync, Stream Governance, Flink for stream processing, and Tableflow for Iceberg/Delta Lake materialization. Available on AWS, Azure, and GCP across 100+ regions .



- **[Solace PubSub+ Cloud](https://solace.com/cloud-dev-pubsub/)**

  Enterprise-grade event broker as a service. Supports pub/sub, queuing, streaming, replay, and request/reply. Open protocols: AMQP, MQTT, JMS, REST, WebSocket. Deployable in shared VPC, customer VPC, dedicated VPC, or on-premises Kubernetes. Features Event Portal for event management and dynamic event mesh across distributed enterprise .



- **[Redpanda Cloud](https://www.redpanda.com/redpanda-cloud)**

  Fully managed streaming data platform with Kafka API compatibility. Built on same high-performance core without JVM or ZooKeeper. BYOC (Bring Your Own Cloud) for data sovereignty, Dedicated clusters, and Serverless with zero base cost. 99.99% uptime SLA for BYOC. Runs on 3x fewer compute resources than Apache Kafka.



- **[RabbitMQ Cloud](https://www.rabbitmq.com/)**

  Managed RabbitMQ service. Supports AMQP, MQTT, STOMP protocols with flexible routing, message queuing, and pub/sub capabilities.



- **[NATS Cloud](https://nats.io/)**

  Managed NATS service. Core NATS offers at-most-once QoS (fire-and-forget). JetStream enables at-least-once/exactly-once, persistent streaming, and Key/Value Store. Single binary server (~15MB memory footprint). Official clients for Go, JavaScript, Python, Java, Rust, C#/.NET, and C .



## Open-Source GitHub Projects



- **[Apache Pulsar](https://github.com/apache/pulsar)**

  Open-source distributed messaging and streaming platform (Apache-2.0). Top 10 Apache Software Foundation project. Features low-latency messaging (<10ms), rapid horizontal scalability, seamless geo-replication, multi-tenancy, automatic load balancing, and tiered storage. Supports up to 1M topics. Official clients for Java, Go, Python, C++, Node.js, and C#. Serverless Functions and 3rd party connectors for MySQL, Elasticsearch, Cassandra .



- **[NATS](https://github.com/nats-io/nats-server)**

  Open-source messaging system (Apache-2.0) optimized for simplicity, performance, and security. Single binary server. Process millions of messages per second with sub-millisecond latency and ~15MB memory footprint. Core NATS offers at-most-once QoS; JetStream adds at-least-once/exactly-once, persistent streaming, and Key/Value Store. Location transparency with service discovery and load balancing. Multi-tenancy via accounts. Use cases include agentic AI, IoT telemetry, microservices, and edge computing .



- **[Apache EventMesh](https://github.com/apache/eventmesh)**

  New generation serverless event middleware (Apache-2.0) for distributed event-driven applications. Built around CloudEvents specification. Extensible connector layer using openConnect for SaaS, CloudService, and Database sources/sinks. Storage layer supports RocketMQ, Kafka, Pulsar, RabbitMQ, Redis. Meta layer supports Consul, Nacos, ETCD, Zookeeper. At-least-once delivery. Event schema management, serverless workflow orchestration, event filtering and transformation .



- **[Centrifugo](https://github.com/centrifugal/centrifugo)**

  Scalable real-time messaging server in language-agnostic way (Apache-2.0). Self-hosted alternative to Pubnub, Pusher, Ably, socket.io. Features WebSocket, HTTP-streaming, SSE, GRPC, WebTransport. Built-in scalability with Redis or NATS. JWT and proxy authentication, channel multiplexing, hot message history, delta compression, presence information .



- **[Outpost (Hookdeck)](https://github.com/hookdeck/outpost)**

  Self-hostable open-source outbound webhooks infrastructure (Apache-2.0). Pushes events to customer-defined destinations: webhook endpoints, SQS, RabbitMQ, Kinesis. At-least-once delivery with retry logic. Multi-tenant support. REST API, SDKs for Go/TypeScript/Python. Topic-based subscriptions, OpenTelemetry integration .



- **[Ripple](https://github.com/madisoheib/Ripple)**

  Self-hosted, Pusher-compatible WebSocket server (license varies). Single static Rust binary. Speaks Pusher Channels protocol so existing clients work unchanged. No Redis, Node, or PHP extensions required. Bounded buffers with slow-client disconnect. Benchmarks: 512 MiB at 40k connections, sustained 50k deliveries/s at p50 14.7ms .



- **[Soketi](https://github.com/soketi/soketi)**

  Next-gen, Pusher-compatible open-source WebSocket server (MIT). Implements Pusher protocol for drop-in replacement. Public, private, presence, and encrypted channels. Horizontal scaling via Redis. Deployable via npm, Docker, Kubernetes, or systemd .



- **[Event (rbaliyan)](https://github.com/rbaliyan/event)**

  Go event bus library (license varies) with reliability primitives. Outbox pattern for transactional publishing, idempotency middleware, poison message quarantine, per-message monitoring, schema provider with strict mode, dead letter queue, producer-side audit log. Supports Redis Streams (recommended) and NATS transports with consumer groups .



### Additional Strong Open-Source Options



- **[RabbitMQ](https://github.com/rabbitmq/rabbitmq-server)** — Open-source message broker (MPL-2.0) with AMQP, MQTT, and STOMP support.

- **[Apache Kafka](https://github.com/apache/kafka)** — Distributed event streaming platform (Apache-2.0) with massive ecosystem.

- **[Redis Streams](https://github.com/redis/redis)** — Log-based messaging with consumer groups and at-least-once delivery.

- **[EMQX](https://github.com/emqx/emqx)** — MQTT broker (Apache-2.0) for IoT and real-time messaging at scale.

- **[MQTT.js](https://github.com/mqttjs/MQTT.js)** — MQTT client for JavaScript/Node.js pub/sub applications.

- Community **n8n** workflows for event routing and cross-platform message delivery.



**Frameworks for building custom systems**: Combine **Apache Pulsar** or **NATS** as the messaging core with **Apache EventMesh** for multi-protocol interconnector layer, **Centrifugo** or **Ripple** for real-time WebSocket delivery, **Outpost** for outbound webhook infrastructure, and **Event (rbaliyan)** for reliability primitives — creating a fully self-hosted, enterprise-grade event-driven messaging platform.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Event-driven messaging platforms handling business events must comply with data protection regulations (GDPR, CCPA, etc.).

- Self-hosted open-source solutions require proper security hardening, TLS configuration, and ongoing maintenance. Message delivery guarantees (at-least-once, exactly-once) have different trade-offs—choose based on idempotency requirements and downstream tolerance for duplicates.



---



**Made for platform engineers, architects, backend developers, and organizations building transparent event-driven messaging solutions.**  

Let's make Event-Driven Messaging Platforms more open, data-driven, and reliable.

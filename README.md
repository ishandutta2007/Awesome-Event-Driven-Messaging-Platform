# Awesome-Event-Driven-Messaging-Platform

## Top Event-Driven Messaging Platform Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Pub/Sub, Message Brokers & Real-Time Event Streaming*  

**Last updated: October 2026**



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

| Platform | Description & Key Features | Starting Pricing | Free Tier / Trial Limits |
| :--- | :--- | :--- | :--- |
| **[Salesforce Platform Events](https://developer.salesforce.com/docs/platform/platform-events/guide/platform-events-intro-emp.html)** | Enterprise messaging platform based on pub/sub model. Publishers and subscribers communicate asynchronously via events. High-volume platform events publish with at-least-once delivery; Event Relay delivers events to Amazon EventBridge. | Enterprise Edition starts at $165/user/month (includes base platform events); High-Volume Platform Events Add-On starts at $500/month (+100,000 events/day). | **Permanent Free Developer Edition**: 10,000 delivered events/24 hrs, 20 concurrent CometD subscribers, and 5 custom event definitions; 30-day free trial orgs available. |
| **[AWS SNS](https://aws.amazon.com/sns/)** | Fully managed pub/sub messaging for A2A and A2P. Supports standard and FIFO topics, subscription filtering, and message fan-out to SQS, Lambda, HTTP/S, and mobile push. | $0.50 per 1 million requests (Standard topics; FIFO topics at $0.30/1M requests + $0.09/GB payload); HTTP/S delivery at $0.60 per 1M notifications. | **Permanent Free Tier**: 1,000,000 API requests/month, 100,000 HTTP/S notifications/month, 1,000 email notifications/month, and 1,000,000 mobile push notifications/month (deliveries to SQS and Lambda are free). |
| **[Azure Service Bus](https://azure.microsoft.com/en-us/products/service-bus/)** | Fully managed enterprise message broker with queues for point-to-point and topics for pub/sub with independent subscriptions, dead-lettering, sessions, and transactions. | Basic tier starts at $0.05 per million operations (queues only, $0 base fee); Standard tier starts at ~$10.00/month base unit (~$0.0135/hr, includes 13M ops), then $0.05 per million operations. | **12-Month Free Trial** (via Azure Free Account): 750 hours/month of Standard tier base unit and 13 million operations/month for 12 months, plus $200 credit for the first 30 days. |
| **[Google Cloud Pub/Sub](https://cloud.google.com/pubsub)** | Asynchronous messaging service decoupling producers and consumers. Features at-least-once delivery, schemas, and fan-in / fan-out patterns. | Standard throughput starts at $40.00 per TiB ($0.04/GiB) after free tier; Pub/Sub Lite starts at $0.005/MiBps partition-hour + $0.04/GiB-month storage. | **Permanent Always Free Tier**: 10 GiB of message throughput/month and first 24 hours of message storage free; new GCP accounts receive a 90-day $300 trial credit. |
| **[Apache Pulsar Cloud (StreamNative)](https://streamnative.io/)** | Cloud-native distributed messaging and streaming powered by Apache Pulsar. Features layered compute/storage separation, multi-tenancy, and geo-replication. | Serverless tier starts at ~$0.50 per ETU (Elastic Throughput Unit) per hour + $0.10/GB-month storage. | **30-Day Free Trial**: $200 in free credits (no credit card required) for Serverless cluster evaluation. |
| **[Confluent Cloud](https://www.confluent.io/confluent-cloud/)** | Fully managed Apache Kafka service built on Kora engine. Features autoscaling clusters, 120+ pre-built connectors, Stream Governance, and managed Flink. | Basic tier starts at $0/month base fee with usage at ~$0.11/GB data ingress, ~$0.11/GB egress, and $0.10/GB-month storage; Standard tier starts at ~$1.50/hour base. | **30-Day Free Trial**: $400 in free credits (no credit card required upfront) valid across Basic, Standard, Enterprise, and Freight clusters. |
| **[Solace PubSub+ Cloud](https://solace.com/cloud-dev-pubsub/)** | Enterprise-grade event broker as a service supporting pub/sub, queuing, streaming, and dynamic event meshes over open protocols (AMQP, MQTT, JMS, REST, WebSocket). | Foundation platform package with consumption drawdown via Platform Capacity Units (PCUs); broker instances scale per PCU-hour (enterprise starting packages via marketplace/sales). | **30-Day Free Trial**: Enterprise-100 Standalone broker with 100 concurrent connections, 100 queues/endpoints, 25 GB message spool storage, and 500,000 subscriptions; permanent Developer Service Tier ($0) capped at 100 connections. |
| **[Redpanda Cloud](https://www.redpanda.com/redpanda-cloud)** | Fully managed streaming data platform with Kafka API compatibility. Built in C++ without JVM or ZooKeeper for low latency and high resource efficiency. | Serverless tier starts at $0 base fee/hour with usage at ~$0.02–$0.045/GB ingress, ~$0.02–$0.04/GB egress, and ~$0.09/GB-month storage; Dedicated clusters start at ~$0.20/hour per broker. | **30-Day Free Trial**: $100 in free credits (no credit card required), capped at 100 MB/s ingress, 300 MB/s egress, 5,000 partitions, and 10,000 connections. |
| **[RabbitMQ Cloud (CloudAMQP)](https://www.cloudamqp.com/)** | Managed RabbitMQ service supporting AMQP 0-9-1, AMQP 1.0, MQTT, and STOMP with flexible routing, message clustering, and management console. | Shared plans start at $19/month (Tough Tiger); dedicated single-node instances start at $99/month (Big Bunny). | **Permanent Free Tier** (Little Lemur plan): 1,000,000 messages/month, 20 concurrent connections, 100 queues, and up to 10,000 queued messages (inactive instances deleted after 2 months). |
| **[NATS Cloud (Synadia Cloud)](https://synadia.com/cloud)** | Managed NATS platform offering core pub/sub, JetStream persistent streaming, Key/Value store, Object Store, and multi-region leaf nodes. | Starter plan starts at $49/month (includes 100 connections, 100 GiB network data, 10 GiB storage, 3 accounts, and 3 leaf nodes). | **Permanent Free Tier** (Personal Plan): 10 concurrent connections, 10 GiB network data/month, 5 GiB standard storage, 10 standard streams, 2 accounts, and 2 leaf nodes. |



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

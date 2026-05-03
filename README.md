# Awesome Stateful Functions [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of resources, libraries, runtimes, SDKs, and learning material for **Apache Stateful Functions** and stateful actor frameworks running on Apache Flink.

Stateful Functions (StateFun) is a programming model for distributed actor-style systems on Apache Flink — durable per-key state, exactly-once messaging, polyglot remote functions, and Kubernetes-native deployment.

## Contents

- [Runtimes](#runtimes)
- [SDKs](#sdks)
- [Examples and playgrounds](#examples-and-playgrounds)
- [Production guides](#production-guides)
- [Related actor frameworks](#related-actor-frameworks)
- [Articles and talks](#articles-and-talks)
- [Apache Flink resources](#apache-flink-resources)

## Runtimes

- [Kzmlabs StateFun Actors](https://github.com/kzmlabs/flink-statefun) - Stateful actors on Apache Flink 2.x and Java 21. Durable per-key state, exactly-once messaging, Kafka and Kinesis I/O, Kubernetes-native deployment. Continues the Apache Stateful Functions programming model on the modern Flink line.
- [Apache Flink Stateful Functions](https://github.com/apache/flink-statefun) - The original Apache project. Last release 3.4.0 (October 2024) targets Flink 1.16 and Java 11.

## SDKs

- [statefun-sdk-java](https://central.sonatype.com/artifact/io.github.kzmlabs.flinkstatefun/statefun-sdk-java) - Java SDK for remote functions, published to Maven Central.
- [statefun-sdk-python](https://github.com/apache/flink-statefun/tree/release-3.4/statefun-sdk-python) - Python SDK, upstream Apache.
- [statefun-sdk-go](https://github.com/apache/flink-statefun/tree/release-3.4/statefun-sdk-go) - Go SDK, upstream Apache.
- [statefun-sdk-js](https://github.com/apache/flink-statefun/tree/release-3.4/statefun-sdk-js) - Node.js SDK, upstream Apache.

## Examples and playgrounds

- [Kzmlabs StateFun Actors — Fraud detection example](https://kzmlabs.github.io/flink-statefun/examples/fraud-detection/) - Per-card risk scoring on a Kafka payments stream with velocity, geo-impossibility, and amount-anomaly detection. Full Java code + module.yaml.
- [Kzmlabs StateFun Actors — IoT fleet digital twins](https://kzmlabs.github.io/flink-statefun/examples/iot-fleet/) - Per-device twin actors for industrial telemetry on Kinesis with rolling stats, anomaly detection, and command/response loop.
- [flink-statefun-playground](https://github.com/apache/flink-statefun-playground) - Apache's collection of polyglot examples: Java, Python, Go, JS samples in Docker compose.

## Production guides

- [StateFun Actors documentation](https://kzmlabs.github.io/flink-statefun/) - Quickstart, install, build, Kafka/Kinesis I/O, Kubernetes deployment, architecture, and migration guide.
- [Kubernetes deployment guide](https://kzmlabs.github.io/flink-statefun/guides/k8s-deployment/) - Production layout via the Flink Kubernetes Operator with RocksDB checkpoints to S3.
- [Migration from Apache Stateful Functions](https://kzmlabs.github.io/flink-statefun/upstream-vs-kzm/) - Coordinate change, Flink 2.x configuration keys, what stays the same.

## Related actor frameworks

For context on the broader stateful-actor / durable-execution space:

- [Restate](https://restate.dev) - Durable execution for distributed services. Different runtime, similar problems.
- [Temporal](https://temporal.io) - Durable workflows. Workflow-style API rather than actor-style.
- [Akka](https://akka.io) - JVM actor framework. Different runtime model, no Flink dependency.
- [Orleans](https://github.com/dotnet/orleans) - Microsoft's virtual-actor framework on .NET.
- [Cloudflare Durable Objects](https://developers.cloudflare.com/durable-objects/) - Edge-runtime stateful actors.

## Articles and talks

- [Stateful Functions: Polyglot Event-Driven Functions for Stateful Distributed Applications](https://www.ververica.com/blog/stateful-functions-internals-behind-the-scenes-of-stateful-serverless) - Ververica's introduction to the runtime internals.
- [Apache StateFun release notes](https://nightlies.apache.org/flink/flink-statefun-docs-release-3.4/) - Latest upstream documentation.
- [Stateful Functions 2.0 — An Event-Driven Database on Apache Flink](https://flink.apache.org/2020/04/07/release-statefun-2.0.0/) - Apache Flink blog post on the 2.0 release.
- [Stateful Functions 3.0: Remote Functions Front-and-Center](https://flink.apache.org/2021/01/27/release-statefun-3.0.0/) - Apache Flink blog post on the 3.0 release.
- [Stateful Functions 3.2.0 Release Announcement](https://flink.apache.org/2022/01/31/release-statefun-3.2.0/) - Apache Flink blog post on the 3.2 release.
- [Lightweight Asynchronous Snapshots for Distributed Dataflows](https://arxiv.org/abs/1506.08603) - Carbone et al. The paper behind Flink's checkpointing, the foundation StateFun's exactly-once semantics rest on.
- [Stateful Functions: Building Event-Driven Applications](https://www.youtube.com/results?search_query=Flink+Forward+Stateful+Functions) - Flink Forward conference talks on Stateful Functions (search results, multiple years).
- [Distributed Architecture and Concepts](https://nightlies.apache.org/flink/flink-statefun-docs-release-3.4/docs/concepts/distributed_architecture/) - Apache deep-dive into how the runtime, dispatcher, and remote functions interact.

## Apache Flink resources

- [awesome-flink](https://github.com/wuchong/awesome-flink) - The canonical curated list for Apache Flink projects, libraries, and tooling.
- [Apache Flink documentation](https://nightlies.apache.org/flink/flink-docs-stable/) - The Flink runtime that StateFun runs on.
- [Flink Kubernetes Operator](https://github.com/apache/flink-kubernetes-operator) - The Operator that provisions StateFun (and Flink) jobs on Kubernetes.
- [Flink Forward conference](https://www.flink-forward.org/) - The annual Apache Flink conference. Several editions feature Stateful Functions talks.
- [Apache Flink blog](https://flink.apache.org/blog/) - Release announcements, design notes, and ecosystem updates.
- [Flink State Backends documentation](https://nightlies.apache.org/flink/flink-docs-stable/docs/ops/state/state_backends/) - How RocksDB and HashMap state backends work, including checkpoint storage to S3.

## Contributing

Contributions are very welcome. Read the [contribution guidelines](CONTRIBUTING.md) first, then open a pull request.

This list aims for **quality over quantity** — entries should be actively useful (working code, clear documentation, demonstrated usage). Entries that haven't seen a commit or release in 24+ months may be moved to an archive section.


# Learning Goals

The main goal of JobFlow is to understand the engineering problems
behind reliable asynchronous job processing.

By the end of the project, I want to be able to explain and demonstrate:

## Queues

- Producer and consumer architecture
- Queue lifecycle
- Queue depth
- Polling
- Queue backends

## Reliability

- Retries
- Exponential backoff
- Jitter
- Dead Letter Queues
- Visibility timeouts

## Concurrency

- Race conditions
- Database locks
- Atomic job acquisition
- PostgreSQL `SKIP LOCKED`

## Delivery Guarantees

- At-most-once
- At-least-once
- Exactly-once
- Idempotency

## Workers

- Worker lifecycle
- Heartbeats
- Crash recovery
- Graceful shutdown

## Scheduling

- Delayed jobs
- Scheduled jobs
- Priority queues
- Queue starvation

## Observability

- Metrics
- Queue latency
- Processing latency
- Throughput
- Prometheus
- Grafana

## Performance

- Load testing
- Benchmarking
- Horizontal scaling
- PHP vs Go workers

## Infrastructure

- Docker
- Kubernetes
- Deployments
- Health checks
- Horizontal Pod Autoscaling
- Event-driven autoscaling
- KEDA
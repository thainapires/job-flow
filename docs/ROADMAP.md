# JobFlow — Roadmap

This roadmap tracks the planned evolution of JobFlow.

The project intentionally starts with a minimal implementation. New abstractions, infrastructure, and technologies are introduced only when they solve a problem that has been explored or reproduced during development.

> This roadmap is expected to evolve as the project progresses.

---

## Phase 1 — Foundations

- [ ] Bootstrap Laravel development environment
- [ ] Configure PostgreSQL
- [ ] Configure Docker
- [ ] Set up testing, formatting, and CI
- [ ] Implement the initial job model
- [ ] Create the job API
- [ ] Build the first database-backed worker
- [ ] Introduce job handlers

**Goal:** understand the fundamental mechanics behind producers, queues, consumers, workers, and job lifecycles.

---

## Phase 2 — Reliability

- [ ] Handle job failures
- [ ] Implement retries
- [ ] Add exponential backoff
- [ ] Add retry jitter
- [ ] Introduce Dead Letter Queues
- [ ] Support manual job replay

**Goal:** understand how asynchronous systems behave when operations fail and how reliable processing can be designed.

---

## Phase 3 — Concurrency

- [ ] Run multiple workers
- [ ] Reproduce duplicate job execution
- [ ] Investigate race conditions
- [ ] Implement atomic job acquisition
- [ ] Introduce database locking
- [ ] Explore idempotency
- [ ] Study delivery guarantees

**Goal:** understand the problems introduced by concurrent consumers and how duplicate processing can be prevented or safely handled.

---

## Phase 4 — Queue Evolution

- [ ] Introduce Redis
- [ ] Implement priority queues
- [ ] Reproduce queue starvation
- [ ] Explore weighted queue consumption
- [ ] Support delayed and scheduled jobs

**Goal:** evolve the queue architecture based on limitations discovered in the initial PostgreSQL-backed implementation.

---

## Phase 5 — Worker Reliability

- [ ] Track worker heartbeats
- [ ] Detect unavailable workers
- [ ] Reproduce worker crashes
- [ ] Detect abandoned jobs
- [ ] Implement visibility timeout
- [ ] Recover abandoned jobs
- [ ] Implement graceful shutdown

**Goal:** understand worker lifecycle management and recover safely from unexpected process failures.

---

## Phase 6 — Observability

- [ ] Define job processing metrics
- [ ] Measure queue depth
- [ ] Measure queue waiting time
- [ ] Measure processing latency
- [ ] Expose Prometheus metrics
- [ ] Build Grafana dashboards

**Goal:** make the internal behavior and health of JobFlow observable.

---

## Phase 7 — Performance

- [ ] Build load testing tools
- [ ] Test different queue sizes
- [ ] Test different worker counts
- [ ] Measure throughput and resource usage
- [ ] Implement a Go worker
- [ ] Benchmark PHP and Go workers

**Goal:** understand how worker count, runtime, and architecture affect throughput and resource consumption.

---

## Phase 8 — Infrastructure & Scaling

- [ ] Containerize the complete system
- [ ] Deploy JobFlow to Kubernetes
- [ ] Configure liveness and readiness checks
- [ ] Explore horizontal worker scaling
- [ ] Configure Horizontal Pod Autoscaling
- [ ] Explore queue-depth-based scaling
- [ ] Introduce KEDA
- [ ] Run an autoscaling experiment

**Goal:** understand how worker-based systems can be deployed, managed, and scaled dynamically.

---

## Phase 9 — Dashboard

- [ ] Build system overview
- [ ] Add job monitoring
- [ ] Add queue monitoring
- [ ] Add worker monitoring
- [ ] Add Dead Letter Queue management
- [ ] Display system metrics

**Goal:** provide a visual interface for observing and interacting with the system.

---

## Phase 10 — Final Study

- [ ] Review learning logs
- [ ] Review architecture decisions
- [ ] Consolidate benchmark results
- [ ] Document architecture evolution
- [ ] Create the final project case study
- [ ] Prepare final diagrams and visual evidence

**Goal:** consolidate the engineering lessons learned throughout the project.
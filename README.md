# Flame: Distributed Analytics Engine

Flame is a simplified distributed analytics engine inspired by Apache Spark, designed to handle large datasets across multiple nodes. Built to support fundamental operations and leveraging a key-value store, Flame facilitates efficient data processing and parallel computation.

## Overview

Flame is capable of:
- Handling large datasets across distributed nodes.
- Performing operations such as flatMap, fold, and join on these datasets.
- Using key-value store tables to manage normal RDDs and PairRDDs.
- Supporting basic operations essential for analytics tasks.

## Requirements

- Implement operations like `flatMap`, `fold`, `join`, any many more.
- Utilize a key-value store to manage datasets.
- Coordinate jobs via a coordinator node and multiple worker nodes.
- Handle job submission via HTTP requests.
- Ensure parallelism by distributing work evenly across workers.
- Extend `FlameContext`, `FlameRDD`, and `FlamePairRDD` interfaces with additional methods.

## Components
- **Coordinator**: Manages job execution and worker nodes.
- **Worker**: Executes tasks assigned by the coordinator.
- **FlameContext**: Interface for job execution context.
- **FlameRDD**: Interface for operations on regular RDDs.
- **FlamePairRDD**: Interface for operations on key-value pairs.

# Compute layout

| Workload | Placement | Budget | Reason |
|---|---|---:|---|
| Motor control | Embedded | 1 ms | Deterministic low-latency control loop |
| Obstacle detection | Edge | 100 ms | Keep sensor-to-brake latency local |
| Pedestrian recognition | Edge AI | 100 ms | Avoid streaming raw camera frames over LTE |
| Global route planning | Cloud | 1~5 s | Non-critical map-level computation |
| Delivery photo upload | Cloud | Minutes | Event-driven workload |
| Log aggregation | Cloud | 1 min~1 h | Batch analysis is sufficient |

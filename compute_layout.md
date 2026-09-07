# Compute layout

| Workload | Placement | Reason |
|---|---|---|
| Motor control | Embedded | Deterministic low-latency control loop |
| Obstacle detection | Edge | Keep sensor-to-brake latency local |
| Pedestrian recognition | Edge AI | Avoid streaming raw camera frames over LTE |
| Global route planning | Cloud | Non-critical map-level computation |
| Delivery photo upload | Cloud | Event-driven workload |
| Log aggregation | Cloud | Batch analysis is sufficient |

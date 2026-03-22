# NVIDIA Benchmark Results

**BlackRoad Pi Cluster vs NVIDIA Hardware**

## Results

| Metric | BlackRoad (Hailo-8) | NVIDIA (A100) | Advantage |
|--------|-------------------|---------------|-----------|
| YOLOv8s FPS/Watt | 64 | 4 | 16x |
| 5-Year TCO | $2,133 | $67,102 | 31x (97%) |
| Concurrent containers | 160 | 0 | Total |
| Fault tolerance | 75% on single failure | 0% | Total |
| Total cluster cost | $1,200 | $15,000+ | 12.5x |
| Power draw | ~50W | ~300W | 6x |

## 8 Experiments

1. Power efficiency (FPS/Watt)
2. Cost efficiency (inference/dollar)
3. Concurrent workloads (186 containers + 4 DBs + 4 Ollama + 2 Hailo)
4. Distributed inference
5. Fault tolerance (75% capacity on single node failure)
6. Total cost of ownership (5-year)
7. Real-time edge AI
8. LLM inference

## BlackRoad Wins

Power efficiency, cost, TCO, versatility, edge deployment, fault tolerance, GPIO access.

## NVIDIA Wins

Raw throughput, training, large models, FP16/FP32 compute.

Benchmark script: `~/run-nvidia-benchmark.sh`

→ [Hardware/Hailo-8](../../../hardware/hailo-8/)
→ [Vendor/NVIDIA](../../../vendor/nvidia/)
→ [Illusion of Complexity](../illusion-of-complexity/)

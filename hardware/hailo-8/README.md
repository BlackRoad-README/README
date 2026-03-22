# Hailo-8 Neural Processing Unit

2 units across Cecilia + Octavia = 52 TOPS combined.

| Spec | Value |
|------|-------|
| TOPS per unit | 26 |
| Total fleet TOPS | 52 |
| Power | ~10W per unit |
| Interface | PCIe M.2 |
| Nodes | Cecilia (.96), Octavia (.101) |

## Benchmarks

| Model | FPS | FPS/Watt |
|-------|-----|----------|
| ResNet50 | 1,360 | 136 |
| YOLOv5s | 122 | 12.2 |

## Pre-compiled HEF Models (20+)

yolov5m, yolov5s, yolov8m, yolov8s, yolov11, resnet_v1_50, resnet_v2_18, face_detection, pose_estimation, semantic_segmentation, instance_segmentation, depth_estimation, and more.

## vs NVIDIA

| Metric | BlackRoad (Hailo-8) | NVIDIA (A100) |
|--------|-------------------|---------------|
| FPS/Watt | 64 | 4 |
| 5-Year TCO | $2,133 | $67,102 |
| Concurrent containers | 160 | 0 |

→ [Cecilia Hailo](../../infrastructure/fleet/cecilia/hailo/)
→ [Octavia Hailo](../../infrastructure/fleet/octavia/hailo/)
→ [NVIDIA benchmarks](../../research/papers/nvidia-benchmarks/)
→ [Vendor/NVIDIA](../../vendor/nvidia/)

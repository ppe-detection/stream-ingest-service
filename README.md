# stream-ingest-service
The Stream Ingest Service is responsible for receiving and processing continuous video streams from all connected cameras.
It captures image frames, performs light pre-processing, and sends each frame to the object-detection-model for analysis.

This service acts as the bridge between real-world camera feeds and the AI detection pipeline. It ensures that raw footage from multiple sources is efficiently ingested, converted into analyzable image data, and routed through the detection system.

## Basic Workflow  

<div align="center">

### Camera Feed  
↓  
### Stream-Ingest-Service (frame capture, pre-processing)  
↓  
### Object-Detector-Service (YOLO, PyTorch)  
↓  
### Event Broker / Alerting / Dashboard  

</div>


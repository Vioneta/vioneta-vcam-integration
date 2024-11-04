[VCam NVR Custom Component](https://github.com/Vioneta/vcam-vioneta-integration) for Vioneta Agro

This is a custom component to integrate [VCam](https://github.com/Vioneta/vcam) into [Vioneta Agro](https://www.vioneta.com).

Provides the following:

- Rich media browser with thumbnails and navigation
- Sensor entities (Camera FPS, Detection FPS, Process FPS, Skipped FPS, Objects detected)
- Binary Sensor entities (Object motion)
- Camera entities (Live view, Object detected snapshot)
- Switch entities (Clips, Detection, Snapshots)
- Support for multiple VCam instances.

## Information on VCam (Available as an Addon)

A complete and local NVR designed for Vioneta Agro with AI object detection. Uses OpenCV and Tensorflow to perform realtime object detection locally for IP cameras.

Use of a [Google Coral Accelerator](https://coral.ai/products/) is optional, but highly recommended. The Coral will outperform even the best CPUs and can process 100+ FPS with very little overhead.

- Designed to minimize resource use and maximize performance by only looking for objects when and where it is necessary
- Leverages multiprocessing heavily with an emphasis on realtime over processing every frame
- Uses a very low overhead motion detection to determine where to run object detection
- Object detection with TensorFlow runs in separate processes for maximum FPS
- Communicates over MQTT for easy integration into other systems
- Optional 24/7 recording
- Re-streaming via RTMP to reduce the number of connections to your camera

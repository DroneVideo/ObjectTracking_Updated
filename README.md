# SampleSolution

Link to [Setup](https://github.com/DroneVideo/docs/blob/gh-pages/setup.md")

## Build


```shell
cd autodrone-openvino
mkdir build
cd build
cmake ..
make
mkdir FP32
```

## Run demo

! First, move nanodet openvino model files (.bin .xml .mapping) to the FP32 folder. Then run these commands:

### Webcam

```shell
./nanodet_demo
```

### Inference images

```shell
./nanodet_demo mode=1 IMAGE_FOLDER/*.jpg
```

### Inference video

```shell
./nanodet_demo mode=2 VIDEO_PATH
```

### Benchmark

```shell
./nanodet_demo mode=3 path=0
```

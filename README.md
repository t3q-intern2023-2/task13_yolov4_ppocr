# yolov4_ppocr
yolov4_darknet + pp_ocr

About Darknet https://github.com/AlexeyAB/darknet

About ppocr https://github.com/PaddlePaddle/PaddleOCR
## Algorithm
Input Video -> Detect License plate -> Recognize License plate  

## Download pretrained weight
.weight https://github.com/Dodant/anpr-with-yolo-v4

## Requirements
yolov4_darknet, ppocr, opencv

## usage(test)
```
python app.py --input video.mp4 --dont_show
```

```json
[
    {
        "frame_name": "frame_0000.jpg",
        "detected_text": "6202 ",
        "center_x": 618,
        "center_y": 638,
        "width": 78,
        "height": 18
    },
    {
        "frame_name": "frame_0000.jpg",
        "detected_text": "1남거 ",
        "center_x": 969,
        "center_y": 630,
        "width": 92,
        "height": 28
    },
    {
        "frame_name": "frame_0000.jpg",
        "detected_text": "1남거 9378 ",
        "center_x": 969,
        "center_y": 630,
        "width": 92,
        "height": 28
    }
	]
```

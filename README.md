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
- **test image : 정지되어 있는 주차장**
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5190595a-ecc4-47d5-b743-29a0eddd6e68/Untitled.jpeg)
    

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/72047325-1eb9-4d06-998b-c164fa08b9f6/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c6396ec6-b8f6-4dd4-8faa-590de784f08a/Untitled.jpeg)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/759893c9-6adb-46ff-90c2-a34d659606ed/Untitled.jpeg)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/77da6a43-da5a-4320-9941-07afc1c9e23f/Untitled.jpeg)

## 결과물

- **출력 예시**

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f0c423be-573a-4da7-a2f9-87b32fca8181/Untitled.png)

- **프레임 별 이미지 (60프레임 기준)**

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7215a5b5-7bd6-4ec3-b191-3f37f01b0af5/Untitled.jpeg)

- **License plate 사진 (Class: license plate가 탐지 되었을 때)**

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/dc28f0ea-efd5-4e43-9620-a4232b039dce/Untitled.jpeg)

- **frame별  BBox coordinates값 및 Detected_text값이 저장된 json 파일**
- [
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

# Footfallcam_Test
  The Footfall cam first round interview question :
  ![image](https://github.com/qianfu1999/Footfallcam_Test/assets/90602872/3eae763b-26d5-4c4f-abd1-d5ac1f43fe5c)

The task is listed belos:
![image](https://github.com/qianfu1999/Footfallcam_Test/assets/90602872/e6263d41-0504-41d9-8e8a-effbe20e48b1)


Solution
-------------------------------------------------------------------------------------------------------------------
1. Run preprocessing.ipynb to get the frame image of the sample video.
2. Given the label name of some selected image. The label has 2 classes which is target and nametag. The label is using a website call makesense.ai to label the classes. Website is put in here (https://www.makesense.ai/)
3. Training the model with the github yolov5 opensource . The website(https://github.com/ultralytics/yolov5/blob/master/README.md) . For the detail can see the colab notebook .ipynb in the location Footfallcam_Test/Model/
4. The training result is shown below.
![image](https://github.com/qianfu1999/Footfallcam_Test/assets/90602872/6e71b677-b350-4f2f-8167-6b41f7b09a39)
5. Save the model and run a detection to the video. The file location is store at FootFallCam_Test/result
6. The detection will provide a drawing rectangle with point out the target and nametag. In the last it will generate an csv output for the coordinate information and the detail list below.
![image](https://github.com/qianfu1999/Footfallcam_Test/assets/90602872/8cfa1af7-7542-49e8-8ca1-f10872b6b67f)


Problem & Future Work
-------------------------------------------------------------------------------------------------------------------
1. The system seem like to detect the person and nametag only.
2. However the video can detect the target and nametag , but there will have another distruction make system wrong recognize such as recognize the pocket to nametag, the person who wear black suit will also wrongly recognize.

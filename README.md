# opencv_dnn_android
准备：
线下载android版本的OpenCV并解压：
https://github.com/opencv/opencv/releases 

## 1. 创建空的android项目

## 2. 增加OpenCV依赖
2.1 选择File - Net - Import module，然后选择OpenCV SDK中的 SDK/java代码路径，按照默认导入即可
2.2 选择file - Project Structure， 点击的app一项，看右边选项，点击Dependencies，选择旁边"+"好，选“Module dependency”，然后选自己下载的OpenCVLibrary版本

## 3.修改参数
打开项目的build.gradle喝OpenCVLibrary的build.gradle文件。根据自己的测试手机参数修改compileSdkVersion和buildToolsVersion，然后点绿色锤子重新构建项目。

## 4.放置模型文件
把训练好的MobileNet_deploy.prototxt和.caffemodel放到app/build/intermediates/assets/debud文件夹下面，点击绿色锤子重新构建项目


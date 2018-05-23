# face_recognition_demo

![](https://img.shields.io/badge/python-3.6-blue.svg)
![](https://img.shields.io/badge/build-passing-brightgreen.svg)  
this demo includes three notebook.  
windows 10, python 3.6.  
## software
before run this demo,you'd better to install these lib  
1. [Anaconda3 for windows](https://www.anaconda.com/download)  
    download [Anaconda3-5.1.0-Windows-x86_64.exe](https://repo.anaconda.com/archive/Anaconda3-5.1.0-Windows-x86_64.exe)  
    just install
2. [TensorFlow](https://tensorflow.google.cn/)  
    In cmd  
    run <code>conda create -n tensorflow pip python=3.6</code>  
    run <code>activate tensorflow</code>  
    If there is no gpu in your laptop.  
    run <code>pip install --ignore-installed --upgrade tensorflow </code>  
    If there is gpu in your laptop.  
    run <code>pip install --ignore-installed --upgrade tensorflow-gpu </code>
3. [Keras](https://keras.io/)  
    run <code>sudo pip install keras</code>
4. [opencv for python](https://www.opencv.org/)   
    In cmd just run <code>conda install -c conda-forge opencv</code>
5. install jupyter notebook,numpy,matlibplot, hdf5 and someother lib in env(tensorflow)

## Hardware
you can use your laptop camera or plugin a usb camera,  
if no camera, two videos are necessary.  
one includes your face, other one includes some faces except you.  
I have not try video,you may experience by yourself.
## Code Instruction
you should run the files as below sequence:  
1. [face_recogniton_get_data.ipynb](https://github.com/JarvisXing/face_recognition_demo/blob/master/face_recogniton_get_data.ipynb)  
you can get face data with this file from camera or video.
2. [face_recogniton_train_model.ipynb](https://github.com/JarvisXing/face_recognition_demo/blob/master/face_recogniton_train_model.ipynb)  
you can use this file to train a simple deeplearning model.
3. [face_recognition.ipynb](https://github.com/JarvisXing/face_recognition_demo/blob/master/face_recognition.ipynb)  
now you can use this file distinguish your face from other faces.  

***note:*** you have to change <code>cascade_path</code> by yourself.  
## File structure
>WORKSPACE_DIR(.)
>>PRJ_NAME.ipynb  
>>PRJ_NAME_get_data.ipynb  
>>PRJ_NAME_train_model.ipynb   
>>DATA_PATH(datasets)  
>>>PRJ_NAME  
>>>>TRAIN_DIR(train)  
>>>>>CLASS_1_DIR  
>>>>>CLASS_n_DIR  

>>>>VALIDATION_DIR(validation)  
>>>>>CLASS_1_DIR  
>>>>>CLASS_n_DIR  

>>>>TEST_DIR(test)
>>>>>CLASS_1_DIR  
>>>>>CLASS_n_DIR  

>>MODEL_PATH(models)  
>>>PRJ_NAME  

>>Image_PATH(images)  
>>>PRJ_NAME  

>>LOG_PATH(logs)  
>>>PRJ_NAME  

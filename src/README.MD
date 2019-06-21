
# Tengine APP - Image Classification

## Preface

- In this project, we use Tengine to run the TensorFlow Mobilenet.v1 model to predict image.

- This App supports for real-time camera image classification. It is built on previous project: [Tengine APP](https://github.com/OAID/Tengine-app/tree/master/android/classification)

- The App processes the real time image camera preview and gives the predict results.


## Installation and Instruction
 

- You can use Android Studio to install and test the project. Make sure your test devices are based on Armv8.

- You need to install adb in your library. After installation. You can always use the following command to see the list of your phone or emulator available for test. 

```
adb advices
```

- Then push frozen_mobilenet_v1_224.pb and synset_words.txt in your phone.

```
adb push frozen_mobilenet_v1_224.pb /data/local/tmp/
adb push synset_words.txt /data/local/tmp/
```

- Make sure the model and labels are in the phone.

```
adb shell ls /data/local/tmp
```

- Go to Android Studio, sync and build the project. 

- Run the project and make sure the App is given permission of using camera and SD card from your phone.

## For using other models

## Features and Demo

### Adjust the number of CPUs to run (default using 4 CPUs)

### Ability to switch between CPU (default) and GPU

### Show inference time

### Ability to use Float (default) and Quantized model

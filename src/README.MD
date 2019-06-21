-
# Tengine APP - Image Classification

## Preface

- In this App, we use Tengine to run the mobilenet.v1 model.

- This project supports for real-time camera image classification. It is built on previous project: [Tengine APP](https://github.com/OAID/Tengine-app/tree/master/android/classification)

## Installation and Instruction
 

- You can use Android Studio to install and test the project.

- You need to install adb in your library. After installation. You can always see the list of your phone or emulator available for test. 

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

## Demo

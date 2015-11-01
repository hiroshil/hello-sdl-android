# Description
This project is a simply "Hello World" Android Studio and SDL application. When it runs on an Android device (API 18 or higher) an OpenGL rendered square will rotate.

## Instructions
1) Download SDL2 and GLM libraries.
2) Download Android Studio and the Android NDK from Google's Android website. This project was tested with android-ndk-r10e. 
3) Export or edit the ".bashrc" file and add the line ```export PATH=$PATH:/home/<usr>/Android/android-ndk-r10e```
4) Boot up Android Studio and download API 18 SDK and possibly other stuff.
5) Import this project with the selection "Import other Eclipse or Gradle projects ..."
6) Navigate to the app/src/main/jni directory of this project and setup the symbolic links to wherever SDL and GLM are on your computer.
	```ln -s /path/to/SDL SDL2```
	```ln -s /path/to/GLM glm```
7) Run ```ndk-build``` from the app/src/main/jni directory of this project to build the app. The project was tested with a real Android device (don't trust the emulator!).


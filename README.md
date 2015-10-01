# android-gif-drawable-eclipse-sample
Sample Eclipse project using android-gif-drawable library made with help of user [nuoyan2](https://github.com/nuoyan2).
It shows where to place files taken from AAR and source files inside Eclipse project structure. Latest archives can be downloaded here: [latest release](https://github.com/koral--/android-gif-drawable/releases/latest).
### Steps to include library in Eclipse project:
* copy `pl` folder from sources jar inside `src` folder of the Eclipse project
* copy all contents of `jni` folder from AAR into `libs` folder of the project
* copy `proguard.txt` from AAR into root folder of the project and rename it to `proguard-project.txt` (required only if proguard will be used)
* copy `res/values/values.xml` from AAR into `res/values` folder of the project
* install android support library, copy `android-support-annotations.jar` into `libs` folder of the project and add it to the build path
* add imports for `R` class in files when it is missing (choose `R` from your package, not `android` one)
 
#### Additional step for versions < 1.1.10
* in `GifInfoHandle.java` replace `BuildConfig.NATIVE_LIBRARY_NAME` with the `"pl_droidsonroids_gif"`

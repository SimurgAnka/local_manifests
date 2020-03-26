# local_manifests
Manifests 
for 
Building A5
[Exynos7580]
 
===========
 
Getting started
 
===========
 
---------------
 
Make a dir for DEVICE_TREE.
```
mkdir *NAME      
(Replace *NAME with your choice)
```
Enter the dir.
```
cd *NAME
```
To initialize your local repository using the Device trees, use a command like this:
```
repo init -u https://github.com/SimurgAnka/local_manifests.git -b nx-10.0
```
Then to sync up:
```
repo sync
```
Now, move the device dirs to the respective dirs in ANDROID SOURCE DIR.
```
(to the same dirs as in the DEVICE_TREE dirs)
 
For eg : DEVICE_TREE/device/samsung/a5xelte ~ ANDROID_SOURCE_DIR/device/samsung/a5xelte
```
 
OR 
 
Simply copy the content of the default.xml into the dir ANDROID_SOURCE_TREE/.repo/local_manifests/local_manifests.xml
```
(will have to create a dir and a file in the .repo dir of the ANDROID_SOURCE_DIR)
(local_manifests > dir && local_manifests.xml > file, content to be copied in the xml file)
```
Then to sync up:
```
repo sync
```
 

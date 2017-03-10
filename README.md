# ResProguardInGradle
when run gradle assemble task ,auto do resource proguard and sign.

#Usage:

1、download resourceproguard.zip and extract it to your_android_studio_project/app/doc

2、input "apply from: './doc/resourceproguard/resourceproguard.gradle'" to your build.gradle in your_android_studio_project/app. 

3、run your app or gradle assembleDebug or gradle assembleRelease ,this gradle script will auto do resource proguard , 7zip , zipalign and sign.

4、detect signature config and scheme version automatically, support APK Signature Scheme v2.

#Other:

1、the resource proguard engine use [AndResGuard](https://github.com/shwenzhang/AndResGuard)

2、you can config the resource proguard in your_android_studio_project/app/doc/resourceproguard/config.xml

3、if you have flavor in your build.gradle ,please modify your_android_studio_project/app/doc/resourceproguard/resourceproguard.gradle

for example:
```java
//variant
def targetVariants = ["googleRelease"];
```
4、this script is only test in mac os，if you use linux or window you should replace the [SevenZip-1.1.16-osx-x86_64.exe](https://github.com/shwenzhang/AndResGuard/tree/master/SevenZip/executable)

5、you can clone this demo repo and enjoy it!

#Contact me:

Blog:http://www.masonliu.com

Email:MasonLiuChn@gmail.com

#License:
    Copyright 2017 MasonLiu, Inc.

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.



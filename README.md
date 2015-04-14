# FbSimpleLib
此為fb simple 官方範例。環境為android studio。<br />
如果需要用到，必須在fb My apps https://developers.facebook.com/apps/ 裡新增APP。<br />
修改所有App ID 此檔為1823693194522353<br />
並且Namespace需要修改成自己的。<br />
在本檔案已經導入了simple fb 以及fb v3 sdk。<br />
<br />
<br />
<br />
若要自己重新導入，請在gradle.properties 放入<br />
<b>*ANDROID_BUILD_SDK_VERSION=19*<br />
<b>*ANDROID_BUILD_TOOLS_VERSION=19.1.0*<br />
<b>*ANDROID_BUILD_MIN_SDK_VERSION=15*<br />
<b>*ANDROID_BUILD_TARGET_SDK_VERSION=19*<br />

在project build.gradle 的dependencies 裡如下所示<br />
classpath 'com.android.tools.build:gradle:1.1.3'<br />


在app build.gradle 的dependencies 裡如下所示<br />
dependencies {<br />
    compile fileTree(include: ['*.jar'], dir: 'libs')<br />
    compile 'com.android.support:appcompat-v7:22.0.0'<br />
    <b>compile project(':facebook')<b><br />
    <b>compile project(':Simple Facebook')<b><br />
}<br />



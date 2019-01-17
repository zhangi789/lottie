
# Lottile
Lottie是Android的一个移动库，它可以解析Adobe After Effects动画导出为json格式并在移动端呈现!。其主要特性有：

1. AS>=3.1.2 
2. Lottie原框架基于androidx开发,提取修改成通用方式
3. 使用方式和implementation 'com.airbnb.android:lottie:$lottieVersion' 一致
4. [动画展示](https://github.com/airbnb/lottie-android) -动画展示 </br>

## 集成AS   版本>=3.1.2 

> Step 1.先在 build.gradle(Project:XXXX) 的 repositories 添加:

	allprojects {
		repositories {
			...
			maven { url "https://jitpack.io" }
		}
	}
> Step 2. 然后在 build.gradle(Module:app) 的 dependencies 添加:

	dependencies {
	       //基础工具库
           implementation 'com.github.zhangi789:lottie:1.8'
	}

## Usage
-----
```xml
 <com.airbnb.lottie.LottieAnimationView
        android:id="@+id/animationView"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        airbnb:lottie_autoPlay="true"
        airbnb:lottie_fileName="LottieLogo2.json"
        airbnb:lottie_imageAssetsFolder="images"
        airbnb:lottie_loop="true" />

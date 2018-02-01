# UCrop

改写大神的Ucrop库，主要是获取裁剪框的RectF，会根据大神的更新,原库地址https://github.com/Yalantis/uCrop，
详细的请查看

### Step 1. Add the JitPack repository to your build file

Add it in your root build.gradle at the end of repositories:
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}

### Step 2. Add the dependency

dependencies {
	        compile 'com.github.wzgl5533:UCrop:1.0.1'
	}

## 本库增加的部分

### 1、增加获取裁剪区域的RectF

在onActivityResult中

RectF rectF = UCrop.getCropView(result);

其中result是返回的intent对象

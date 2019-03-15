# maven
我的maven仓库

### 引用方式

**1.在项目的build.gradle当中添加maven地址**

allprojects {

    repositories {
    
        google()
        
        jcenter()
        
        //添加
        
        maven { url 'https://raw.githubusercontent.com/huangbei1990/maven/master/' }
    }
    
}


**2.在模块的build.gradle当中添加需要引用的库**

例如添加permission库

dependencies {

    ...
    
    implementation 'hbuilder.android.utils:permission:1.1'
    
}

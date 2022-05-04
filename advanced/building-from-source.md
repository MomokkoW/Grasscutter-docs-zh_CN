# 🏗 Building from source

首先，下载适宜的JDK版本。

{% hint style="info" %}
对于Stable分支，需要JDK8（[在此下载](https://mirrors.huaweicloud.com/java/jdk/8u202-b08/)）；

对于Development分支，需要JDK17（[在此下载](https://mirrors.tuna.tsinghua.edu.cn/Adoptium/17/jdk/)）。
{% endhint %}

其次，使用`git clone https://github.com/grasscutters/grasscutter.git`获取源代码或者直接下载**（不推荐）**

{% hint style="info" %}
如果使用Development分支，需额外进行`git checkout -b development origin/development`操作。

如果GitHub访问速度过慢，可以尝试使用镜像（e.g. githubfast.com）
{% endhint %}

在命令行下运行

```shell
cd Grasscutter

# 对于Windows用户（Powershell，MinGW，Cygwin）
.\gradlew.bat #设置环境
.\gradlew jar #编译

# 对于Linux用户
chmod +x gradlew #添加可执行标记
.\gradlew jar #编译
```

{% hint style="info" %}
对于旧版的Grasscutter，编译结果为`grasscutter.jar`。

如果你使用Windows CMD，请**不要**加入`./`前缀。
{% endhint %}
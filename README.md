>Android studio 的编译脚本有诸多功能，更多的利用这些功能，会让IDE变成你的开发利器。

## 利用Gradle获取git提交的内容
Android每一次打包，总需要手动改正编译中的versionCode，因为新版本总是要比上一版大的，这就会非常麻烦。git中的commit次数是一个不错的idea。这样就会让versionCode肯定会大于上个版本，不过增长过快也算是一个不怎么友好的地方。

## 利用Gradle获取properties配置文件
java代码也可以，但是gradle也是可以获取properties配置文件内容的。同样我们在version.properties中写了一个版本名称。用Gradle文件来实现读取。

## 利用Gradle对文件进行操作
在Android studio的build文件夹下是编译所产生的文件，对文件命名是一个仙儿易见得需求。

## 从控制台录入签名和从环境变量中获取签名信息
对于扁平化的公司而言，开发聊聊几个人，但是如果企业规模较大，开发团队比较大，处于安全考虑，不希望把应用的签名信息直接写到gradle中，这里有两周方法，一中是从环境变量中获取，另外一种是从控制台录入。

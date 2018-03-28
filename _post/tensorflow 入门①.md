#<cenert> tensorflow 入门（一）</center>
## windows下 环境配置
> mac 和 Ubantu 下使用 anaconda安装 一次成功 就不描述了

-----
 #####网上流传的安装方式：
 1. 安装Anaconda
 2. 安装Tensorflow
 
> 相关的链接：
> https://blog.csdn.net/u010858605/article/details/64128466/

---
####遇到的问题
* windows 32位系统 tensorflow 无法 成功安装， 提示 XXXXXXXX 
* 提示 CondaHTTPError: HTTP 000 CONNECTION FAILED for url  等信息
* import tensorflow 时提示 can't load module
* import tensorflow 时提示 can‘t load DLL

####对应的解决
* 老老实实更新系统吧 老铁
* 因为是公司环境 部分端口被限制了， 请使用VPN
* 可能是 python 版本不支持， 也可能是有其他环境没有装好， 我是第二次使用 pip 安装后就可以使用了
* 可能是 python 版本不支持， 晚上教程默认是使用 python=3.5 实际上安装的是 python 3.5.5 该版本不支持， 我安装3.5.4后能正常运行

---
#### 入门惯例 附上 hello world

``` python
import tensorflow as tf
hello = tf.constant('hello, world')
sess = Session()
print(sess.run(hello))


```
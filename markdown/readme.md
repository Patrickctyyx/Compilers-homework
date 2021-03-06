# Markdown 解释器

原创作者：岐山凤鸣

下面介绍一下用法。

# 安装

前提：电脑上已经安装好了Python3，并加入了环境变量。

Git: https://github.com/Ecohnoch/Compilers-homework/tree/master/markdown

或者百度网盘：https://pan.baidu.com/s/1nvwSFgt

下载得到markdown文件夹。


# 用法

安装得到的markdown文件夹后，放到一个文件夹路径很清晰的地方。

然后打开命令行提示符(Windows)或者终端(Linux及MacOS)

cd到当前目录下，比如在我电脑上(MacOS), 我把文件夹放到了桌面上:

```
$ cd desktop/markdown
```

然后输入如下命令即可：

```
$ python3 markdown.py 想要解析的markdown文档名 想要输出的html文档名
```

注： 想要解析的markdown文档必须放在该目录下

例如里面自带了一个test.md示例，我可以这样：

```
$ python3 markdown.py test.md outputfuck.html
```

然后在output文件夹中就可以发现输出的html文档，用浏览器打开即可。

注：如果需要代码高亮功能，则output文件夹中的两个非html也需要跟着html一起被移动。

# 当前版本

更新： 2017年6月9日：

当前版本实现了markdown的一部分用法。

## 正常段落

正常的段落，要注意【两次回车】是换行，不支持一行行换行

例如：

```
This is a normal paragraph.

This is the second paragraph.

这是第三段
```

## 六种标题

包括如下六种标题：

---

# 大标题
## 二号标题
### 三号标题
#### 四号标题
##### 五号标题
###### 六号标题

写法分别为：

几个#+空格+标题名。

例如：

```
### 这是三号标题
```

解析后便是三号标题。
---

## 引用

> 这样的就叫引用

写法为： >+空格+引用文字

例如：

```
> 这样的就叫引用
```

## 列表

* 这样的
* 就叫
* 列表

写法为： *+空格+第x行

例如：

```
* 这样的
* 就叫
* 列表
```

## 分隔线

---

上面这个就是分隔线

写法为： ---或更多的-单独占一行

例如：

```
---

或者：

——-----

都可以
```

## 代码且高亮

```
这样的就叫代码
```

支持高亮：

```
int main(){
	print("This is a test")
}
```

写法为： ```+换行+代码段+换行+```

例如：

```

```
test the codes
```

```

## 字体加粗

在任意的文字两边加上**，均可让其文字加粗，例如：

```
这里有一段**你想加粗**的文字
```

## 文字下划线

在任意想加下划线的地方两边加上++，均可让文字拥有下划线，例如：

```
这里有一段你想加++下划线++的地方
```

## 文字背景色

在任意想加背景色的地方两边加上==，均可让文字拥有背景色，例如：

```
这里有一段你想加==背景色==的地方
```

目前只支持红色。

## 其他

其他用法如：

- 文本加粗
- 文本斜体
- 图片
- 超链接
- 表格

等功能有待更新版本、

祝高考顺利。

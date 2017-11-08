# 使用说明

#### 1. 请先安装 tinify 的依赖库：

```python
python -m pip install tinify
```

#### 2. 申请 tinify key

到 [https://tinypng.com/developers](https://tinypng.com/developers) 申请自己的 key，每个 key 每个月可以压缩 500 个文件。

#### 3. 执行脚本

申请完 key 之后，更新到代码段中的：
```python
tinify.key = "your key" # AppKey
```

然后带参数执行脚本即可。

```
[Usage] compress-with-tinypng.py [filepath]
```

带的第一个参数是必选的，可以是文件，也可以是文件夹。

第二个参数是可选的，自定义 key，如果输入了第三个参数，则优先使用自定义 key

压缩后的文件，默认输出到当前脚本所在目录下的 tinypng 文件夹中，如果要输出到其他位置，可以自行修改脚本实现。

PS：已使用 Python2.7 和 Python3.4 亲测有效，其他 Python 版本如果有异常，请反馈

# docling

## github下载

```bash
git clone https://github.com/jasktim/docling.git
```



## 1、安装库

```bash
# 安装docling
pip install docling

# 安装modelscope
pip install modelscope
```



## 2、使用modelscope下载模型

```bash
# 创建模型存放文件夹
mkdir models
cd models

# 下载docling模型
modelscope download --model ds4sd/docling-models --local_dir ./docling-models

# 下载easyocr模型
modelscope download --model Ceceliachenen/easyocr --local_dir ./easyocr
```



## 3、运行代码

- 修改test.py中两个模型的路径为绝对路径
- 修改待解析的pdf文件路径

```python
python test.py
```

运行代码，即可输出markdown格式的pdf内容
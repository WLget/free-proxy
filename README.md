## 获取免费节点的进阶方法
# 一、来源及优点

1、开发源代码的大佬的github

2、优点：代码部署在服务器上，利用爬虫代码抓取免费节点 ，并在服务器端直接进行测速优选！

# 二、部署在哪里？怎样部署？

1、项目部署在：谷歌Colab Link:https://colab.research.google.com/

2、在Colab上克隆项目仓库

!git clone https://github.com/wzdnzd/aggregator.git

3、安装依赖项

进入目录： 

 %cd aggregator

安装项目所需的 Python 依赖项 ：

!pip install -r requirements.txt
4、运行 collect.py 脚本

!python -u subscribe/collect.py -s 

5、查看结果

!cat /content/aggregator/data/clash.yaml

6、下载结果

from google.colab import files
files.download('/content/aggregator/data/clash.yaml')

注意：共3个文件，根据需要自己更改指令中的文件名！

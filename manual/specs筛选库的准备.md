#### specs 筛选库的准备




#### 下载
推荐直接从specs官网上下载，有如下优点
1. sdf 文件中有specs编号
2. 所有的化合物都是可以购买的。
zinc中specs化合物库没有specs编号。

##### 处理
提取specs编号；



#####
所下载的sdf文件是2D的，建议通过ligprep进行处理。


#####  处理之前需要对sdf文件预处理
ligprep 处理的下载下来的sdf，会丢失编号信息。
SD 没有单独的小分子名称信息只有各种字段。
先通过openbabel将sdf转成mol格式（建议使用命令行）。
因为你的sd是2D的，所以转成mol格式。然后把给每个分子赋予名字。

##### ligprep 处理用于glide筛选


##### 转成mol2格式并split


##### 用prepare_ligand4.py处理成pdbqt文件用于autodock对接

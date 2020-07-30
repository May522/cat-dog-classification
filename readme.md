## 猫狗大战
这是一个对猫狗图像进行分类的项目，其数据集可以在kaggle竞赛网站下载。
[猫狗数据集](https://www.kaggle.com/c/dogs-vs-cats-redux-kernels-edition/data)

### 编程环境:
        操作系统：WIN10
        GPU型号： NVIDIA GeForce 940MX
        cuda: 10.0
        anaconda: 4.8.3
        pytorch: 1.2.0

### 文件结构为：
train
copy
    -train
        -cats
        -dogs
    -val
        -cats
        -dogs
test
数据集预处理.ipynb
模型训练.ipynb
多模型融合.ipynb


### 数据集预处理.ipynb
内容：数据集处理、计算训练集的均值和方差

### 模型训练.ipynb
内容：用alexnet模型、VGG16模型、resnet18、resnet50 进行迁移学习
在测试集上，alexnet模型的准确率达到大约95%，VGG16模型为98%,resnet18约为97%，resnet50约为98%。

### 多模型融合.ipynb
内容：把resnet50、inception-v3、Xception三个模型结合在一起进行训练
在测试集上，该模型准确率到达大约99.6%。

备注：如果自己电脑配置不够，可在云服务器上训练，速度很快。
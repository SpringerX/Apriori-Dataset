# Apriori

## Apriori-Dataset

结课作业数据集 groceries.csv

[分类、聚类weka示例数据集](https://github.com/SpringerX/Weka-Dataset)（此数据集跟结课作业无关）

## 《分布式配置参考教程》

新添加的《分布式配置参考教程》为大家在docker容器中进行Hadoop分布式配置提供参考，该教程可以为大家提供大体的配置思路。

**注意：** 部分细节可能并不适用于Hadoop 3.1.3，主要在于某些xml配置文件的修改，例如但不限于yarn-site.xml，这里可以找对应版本的配置教程加以参考。另外，docker安装参照我提供的另外一个教程就可以，不建议参考这个教程中提供的方法。

**注意：** 建议在Docker上进行Hadoop分布式配置的同学改用版本号为2.7.1的Hadoop（见群文件）

## Apriori算法实现参考

[market-basket-analysis](https://github.com/SpringerX/market-basket-analysis)

## 大作业思路参考

- Hadoop版本变更为2.7.1；

- 可以在多台虚拟机上实现Hadoop分布式配置，也可以找多台计算机组局域网实现，已安装Ubuntu系统（包括云服务器用户）或者Windows是专业版的同学，可以在Docker容器中进行配置 **（推荐）** ，但暂时不考虑提供Windows专业版下的Docker安装参考；

- 因为Windows系统的一些限制，子系统用户安装Docker会有一定的困难，暂时不考虑提供参考教程；

- 参考本项目内教程《Ubuntu 18.04 安装 Docker》，在Ubuntu系统内安装Docker；

- 而后参考《分布式配置参考教程》中的章节3.3.5中的“3.在Docker上安装Ubuntu系统”及以后各小节内容（P13-P20)，在Docker容器中进行Hadoop分布式配置；

- 最后参考《Apriori算法实现参考》进行Apriori算法编程实现，对指定数据集 groceries.csv 进行运算，并得出运算结果；

- 运算结果中我们需要的部分主要在final-output文件夹下（如果参考《Apriori算法实现参考》），请同学们将Apriori算法得出的Rule及其置信度数据截图并保存；

- 记录实验过程中的关键步骤，并撰写实验报告。

## 基本完结

- 祝大家实验&&考试顺利~

- 考试周也要稳住鸭~

# Climate-Change-in-Data-Science
This project is what I am doing for now during my PhD research.

## Methods

### Casual inference

- Casual inference 初识：基础知识框架建立
    
    [Casual inference知识框架](https://www.notion.so/Casual-inference-c9fdbbbe33684c91af4ed1e79e33a6a1?pvs=21)
    
- [大白话谈因果 - 知乎 (zhihu.com)](https://www.zhihu.com/column/c_1408014345809227776)
- 总结到目前为止比较主流的做casual inference的方法，包括理论以及代码，实验
    - 这一节介绍了因果推断的基本概念
        
        [因果推断综述及基础方法介绍（一）](https://zhuanlan.zhihu.com/p/258562953)
        
    - 第二节介绍了一些前沿论文以及应用
        
        [因果推断综述及基础方法介绍（二）](https://zhuanlan.zhihu.com/p/366702128)
        
    - 以下github仓库总结了做因果推断的一些方法论
        
        https://github.com/rguo12/awesome-causality-algorithms
        
        为方便查阅，已将该仓库转载于以下链接
        
        [Awesome Casual inference Algorithms](https://www.notion.so/Awesome-Casual-inference-Algorithms-be23e24b0ddd4b9f810e5b219f8acfad?pvs=21)
        

[主流方法以及代码](https://www.notion.so/aaee008d7673428abee8e30c10f16b44?pvs=21)

- 做文献综述，在主流的方法总结基础上阅读该领域的最新方法与应用，将突破点总结归纳。与上一点一起合并成文献综述
- Literature review

---

---

### Time Series

- ****时间序列预测从入门到精通****

[时间序列预测从入门到精通（一）：基础知识](https://zhuanlan.zhihu.com/p/393594761)

[时间序列预测从入门到精通（二）：传统方法](https://zhuanlan.zhihu.com/p/393644272)

[时间序列预测从入门到精通（三）：深度学习方法](https://zhuanlan.zhihu.com/p/393706324)

- 时间序列分析 （分章节与小点介绍）

[时间序列分析101：序言](https://skywateryang.gitbook.io/timeseriesanalysis101/)

- https://github.com/qingsongedu/awesome-AI-for-time-series-papers
- https://github.com/MaxBenChrist/awesome_time_series_in_python
- https://github.com/cuge1995/awesome-time-series
- https://github.com/datamonday/Time-Series-Analysis-Tutorial : 包括了时间序列的论文以及博客

---

---

## Dataset

### CMIP6数据集：

- Intro:
    
    ***CMIP6，全称为耦合模型比较项目第6阶段（Coupled Model Intercomparison Project Phase 6）***，是气候科学研究中的一个重要项目。该项目旨在对全球气候模型的结果进行比较和评估，从而提高我们对地球气候系统的理解和预测未来气候变化的能力。
    
    CMIP6的主要目标包括：
    
    1. 评估模型对过去、现在和未来气候状态的模拟和预测能力。
    2. 研究和理解气候反馈过程和气候敏感性。
    3. 提供多个未来气候变化的情景路径，以供决策者和政策制定者参考。
    
    CMIP6数据集是一组大型的气候模型输出数据集，包括大量关于气候变量（如温度、降水、风速等）的数据。这些数据既包括过去（通过对历史气候变化的模拟）的数据，也包括未来（通过对不同排放情景下的未来气候变化进行模拟）的数据。
    
    [cmip6 - Home | ESGF-CoG](https://esgf-node.llnl.gov/projects/cmip6/)
    
- 数据下载
    - 在以下网址直接搜索所需数据集（CMIP5 or CMIP6均可）
        
        [Copernicus Climate Data Store |](https://cds.climate.copernicus.eu/cdsapp#!/dataset/projections-cmip6?tab=overview)
        
    - 在以下网址通过索引搜索所需的数据集并下载（globus / wget）
        
        [ESGF MetaGrid](https://aims2.llnl.gov/search)
        
- ArcGIS
    - [Arcpy / Matlab / Arcgis处理CMIP6数据_PeanutbutterBoh的博客-CSDN博客](https://blog.csdn.net/weixin_43637490/article/details/124960959)
    - [使用Arcgis处理CMIP6(netCDF)数据的流程 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/149845115?from_voters_page=true)
- CDO基本操作
    - [CDO简介及常用语法 | ZSYXY Meteorological workshop (yxy-biubiubiu.github.io)](https://yxy-biubiubiu.github.io/2020/06/07/cdo/)
    - [CDO学习2 CDO 入门教程Tutorial - chinagod - 博客园 (cnblogs.com)](https://www.cnblogs.com/jiangleads/p/11146721.html)
    - [CDO入门和使用实践_cdo使用_趴着喝可乐的博客-CSDN博客](https://blog.csdn.net/u011424614/article/details/120696468)
- Xarray基本操作
    - [Xarray 文档](https://docs.xarray.dev/en/stable/index.html)
    - [(182条消息) xarray 使用教程 - 未完待续_可乐要加冰_ice的博客-CSDN博客](https://blog.csdn.net/mihuanchengbao/article/details/126641111)
    - 以下作者将其将数据处理分多章讲解，包括配置环境与Xarray的使用
        - https://www.zhihu.com/column/c_1422150022150877184 Python气象数据处理
- 气候降尺度方法

[降尺度](https://www.notion.so/55b93e7a9e874435b4ecd0c08dfa3dfe?pvs=21)

***统计降尺度 （SD） 技术***

为了提供可靠的数据集并突出统计缩减的敏感性，在分析中使用了三种不同的SD方法（如下所述）与GCM和RCP结合使用。每种技术都使用三个网格化观测数据产品（Daymet版本2.1，Livneh版本1.2和PRISM版本AN81d）来校准方法的准确性。

1. 德尔塔法（DeltaSD） – 一种广泛使用的简单方法，假设变化发生在更大的区域范围内，并且气候变量之间的关系在未来情景中将保持不变。（[Pourmokhtarian等人，2016](https://doi.org/10.1890/15-0745))
2. 等距分位数映射方法 （EDQM） – 这是分位数映射技术的修改版本，用于通过专门针对每月 GCM 输出的偏差校正来解释时间变化。（[李等人，2010](https://doi.org/10.1029/2009JD012882))
3. 分段异步回归方法（PARM） – 与EDQM类似，该方法利用偏置校正技术，但也通过将一系列线拟合到点数据来解决采样变量的随机不规则性，以消除小规模噪声。（[兰赞特等人，2019](https://doi.org/10.1002/joc.6288))

由于SD方法性能特征的可变性，使用这三种SD技术和各种观测数据产品表明，SD方法的选择可以影响产生的气候预测的可变性。

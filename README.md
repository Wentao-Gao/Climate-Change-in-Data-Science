# Climate Change Prediction Using Casual Inference 

因果推断在气候预测中的应用

***Author: Wentao Gao***

***Github: https://github.com/gwt9970161/Climate-Change-in-Data-Science***

This project is what I am doing for now during my PhD research. I will mainly focused on casual network. 根据目前对该项目的了解，需要将因果推断与时间序列相结合，找到在时间段而非单一时间中进行因果推断，并且最终应用在气候预测中，减少对预测的干扰，提高气候预测的准确率，需要了解的知识包括以下几个类别：
   
   - Casual Inference，
   
   - Time Series,

   - NCEP-NCAR Reanalysis 1 data analysis

## Weekly plan:

### Week 1(19/06/2023)
1. 下载并处理netCDF4数据，输出一个包含特定经纬度的CSV格式数据，包括时间，温度，湿度，海平面压力以及我们所需预测的数据—降雨量。
2. 用这个简单的数据进行时间序列分析。包括平稳性检验等。
    - [Time Series data analysis.ipynb](https://colab.research.google.com/drive/1hu2gfUGSKEyGV9r5K6kG7mlPpKVz3aD7#scrollTo=ae4i6KHH211z)
3. 使用一个简单的机器学习模型进行训练以及预测。
    - [RNN Method - Prediction of precipitation.ipynb](https://colab.research.google.com/drive/1JQJJaEqXEAFCjlkjuqsEx0Zn1ykAdDhi#scrollTo=umofRzBWlcsw)
4. 使用一个更好的模型来处理这个预测问题，在这里我选择了LSTM来处理。
    - [LSTM Method - Prediction of Precipitation.ipynb](https://colab.research.google.com/drive/1HE52cH7wIfjQl64MekuAGvopxx2SQtmu#scrollTo=ZlFnxgpCGl1j&uniqifier=1)
5. 看Jiuyong老师给的论文，了解时间序列如何应用在Drought Prediction中。


| Paper | Link | 
| --- | --- | 
| Evaluation of Time Series Models in Simulating Different Monthly Scales of Drought Index for Improving Their Forecast Accuracy | https://ira.lib.polyu.edu.hk/bitstream/10397/96563/1/feart-10-839527.pdf | 
| Estimation of SPEI Meteorological Drought using Machine Learning Algorithms | https://research-repository.griffith.edu.au/bitstream/handle/10072/404189/Gyasi-Agyei483825-Published.pdf?sequence=2 | 
| Prediction of Impending Drought Scenarios Based on Surface and Subsurface Parameters in a Selected Region of Tropical Queensland,Australia | https://www.scirp.org/pdf/jwarp_2021081015095566.pdf | 
| Monthly drought prediction based on ensemble models | https://peerj.com/articles/9853.pdf | Keywords Standardized precipitation index, Equal ensemble drought prediction, Weighted ensemble drought prediction, Conditional ensemble drought prediction, Copulas |
| A novel intelligent deep learning predictive model for meteorological drought forecasting | https://link.springer.com/article/10.1007/s12652-022-03701-7 | 

## Todo list:

- **[Causal networks for climate model evaluation and constrained projections](https://www.nature.com/articles/s41467-020-15195-y/)** 
  - ***[Translation and Summary of the paper](https://www.notion.so/wentao-gao/Causal-networks-for-climate-model-evaluation-and-constrained-projections-1b78b4afe1a24ccca1a57d9d0bf776ec#d2eb67fd9a7a4b3daa3e518e403a51a8)***
  - 用了什么模型
  - 什么评价指标
  - 数据是如何处理的
  - 如何将数据使用模型进行训练与预测的
- CMIP5/6 数据下载并整理成易使用的版本
- [Tigramite – 时间序列数据集的因果推理](https://github.com/jakobrunge/tigramite)

## Toolboxes
***（摘自仓库 [awesome-causality-algorithms](https://github.com/rguo12/awesome-causality-algorithms) ）***

### Comprehensive
|Name|Paper|Code|
|---|---|---|
|Trustworthy AI|Paper: [gCastle: A Python Toolbox for Causal Discovery](https://arxiv.org/pdf/2111.15155.pdf) Preview:This repository aims to include trustworthy AI related projects from Huawei Noah's Ark Lab. 目前的项目包括：因果结构学习，因果分解表征学习 Current projects include:Causal Structure Learning, Causal Disentangled Representation Learning, gCastle (or pyCastle, pCastle).|[Python](https://github.com/huawei-noah/trustworthyAI)|
|[YLearn](https://ylearn.readthedocs.io/en/latest/)|[Doc](https://ylearn.readthedocs.io/zh_CN/latest/index.html) YLearn, a pun of “learn why”, is a python package for causal learning which supports various aspects of causal inference ranging from causal discovery，causal effect identification, causal effect estimation, counterfactual inference，policy learning，etc.|[Python](https://github.com/DataCanvasIO/YLearn)|

### Treatment Effect Estimation / Uplift Modeling
|Name|Paper|Code|
|---|---|---|
|DoWhy|[Amit Sharma and Emre Kiciman. "Tutorial on Causal Inference and Counterfactual Reasoning." In ACM SIGKDD 2018](http://causalinference.gitlab.io/kdd-tutorial/)|[Python](https://github.com/microsoft/dowhy)|
|EconML|["Causal Inference and Machine Learning in Practice with EconML and CausalML" In EconML/CausalML KDD 2021 Tutorial](https://causal-machine-learning.github.io/kdd2021-tutorial/)|[Python](https://econml.azurewebsites.net/spec/spec.html)|
|Uber CausalML|[Chen, Huigang, et al. "Causalml: Python package for causal machine learning." arXiv preprint arXiv:2002.11631 (2020).](https://arxiv.org/pdf/2002.11631.pdf)|[Python](https://github.com/uber/causalml)|
|JustCause|For evaluation of heterogeneous treatment effect estimators on common reference as well as synthetic data. [Underlying thesis](https://justcause.readthedocs.io/en/latest/_downloads/e054f7a0fc9cf9e680173600cb4b4350/thesis-mfranz.pdf)|[Python](https://github.com/inovex/justcause)|
|WhyNot|An experimental sandbox for causal inference and decision making in dynamics. [Documentation](https://whynot.readthedocs.io/en/latest/)|[Python](https://github.com/zykls/whynot)|
|scikit-uplift|Uplift modeling in scikit-learn style in python. [Documentation](https://www.uplift-modeling.com/en/latest/index.html) and [User guide for uplift modeling](https://www.uplift-modeling.com/en/latest/user_guide/index.html)|[Python](https://github.com/maks-sh/scikit-uplift)|

### Causal Discovery
|Name|Paper|Code|
|---|---|---|
|[Bench Press](https://benchpressdocs.readthedocs.io/en/latest/)|Reproducible and scalable execution and benchmarks of **41** structure learning algorithms supporting multiple language|[Code](https://github.com/felixleopoldo/benchpress)|
|[causal-learn](https://causal-learn.readthedocs.io/en/latest/)|Causal Discovery for Python. A translation and extension of TETRAD.|[Python](https://github.com/cmu-phil/causal-learn)|
|[TETRAD toolbox](http://www.phil.cmu.edu/tetrad/about.html)|[Ramsey, Joseph D., Kun Zhang, Madelyn Glymour, Ruben Sanchez Romero, Biwei Huang, Imme Ebert-Uphoff, Savini Samarasinghe, Elizabeth A. Barnes, and Clark Glymour. "TETRAD-AToolbox FOR CAUSAL DISCOVERY."](https://www.atmos.colostate.edu/~iebert/PAPERS/CI2018_paper_35.pdf)|[R](https://github.com/bd2kccd/r-causal)|
|Causaldag|Python package for the creation, manipulation, and learning of Causal DAGs|[code](https://github.com/uhlerlab/causaldag)|
|CausalNex|A toolkit for causal reasoning with Bayesian Networks.|[Python](https://github.com/quantumblacklabs/causalnex)|
|Tetrad|Tetrad is a modular, object-oriented program for causal inference.|[Java](https://github.com/cmu-phil/tetrad)|
|CausalDiscoveryToolbox|[Kalainathan, Diviyan, and Olivier Goudet. "Causal Discovery Toolbox: Uncover causal relationships in Python." arXiv preprint arXiv:1903.02278 (2019).](https://arxiv.org/pdf/1903.02278)|[Python](https://github.com/Diviyan-Kalainathan/CausalDiscoveryToolbox)|


### Other Applications
|Name|Paper|Code|
|---|---|---|
|[Chaos Genius](https://www.chaosgenius.io/)|ML powered analytics engine for outlier/anomaly detection and root cause analysis.|[Python](https://github.com/chaos-genius/chaos_genius/)|



## Methods

### Casual inference

- Casual inference 初识：基础知识框架建立. [Casual inference知识框架](https://www.notion.so/Casual-inference-c9fdbbbe33684c91af4ed1e79e33a6a1?pvs=21)

    1. **概念和术语理解**：包括“因果效应”、“干预”、“潜在结果”等基本概念。
    
    2. **潜在结果框架**（Potential Outcomes Framework）：这是研究因果推断的主要工具之一，通过定义“潜在结果”来量化和理解因果关系。
    
    3. **图模型和因果图**（Graphical Models and Causal Diagrams）：这些工具可以帮助我们以视觉化的方式理解因果关系。其中，最有名的可能是Judea Pearl的因果图理论。   
    
    4. **反事实理论**（Counterfactual Theory）：这个理论是理解因果推断的另一种方式，其关注的是“如果没有发生，会怎样？”这类问题。
    
    5. **因果效应的估计**（Estimation of Causal Effects）：这是因果推断的主要目标，包括通过观察数据（Observational Data）和实验数据（Experimental Data）来估计因果效应。
    
    6. **随机试验和观察性研究**：随机试验（Randomized Experiments）通常被视为确定因果关系的"金标准"，但在许多情况下，我们无法进行随机试验，而必须依赖观察性研究（Observational Studies）。

    7. **混淆和选择偏差**（Confounding and Selection Bias）：这两个问题是因果推断中需要特别注意的问题。混淆是因为一个未观察的变量同时影响了处理和结果，而选择偏差是因为处理的选择依赖于潜在的结果。
    
    8. **工具和方法**：包括匹配（Matching）、倾向评分（Propensity Score）、工具变量（Instrumental Variables）、中介分析（Mediation Analysis）等。
    
    9. **因果推断的实际应用**：在诸如经济学、流行病学、社会科学、机器学习等领域中的实际应用。
   
    
- 这个系列用相对大白话的语言讲解了**因果推断的算法**  [大白话谈因果 - 知乎 (zhihu.com)](https://www.zhihu.com/column/c_1408014345809227776)
- 总结到目前为止比较主流的做casual inference的方法，包括理论以及代码，实验
    - 这一节介绍了因果推断的基本概念
        
        [因果推断综述及基础方法介绍（一）](https://zhuanlan.zhihu.com/p/258562953)
        
    - 第二节介绍了一些前沿论文以及应用
        
        [因果推断综述及基础方法介绍（二）](https://zhuanlan.zhihu.com/p/366702128)
        
    - 以下github仓库总结了做因果推断的一些方法论
        
        https://github.com/rguo12/awesome-causality-algorithms
        
        为方便查阅，已将该仓库转载于以下链接
        
        [Awesome Casual inference Algorithms](https://www.notion.so/Awesome-Casual-inference-Algorithms-be23e24b0ddd4b9f810e5b219f8acfad?pvs=21)
        


---

---

### Time Series

- ****时间序列预测从入门到精通****

[时间序列预测从入门到精通（一）：基础知识](https://zhuanlan.zhihu.com/p/393594761)

[时间序列预测从入门到精通（二）：传统方法](https://zhuanlan.zhihu.com/p/393644272)

[时间序列预测从入门到精通（三）：深度学习方法](https://zhuanlan.zhihu.com/p/393706324)

- 时间序列分析 （分章节与小点介绍）

- 一份时间序列的纯小白入门教程，从基本概念，EDA，再到各种模型: [时间序列分析101：序言](https://skywateryang.gitbook.io/timeseriesanalysis101/)

- https://github.com/qingsongedu/awesome-AI-for-time-series-papers
- https://github.com/MaxBenChrist/awesome_time_series_in_python
- https://github.com/cuge1995/awesome-time-series
- https://github.com/datamonday/Time-Series-Analysis-Tutorial : 包括了时间序列的论文以及博客

---

---

## Dataset

### NCEP-NCAR Reanalysis 1 数据集（Focus Now）

[NCEP-NCAR Reanalysis 1](https://psl.noaa.gov/data/gridded/data.ncep.reanalysis.html)可进网址下载.



- netCDF数据读取以及处理
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

### CMIP6数据集：(暂且搁置)

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
        

- 气候降尺度方法

[降尺度](https://www.notion.so/55b93e7a9e874435b4ecd0c08dfa3dfe?pvs=21)

***统计降尺度 （SD） 技术***

为了提供可靠的数据集并突出统计缩减的敏感性，在分析中使用了三种不同的SD方法（如下所述）与GCM和RCP结合使用。每种技术都使用三个网格化观测数据产品（Daymet版本2.1，Livneh版本1.2和PRISM版本AN81d）来校准方法的准确性。

1. 德尔塔法（DeltaSD） – 一种广泛使用的简单方法，假设变化发生在更大的区域范围内，并且气候变量之间的关系在未来情景中将保持不变。（[Pourmokhtarian等人，2016](https://doi.org/10.1890/15-0745))
2. 等距分位数映射方法 （EDQM） – 这是分位数映射技术的修改版本，用于通过专门针对每月 GCM 输出的偏差校正来解释时间变化。（[李等人，2010](https://doi.org/10.1029/2009JD012882))
3. 分段异步回归方法（PARM） – 与EDQM类似，该方法利用偏置校正技术，但也通过将一系列线拟合到点数据来解决采样变量的随机不规则性，以消除小规模噪声。（[兰赞特等人，2019](https://doi.org/10.1002/joc.6288))

由于SD方法性能特征的可变性，使用这三种SD技术和各种观测数据产品表明，SD方法的选择可以影响产生的气候预测的可变性。

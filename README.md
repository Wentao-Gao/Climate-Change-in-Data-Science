# Drought Prediction Using Causal Inference (In climate change)

@causality @time series prediction @long term forcasting @feature selection @causal transfer learning


***Research Progress***

- Finished Reshearch Proposal in 2023-10-05.
- Finished My firsr conference paper for IJCAI in 2024-1-17.
- Got rejected by IJCAI.
- Submitted to ECAI in 2024-04-25
- Finished my second conference paper for AAAI in 2024-08-12.
- AAAI under review.
- Prepare my third paper for ICASSP 2025
- Finished my third paper for ICASSP in 2024-09-10
- First paper got accepted by AJCAI 2024 Oral.
- Finished my fourth paper for ICRA 2025
- Prepare my fifth paper for KDD, solving zero inflated problem.
- Got rejected by AAAI.
- Zero inflation paper using improved transformer is submitted to ijcai, 
while the other one which is using diffusion model submitted to ICML


***Next step***

- Next step should be preparing dataset for drought prediction and decide which one suits drought prediction better,
Time series forecasting or classification.

***Papers***

[A Deconfounding Approach to Climate Model Bias Correction](https://arxiv.org/abs/2408.12063)


***Blog***

[Time series deconfounder](https://zhuanlan.zhihu.com/p/681178681)

因果推断在气候预测中的应用

If this helps, please star me and follow me. If you have any questions, please feel free to contact me.

***Latest work***
During work in zero flation, I found that it is hard to find a good implementation for simulation data with zero inflation. So I will provide my implementation 
for everyone who wants to use. Please find the github in anothe markdown file: [Zero Inflation Simulation](https://github.com/Wentao-Gao/Zero_inflation_data_simulation/tree/main).
This is also used in my paper. 

[ElNino data download](https://psl.noaa.gov/data/timeseries/month/DS/Nino4/)


***Author: Wentao Gao***

***Github: https://github.com/gwt9970161/Climate-Change-in-Data-Science***

***A quick overview of causality: [Causality: an intro](https://www.researchgate.net/publication/374233586_Causality_A_Brief_Intro)***

***An introduction to AI: [Lecture Notes(in chinese)](https://wentao-gao.notion.site/Bristol-Intro-to-AI-8ba5854a9a8e49d9a2e1659af5446fa3?pvs=4)***


This project is what I am doing for now during my PhD research. I will mainly focused on casual network. Based on the current understanding of the project, there is a need to integrate causal inference with time series analysis. The objective is to utlize causality in time series prediction. Here are some important part of my research.
   
   - Casual Inference basis，
   
   - Time Series prediction method,

   - NCEP-NCAR Reanalysis 1 data analysis

   - Causal discovery algorithm

   - Feature selection methods


## Domain adaptation paper collection


## Weekly plan:

Further Weekly plan will be posted in the ppt in the ***[Weekly Report part](https://github.com/Wentao-Gao/Climate-Change-in-Data-Science/tree/main/Weekly%20Report)***.

The first 4 weeks are focus on the time series analysis and prediction. 5-8 weeks are focus on the causal inference framework. Week 4 and Week 8 are the summary of time series and causal inference seperately. Please find the summary notes if you are interested in these part.

### Week 1(19/06/2023)
1. **Download and process netCDF4 data**
   - Output a CSV formatted data containing specific latitudes and longitudes, including time, temperature, humidity, sea-level pressure, and the data we need to predict—precipitation.
     - [Convert netCDF4 file to CSV file.ipynb - Colaboratory](https://colab.research.google.com/drive/1mOIKYZ4DrjF4IH5llI0KKn68sRWawW6p)
     - [Replace column and append to main CSV file.ipynb - Colaboratory](https://colab.research.google.com/drive/1oySrXdK_yOxM0cGow9rHRk-zMchCL_oz)

2. **Conduct time series analysis**
   - Using this simple data, including tests for stationarity and others.
     - [Time Series data analysis.ipynb](https://colab.research.google.com/drive/1hu2gfUGSKEyGV9r5K6kG7mlPpKVz3aD7#scrollTo=ae4i6KHH211z)

3. **Train and predict using a simple machine learning model**
   - [RNN Method - Prediction of precipitation.ipynb](https://colab.research.google.com/drive/1JQJJaEqXEAFCjlkjuqsEx0Zn1ykAdDhi#scrollTo=umofRzBWlcsw)

4. **Use a better model for prediction**
   - Specifically, the LSTM method for tackling this prediction problem.
     - [LSTM Method - Prediction of Precipitation.ipynb](https://colab.research.google.com/drive/1HE52cH7wIfjQl64MekuAGvopxx2SQtmu#scrollTo=ZlFnxgpCGl1j&uniqifier=1)

5. **Research**
   - Read the paper provided by Professor Jiuyong to understand how time series is applied in Drought Prediction.


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
- [Tigramite – causal inference in time series](https://github.com/jakobrunge/tigramite)

## Toolboxes for Causality
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

- **Introduction to Casual Inference**: Laying the foundational framework. [Casual Inference Framework](https://www.notion.so/Casual-inference-c9fdbbbe33684c91af4ed1e79e33a6a1?pvs=21)

    1. **Understanding of Concepts and Terminologies**: This includes fundamental concepts like "causal effect", "intervention", and "potential outcomes".
    
    2. **Potential Outcomes Framework**: One of the primary tools to study causal inference, it quantifies and understands causal relationships by defining "potential outcomes".
    
    3. **Graphical Models and Causal Diagrams**: These tools aid in visualizing causal relationships. Notably, Judea Pearl's causal diagram theory is among the most prominent.
    
    4. **Counterfactual Theory**: Another approach to understanding causal inference. It focuses on "what would have happened if not?" type of questions.
    
    5. **Estimation of Causal Effects**: The primary objective of causal inference, it estimates causal effects through both observational and experimental data.
    
    6. **Randomized Experiments and Observational Studies**: Randomized experiments are often considered the "gold standard" for determining causality. However, in many instances where such experiments are not feasible, we have to rely on observational studies.
    
    7. **Confounding and Selection Bias**: Both are pivotal concerns in causal inference. Confounding arises when an unobserved variable affects both the treatment and the outcome, whereas selection bias emerges when the choice of treatment depends on potential outcomes.
    
    8. **Tools and Techniques**: This includes matching, propensity score, instrumental variables, mediation analysis, etc.
    
    9. **Practical Applications of Causal Inference**: How causal inference is applied in real-world scenarios in fields such as economics, epidemiology, social sciences, machine learning, among others.
   
    
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
        


## Dataset

### NCEP-NCAR Reanalysis 1（Focus Now）

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



# 总体目的

要为工业数据智能课题组（Industrial Data Intellignece Group）的新生写一个数据智能入门指南，使得新生同学可以了解机器学习的基本概念（数据、样本、模型、训练目标、loss、泛化性、正则），主流的几个流派（判别模型/生成模型，确定性模型/概率模型）。而后，分几个板块，分别介绍贝叶斯机器学习、序列建模模型、视觉模型、语言大模型、多模态模型、深度生成模型；而后，从learning的角度，再分别介绍transfer、continual、federated、manifold、meta learning等一系列场景概念，以及每个场景下采用的关键技术及其分类。总体目标是深入浅出地为新生以及没有基础的老师讲明白目前深度学习+机器学习的基本概念和关键技术。

# Guideline的架构设计
整体有两个part：
- 前一个part用于介绍基础机器学习概念，重点是要讲清楚整个机器学习的全流程，数据-模型-训练（优化）-推理，重点参考的是 mml-book.pdf这本书，路径为："C:\Users\win11\OneDrive\Myworks\Introduction2DataIntelligence\mml-book.pdf"
- 后一个part再次分为3个部分，第1部分讲贝叶斯机器学习，第2部分讲目前的深度学习模型（或者是，深度学习与贝叶斯机器学习结合），第三部分讲“learning的角度，再分别介绍transfer、continual、federated、manifold、meta learning等一系列场景概念”
    - 贝叶斯机器学习部分的主要参考书为《机器学习：贝叶斯和优化方法》这本书，路径为："C:\Users\win11\OneDrive\Myworks\Introduction2DataIntelligence\机器学习：贝叶斯和优化方法（英文文字）.pdf"，重点要让读者搞清楚参数化模型和非参数化模型的概念，对于概率模型+数据应该是一个怎样的learning方式，确定性模型和概率模型之间的联系是什么（其中一些东西是共同的，比如一些正则化，其实在概率模型中对应的是最大后验估计），叙述形式可以由agent来拟定，分几个
    - 第二部分分为“序列建模模型、视觉模型、语言大模型、多模态模型、深度生成模型”几个章节展开，每个部分都需要数学和形象化解释并重，并给出具体的模型例子；例如深度生成模型就必须要给出VAE和Diffusion等模型的具体数学推导公式，序列建模必须要有RNN到Transformer的整个发展流程以及每个模型的关键数学表示
    -第三部分分别介绍transfer、continual、federated、manifold、meta learning等一系列场景概念，以及每个场景下采用的关键技术及其分类；对于关键的技术也需要对数学进行详细叙述和证明，但是同时也要有形象的说明

# 写作方式
用latex进行写作，用学术的中文，中文不好表示时可以用英文，对于关键的算法和概念请给出中英文；每一个小章节写成一个tex文件，给出一个main文件的入口。
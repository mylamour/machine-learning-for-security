### 计算机安全工程师的机器学习

## 这是？

这是本人目前工作中读到的一些论文和Todo,自诩作为一名半成品安全工程师,同时也作为一名半成品机器学习工程师，将机器学习应用到攻击中是我一直以来的愿望。不过目前所做的却大多是检测性质的工作。当然最早在2000年的时候就已经有人应用机器学习到病毒检测了。所以,17年后两个知识学科的交集应该显得并不那么突兀。(当我有些得意要把两者结合到一起的主意时，才发现早已经有人开始去做，甚至一些做的还很不错。)

这并不是一个教程计划，而是一个资源收集，所以假设你已经具有了基础的渗透能力和机器学习能力。机器学习(Or深度学习)在安全领域可以应用的地方还是很多的。例如:

* 病毒检测
* DGA检测
* Webshell检测
* 异常流量分析
* 各种检测绕过,webshell检测以及各种检测
* 自动化钓鱼，生成受害者感兴趣的东西给他点
* 生成符合规律的密码(总觉得这个用处不大,但是应该也能减少一定的爆破时间吧)
* 用户画像查找嫌疑人

> 这些检测与绕过大部分无非是与文本相关的处理，所以可算是NLP在安全领域的应用,同时也可以看到,将二进制文件转换为灰度图可以用来检测病毒,所以这个可以算是CV的迁移应用。同样，在绕过检测这个环节里，有可能会用到RL的一些知识。


格式如下:

```bash
**[序号]** 名称 [[pdf]](链接) **(描述,应用场景)** 推荐星级 :star::star::star::star::star:
```

---

## 目录

- [这是？](#这是)
- [正文 ](#正文)
- [资源](#资源)
---

## 正文

**[0]** Ye Zhang, Byron Wallace. "A Sensitivity Analysis of (and Practitioners' Guide to) Convolutional Neural Networks for Sentence Classification",  6 Apr 2016 [[pdf]](https://arxiv.org/abs/1510.03820v1) **(文本分类，检测webshell)** 推荐星级:star::star::star::star::star:

**[1]** Yoon Kim. "Convolutional Neural Networks for Sentence Classification", 3 Sep 2014 [[pdf]](https://arxiv.org/abs/1408.5882) **(文本分类，检测webshell)** 推荐星级:star::star::star::star::star:

**[2]** Hyrum S. Anderson, Jonathan Woodbridge, Bobby Filar. "DeepDGA: Adversarially-Tuned Domain Generation and Detection",6 Oct 2016 [[pdf]](https://arxiv.org/abs/1610.01969) **(生成对抗网络，DGA检测)** 推荐星级:star::star::star::star::star:

**[3]** "DeepSign: Deep Learning for Automatic Malware
Signature Generation and Classification" [[pdf]](http://www.covert.io/research-papers/deep-learning-security/DeepSign-%20Deep%20Learning%20for%20Automatic%20Malware%20Signature%20Generation%20and%20Classification.pdf) **(病毒签名生成和检测)** 推荐星级:star::star::star::star::star:

**[4]** Jonathan Woodbridge, Hyrum S. Anderson, Anjum Ahuja, Daniel Grant. "Predicting Domain Generation Algorithms
with Long Short-Term Memory Networks",2 Nov 2016 [[pdf]](https://arxiv.org/abs/1611.00791) **(LSTM,DGA检测)** 推荐星级:star::star::star::star::star:

**[5]** Hyrum S. Anderson, Anant Kharkar,Bobby Filar. "Evading Machine Learning Malware Detection" [[pdf]](https://www.blackhat.com/docs/us-17/thursday/us-17-Anderson-Bot-Vs-Bot-Evading-Machine-Learning-Malware-Detection-wp.pdf) July 22-27, 2017 **(绕过病毒检测)** 推荐星级:star::star::star::star::star:

**[6]** L. Nataraj, S. Karthikeyan,G. Jacob. "Malware Images: Visualization and Automatic Classification" [[pdf]](https://vision.ece.ucsb.edu/sites/vision.ece.ucsb.edu/files/publications/nataraj_vizsec_2011_paper.pdf), 2011 **(二进制可视化，病毒检测)** 推荐星级:star::star::star::star::star:

**[7]** L. Nataraj, Vinod Yegneswaran,Phillip Porras,Jian Zhang. "A Comparative Assessment of Malware Classification using Binary Texture Analysis and Dynamic Analysis" [[pdf]](https://vision.ece.ucsb.edu/sites/vision.ece.ucsb.edu/files/publications/aisec17-nataraj.pdf) **(二进制可视化，图像分类，病毒检测)** 推荐星级:star::star::star::star::star:


## 资源

* [Machine Learning for Cyber Security](https://github.com/wtsxDev/Machine-Learning-for-Cyber-Security)
* [Jason Trost:Collection of Deep Learning Cyber Security Research Papers](https://medium.com/@jason_trost/collection-of-deep-learning-cyber-security-research-papers-e1f856f71042)
* [The Definitive Security Data Science and Machine Learning Guide](http://www.covert.io/the-definitive-security-datascience-and-machinelearning-guide/)
* [CS 259D: Data Mining for Cyber Security](http://web.stanford.edu/class/cs259d/)

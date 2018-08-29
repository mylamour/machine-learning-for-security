### 计算机安全工程师的机器学习

## 这是？

这是本人目前工作中读到的一些论文，文档以及一些Todo,自诩作为一名半成品安全工程师,同时也作为一名半成品机器学习工程师，将机器学习应用到攻击中是我一直以来的愿望。不过目前所做的却大多是检测性质的工作。当然最早在2000年的时候就已经有人应用机器学习到病毒检测了。所以,17年后两个知识学科的交集应该显得并不那么突兀。(当我有些得意要把两者结合到一起的主意时，才发现早已经有人开始去做，甚至一些做的还很不错。)

这并不是一个教程计划，而是一个资源收集，所以假设你已经具有了基础的渗透能力和机器学习能力。机器学习(Or深度学习)在安全领域可以应用的地方还是很多的。例如:

* 病毒检测
* DGA检测
* Webshell检测
* 异常流量分析
* 各种检测绕过,webshell检测以及各种检测
* 自动化钓鱼，生成受害者感兴趣的东西给他点
* 生成符合规律的密码(总觉得这个用处不大,但是应该也能减少一定的爆破时间吧)
* 用户画像查找嫌疑人
* 威胁情报文本摘要
* 用于Fuzzing攻击
* 反诈骗聊天机器人(之前看到过一个专门用于和垃圾邮件聊天的机器人，用于消耗骗子的时间)

> 这些检测与绕过大部分无非是与文本相关的处理，所以可算是NLP在安全领域的应用,同时也可以看到,将二进制文件转换为灰度图可以用来检测病毒,所以这个可以算是CV的迁移应用。同样，在绕过检测这个环节里，有可能会用到RL的一些知识。


格式如下:

```bash
**[序号]** 作者. "名称", [[pdf]](链接),年份 **(描述,应用场景)** 推荐星级 :star::star::star::star::star:
```

---

## 目录

- [这是？](#这是)
- [正文 ](#正文)
- [资源](#资源)
---

## 正文


### Webshell Detection

**[1]** Ye Zhang, Byron Wallace. "A Sensitivity Analysis of (and Practitioners' Guide to) Convolutional Neural Networks for Sentence Classification", [[pdf]](https://arxiv.org/abs/1510.03820v1),6 Apr 2016 **(文本分类，检测webshell)** 推荐星级:star::star::star::star::star:

**[2]** Yoon Kim. "Convolutional Neural Networks for Sentence Classification" [[pdf]](https://arxiv.org/abs/1408.5882),3 Sep 2014 **(文本分类，检测webshell,XSS等)** 推荐星级:star::star::star::star::star:

**[3]** Johannes Dahse. "Static Detection of Complex Vulnerabilities in Modern PHP Applications" [[pdf]](https://d-nb.info/1099703417/34), 02 Feb 2016 **(AST，检测webshell)** 推荐星级:star::star::star::star::star:

### DGA Detection

**[1]** Hyrum S. Anderson, Jonathan Woodbridge, Bobby Filar. "DeepDGA: Adversarially-Tuned Domain Generation and Detection" [[pdf]](https://arxiv.org/abs/1610.01969),6 Oct 2016 **(生成对抗网络，DGA检测)** 推荐星级:star::star::star::star::star:

**[2]** Jonathan Woodbridge, Hyrum S. Anderson, Anjum Ahuja, Daniel Grant. "Predicting Domain Generation Algorithms
with Long Short-Term Memory Networks" [[pdf]](https://arxiv.org/abs/1611.00791),2 Nov 2016 **(LSTM,DGA检测)** 推荐星级:star::star::star::star::star:

### Malware Detection

**[1]** "DeepSign: Deep Learning for Automatic Malware
Signature Generation and Classification" [[pdf]](http://www.covert.io/research-papers/deep-learning-security/DeepSign-%20Deep%20Learning%20for%20Automatic%20Malware%20Signature%20Generation%20and%20Classification.pdf) **(病毒签名生成和检测)** 推荐星级:star::star::star::star::star:

**[2]** Hyrum S. Anderson, Anant Kharkar,Bobby Filar. "Evading Machine Learning Malware Detection" [[pdf]](https://www.blackhat.com/docs/us-17/thursday/us-17-Anderson-Bot-Vs-Bot-Evading-Machine-Learning-Malware-Detection-wp.pdf),22-27 July 2017 **(绕过病毒检测)** 推荐星级:star::star::star::star::star:

**[3]** L. Nataraj, S. Karthikeyan,G. Jacob. "Malware Images: Visualization and Automatic Classification" [[pdf]](https://vision.ece.ucsb.edu/sites/vision.ece.ucsb.edu/files/publications/nataraj_vizsec_2011_paper.pdf),2011 **(二进制可视化，病毒检测)** 推荐星级:star::star::star::star::star:

**[4]** L. Nataraj, Vinod Yegneswaran,Phillip Porras,Jian Zhang. "A Comparative Assessment of Malware Classification using Binary Texture Analysis and Dynamic Analysis" [[pdf]](https://vision.ece.ucsb.edu/sites/vision.ece.ucsb.edu/files/publications/aisec17-nataraj.pdf) **(二进制可视化，图像分类，病毒检测)** 推荐星级:star::star::star::star::star:

**[5]** Kolter, Maloof. "Learning to detect malicious executables in the wild" [[pdf]](http://machinelearning.wustl.edu/mlpapers/paper_files/KolterM06.pdf),2004 **(NLP, n-grams of byte codes,静态分析,病毒检测)** 推荐星级:star::star::star::star::star:

**[6]** Microsoft. "Microsoft portable executable and common object file format specification", [[pdf]](https://adeetc.thothapp.com/classes/SO/1617i/LI41N/workitems/1833/attachment),2013 **(微软PE文件的格式说明,需要了解的基础知识)** 推荐星级 :star::star::star::star::star:

**[7]** J. Saxe and K. Berlin. "Deep neural network based malware detection using two dimensional binary program features.In Malicious and Unwanted Software (MALWARE)", [[pdf]](https://arxiv.org/pdf/1508.03096.pdf),3 Sep 2015 **(DNN套路病毒检测，面对未知病毒也可检测)** 推荐星级 :star::star::star::star::star:


### IDS

**[1]** 金波,林家骏,王行愚. "入侵检测技术评述[J]. 华东理工大学学报", 21 09 2017 推荐星级 :star::star::star:


### Password

**[1]** Briland Hitaj, Paolo Gasti, Giuseppe Ateniese, Fernando Perez-Cruz "PassGAN A Deep Learning Approach for Password Guesssing", [[pdf]](https://arxiv.org/pdf/1709.00440.pdf),1 Sep 2017 **(GAN网络 破解密码)** 推荐星级 :star::star::star::star::star:

### Attack

**[1]** Alex Graves, "Generating Sequences With Recurrent Neural Networks", [[pdf]](https://arxiv.org/pdf/1308.0850.pdf), 5 Jun 2014 **(文本生成必备论文，RNN,作为LSTM生成XSS必读论文)** 推荐星级 :star::star::star::star::star:

**[2]** Hila Peleg, Patrice Godefroid,Rishabh Singh, "Learn&Fuzz: Machine Learning for Input Fuzzing", [[pdf]](https://patricegodefroid.github.io/public_psfiles/ase2017.pdf), 2017 **(机器学习和Fuzzing )** 推荐星级 :star::star::star::star::star:

## 资源

> 资源再多,也没什么用。以如今互联网的发展程度，找资源可以说是轻而易举。稍微动动脑子,都能拿的到。但是关键在于,有和用是两码事。本来并不想在资源这里列很多东西。但觉得不列出来是不完整的,这些知识都是相辅相成的。但又怕列多了误导别人(说的好像真有人来看似的)。因此,暂且仅挑几本书放在下面吧。

* [Machine Learning for Cyber Security](https://github.com/wtsxDev/Machine-Learning-for-Cyber-Security)
* [Jason Trost:Collection of Deep Learning Cyber Security Research Papers](https://medium.com/@jason_trost/collection-of-deep-learning-cyber-security-research-papers-e1f856f71042)
* [The Definitive Security Data Science and Machine Learning Guide](http://www.covert.io/the-definitive-security-datascience-and-machinelearning-guide/)
* [CS 259D: Data Mining for Cyber Security](http://web.stanford.edu/class/cs259d/)
* [The Art of Memory Forensics](https://www.amazon.com/Art-Memory-Forensics-Detecting-Malware/dp/1118825098)
* [Practical malware analysis: the hands-on guide to dissecting malicious software](https://vision.ece.ucsb.edu/sites/vision.ece.ucsb.edu/files/publications/aisec17-nataraj.pdf)
* [Malware Analyst's Cookbook](https://www.amazon.com/Malware-Analysts-Cookbook-DVD-Techniques/dp/0470613033)
* [Linux Firewalls: Enhancing Security with nftables and Beyond (4th Edition)](https://www.amazon.com/Linux-Firewalls-Enhancing-Security-nftables/dp/0134000021)

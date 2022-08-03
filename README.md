### 问题1




图像分类是一个输入图像，输出该图像所属类别的CV核心问题之一。图像分类的传统方法是特征描述及检测，其对简单数据有效，但却不适用于如今复杂的数据。如今深度学习是处理图像分类的主流方法。面对复杂数据，我们通常通过更改网络结构、损失函数、或数据预处理等操作实现提高准确率的效果。但是不同的处理其优化方式、适用范围不同。（请在pytorch平台上进行实验，代码中需注释表明关键模块）


1.使用pytorch平台提供的预训练的VGG19作为backbone，交叉熵为损失函数，对cifar100中10类(maple, bed, bus, plain, dolphin, bottles, cloud, bridge, baby, rocket)训练一个10分类网络。记录网络在测试集上对不同类别的识别准确率，并保存网络模型。  
2.将问题1中的十个类别更换为：maple, bed, bus, plain, streetcar, oak, palm, pine, willow, forest。使用相同的实验配置训练一个10分类网络，与问题1中的分类准确率比较，并分析它们的差异。如果新的准确率更低，请从损失函数的角度提高分类精度。  
3.对问题1，2的网络读取卷积层最后一层的特征，将这两组特征分别通过T-SNE可视化成二维的特征分布图。比较这两个特征分布图，结合问题1、2试着分析不同的原因。  




### 问题2


假设给定一个数据集A，其包含100个元素{a1,…,a100}，每个元素大小未知，ai不等于aj，给定数据集B，其包含500个元素对（ai，aj），和它们的大小关系{ai>aj或ai<aj}，i不等于j，ai，aj在数据集中分布均匀。  
 1、设计一种通过变量对（ai，aj）的大小关系对数据集A中元素排序的求解程序。  
 2.分析这个算法的复杂度。  
 3.分析当已知多少元素对(ai,aj)时算法可有唯一解。  

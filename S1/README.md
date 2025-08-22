
1. PyTorch提供了一个核心数据结构——Tensor，一个与NumPy数组非常相似的多维数组。
2. Tensor可用于加速数学运算，并且PyTorch内置了可用于分布式训练、高效数据加载的函数包，以及大量常用的深度学习函数。
3. TensorFlow

- 使用Keras作为核心API
- 提供即时执行模式（eager mode）
- 宣布eager mode为TF2.0的默认执行模式

4. PyTorch

- 使用Caffe2作为后端
- 替换了基于Lua的Torch项目中重复使用的大多数低级代码
- 增加了对ONNX的支持，定义了一种与深度学习库无关的模型描述和转换格式
- 增加了称为TorchScript的延迟执行图模式运行引擎

5. PyTorch中有很多非Python代码，大多数PyTorch都是用C++和CUDA编写的，CUDA是NVIDIA提供的类似C++的语言，可以将其编译然后在NVIDIA GPU上大规模并行运行。

6. PyTorch的**核心**是提供多维数组的库，在PyTorch术语中这些多维数组称为张量（tensor），而torch模块则提供了可对其进行扩展操作的库。PyTorch提供的**第二个核心**功能是允许张量跟踪对其所执行的操作，并通过反向传播来计算输出相对于其任何输入的导数。此功能由张量自身提供，并通过torch.autograd进一步扩展完善。

7. PyTorch 的主要功能模块包括以下几个：
- torch: 核心模块，包含张量操作、数学运算、随机数生成等基础功能。

- torch.nn: 提供构建神经网络的工具，包括各种层（如卷积层、全连接层）、激活函数、损失函数等。

- torch.optim: 包含优化器模块，用于实现各种优化算法（如 SGD、Adam、RMSprop 等）。

- torch.utils.data: 数据加载模块，提供 DataLoader 和 Dataset 类，用于加载和处理数据。

- torchvision: 计算机视觉相关模块，包含常用的数据集（如 CIFAR-10、ImageNet）、数据增强工具和预训练模型。

- torchtext: 自然语言处理相关模块，支持文本数据处理、词嵌入和数据集加载。

- torchaudio: 音频处理模块，支持音频数据加载、转换和预处理。

- torch.distributed: 分布式训练模块，支持多 GPU 和多节点的分布式训练。

- torch.cuda: GPU 加速模块，提供对 CUDA 的支持，用于加速张量计算。

- torch.autograd: 自动微分模块，支持动态计算图和梯度计算。

- torch.jit: 提供 TorchScript 功能，用于将模型序列化和优化。

- torch.onnx: 支持将 PyTorch 模型导出为 ONNX 格式，用于跨平台部署。
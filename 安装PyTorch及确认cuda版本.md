
安装 PyTorch 深度学习框架时需要确认当前机器 cuda 版本，很多花里胡哨的文章介绍各种复杂的命令，有的居然还要关注公众号才能阅读完整完整....

哪有这么麻烦！直接在命令终端中执行 `nvidia-smi` 命令即可！以 Windows 为例：

![show-cuda-version.png](http://snic88335.hd-bkt.clouddn.com/cuda-version/show-cuda-version.png)

红框中就是当前机器 cuda 版本，我的是 12.4，之后直接到 pytorch 官网（[https://pytorch.org/get-started/locally/](https://pytorch.org/get-started/locally/)）下载该 cuda 对应安装版本即可：

![install-PyTorch.png](http://snic88335.hd-bkt.clouddn.com/cuda-version/install-PyTorch.png)

在终端中输入安装命令回车就完事了：

```bash
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu124
```
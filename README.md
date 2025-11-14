# MST_py38 - Multiscale Transformer 可复现环境
这是一个为复现 [caiyuanhao/MST](https://github.com/caiyuanhao1998/MST) 项目而准备的 Python 3.8 完整环境包。

## 📦 环境包下载

由于环境包体积较大（超过2GB），无法直接存放在GitHub。请通过以下方式下载：

### 百度网盘下载
- **下载链接**: https://pan.baidu.com/s/1uWh2_4IQCDicr9RAo5kkwg?pwd=wmw7 
- **提取码**: 提取码: wmw7  （请替换为您的实际提取码）

### 下载说明
1. 点击上方链接或复制到浏览器打开
2. 输入提取码
3. 下载 `MST_py38.tar.gz` 文件

## 🚀 快速开始

### 环境恢复步骤
# 1. 进入conda环境的默认存放目录（所有conda环境都在这里）
cd /home/*******/anaconda3/envs/

# 2. 解压上传的环境压缩包（生成 `MST_py38` 文件夹，即完整环境）
tar -xzf /home/********/MST_py38.tar.gz

# 3. 激活刚解压的环境
conda activate MST_py38

# 4. 验证环境是否正常（以你的环境为例，假设包含GPU版torch）
python -c "import torch; print('Python版本：', torch.__version__); print('CUDA可用：', torch.cuda.is_available()); print('GPU型号：', torch.cuda.get_device_name(0) if torch.cuda.is_available() else '无')"

# 5.环境激活后，直接运行训练脚本即可：
python /home/********/MST-main/simulation/train_code/train.py

## ⚠️ 注意事项
- 本环境基于 Python 3.8 构建
- 确保系统有足够的磁盘空间（建议10GB以上）
- 如遇网络问题，可尝试使用网盘客户端下载

## 🤝 参与贡献
如果您发现环境配置问题或有改进建议，欢迎提交Issue或Pull Request！

## 📄 许可证
本项目采用 MIT 许可证 - 详见 [LICENSE](LICENSE) 文件

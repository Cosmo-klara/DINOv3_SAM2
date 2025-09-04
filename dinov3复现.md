## DINOV3复现

### 环境配置

#### 网络配置

连接服务器后需要先进行网络配置, 也即将 BIT-srun-login-script 项目clone到服务器上

> 该项目依赖于requests库，建议 pip install 后再尝试运行

其中always_online.py中的用户和密码需要替换为你的校园网账户密码

运行

```bash
cd BIT-srun-login-script
python always_online.py
```

验证网络环境，`ping baidu.com` 测试一下能不能 ping 通

#### 项目环境配置

随后进入项目目录并配置基本环境（如果pip下载仍旧超时，请自行搜索配置pip国内镜像下载源，阿里云或者清华源）

```bash
cd ../dinov3
conda env create -f conda.yaml
conda activate dinov3
```

### 连接远程服务器

```bash
pip install notebook
jupyter notebook password
```

随后输入并确认密码，

### 模型下载


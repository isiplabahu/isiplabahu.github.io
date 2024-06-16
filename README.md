## 实验室网站使用指南

请严格按照以下步骤进行，不要进行其他修改！

### 1. fork 实验室主页仓库然后克隆到本地进行修改

不知道怎么 fork 或者使用 git 的请自行查阅相关资料, 或者请教实验室其他会的同学

```bash
git clone https://github.com/your_user_name/isiplabahu.github.io.git
```

### 2. 添加论文引用

在 `_bibliography/papers.bib` 中添加你的论文, 格式为 bib, 参考如下:

```
@article{20230115,
bibtex_show={true},
author={Gao, Teng and Pan, Qing and Zhou, Jian and Wang, Huabin and Tao, Liang and Kwan, Hon},
year={2023},
month={01},
title={A Novel Attention-Guided Generative Adversarial Network for Whisper-to-Normal Speech Conversion (Submitted)},
volume={15},
journal={Cognitive Computation},
doi={10.1007/s12559-023-10108-9},
preview={wave-mechanics.gif},
html={https://arxiv.org/abs/2111.01342},
selected={true}, # 为true表示该论文会展示在实验室首页
}
```
自行填写论文状态信息，例如论文名、年月日、论文状态 (Submitted, Accepted) 等

### 3. 添加论文 demo 页面

- 在 `_posts` 文件夹下新建你的 demo.md 文件，参考格式如下：

```
文件名: year-month-day-xxxx.md
例如: 2023-11-11-demo.md
具体内容可以参照 2023-11-11-demo.md
```
- demo 页面需要包含图片、音频等的 (不要上传代码、模型等大型文件), 统一将相关资源放在 `_assets/your_name` 文件夹下, 文件夹以姓名拼音命名
- markdown 格式

### 4. 代码

在你的个人 github 账号下创建新仓库, 然后在 `_data/repositories.yml` 中引用, 参考如下

```
github_users:
  - isiplabahu
  - clumsyroot

github_repos:
  - isiplabahu/isiplabahu.github.io
  - your_github_user_name/repositories_name # 在这里添加你的代码，格式为: 你的github账号名称/代码仓库名称
```

**非管理员需要进行以下两步, 管理员可以直接`git push`**

### 5. 提交你的修改


[如何创建 pull request ](https://www.freecodecamp.org/chinese/news/how-to-make-your-first-pull-request-on-github/)

### 6. 网站管理员检查后同意提交的修改

![accept_request](/assets/img/readme_request.png "accept request")

==除了以上提到的几个部分，请慎重修改其他地方，网站管理员需要尤其注意！！!==
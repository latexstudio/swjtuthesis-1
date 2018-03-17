# 西南交通大学学位论文 LaTeX 模板

[![Travis build](https://travis-ci.org/swjtutug/swjtuthesis.svg?branch=master)](https://travis-ci.org/swjtutug/swjtuthesis)
[![GitHub release](https://img.shields.io/github/release/swjtutug/swjtuthesis/all.svg)](https://github.com/swjtutug/swjtuthesis/releases/latest)
[![Github downloads](https://img.shields.io/github/downloads/swjtutug/swjtuthesis/total.svg)](https://github.com/swjtutug/swjtuthesis/releases)
[![GitHub commits](https://img.shields.io/github/commits-since/swjtutug/swjtuthesis/v1.0.0.svg)](https://github.com/swjtutug/swjtuthesis/commits/master)

本项目是西南交通大学的学位论文 LaTeX 模板 swjtuthesis，按照最新版的
《[西南交通大学研究生学位论文撰写规范](http://gs.swjtu.edu.cn/ws/gs/dd/25)》
和
《[本科毕业设计（论文）指导纪要（模板）](http://jwc.swjtu.edu.cn/download/file/2014060410031788.doc)》
的要求编写，兼容最新版的 TeX Live、MacTeX 、MikTeX 发行版，支持跨平台使用。

注意：

1. 使用说明文档
[swjtuthesis.pdf](https://github.com/swjtutug/swjtuthesis/releases/download/v1.0/swjtuthesis.pdf)
在发布版中附带，用户也可自行编译；**使用模板前应仔细阅读**。

2. 本模板要求 TeX Live、MacTeX、MikTeX 不低于 2015 年的发行版，
并且尽可能升级到最新。

3. **不支持** [CTeX 套装](http://www.ctex.org/CTeXDownload)。

4. 这个版本不知道为什么make无法运行，但是其他方式确实可以的。

## 下载地址

- GitHub Releases：https://github.com/swjtutug/swjtuthesis/releases


## 编译文档

- 编译模板的使用说明文档 `swjtuthesis.pdf`：
   ```
   latexmk swjtuthesis.dtx
   ```
- 编译论文 `main.pdf`：
   ```
   latexmk
   ```
- 如需清理论文编译过程中的临时文件，可以：
   ```
   latexmk -c
   ```

- 以上编译过程也可以用 `make` 工具：
   ```
   make doc        # 编译生成 swjtuthesis.pdf
   make            # 编译生成论文 main.pdf
   make clean      # 删除编译过程中生成的临时文件
   ```
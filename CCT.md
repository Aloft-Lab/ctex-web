---
title: CCT
menu_order: 3
---
### CCT

最早的中文TeX扩展系统之一，由中国科学院数学与系统科学研究院张林波研究员开发，目前仍然被众多国内学术期刊使用。

CTeX套装中包含了最新版本的CCT。

#### 最新补丁

- 在较新版本 Windows 10/11（具体版本不详）的默认安全设置下，会发生 `ctex.exe` 无法运行 `patchdvi.exe` 的错误，导致使用 CCT 字库的 CCT 用户无法用 CTeXify 编译。使用 CJK 字库的 CCT 用户不受影响。发生该错误的原因似乎是 `patchdvi.exe` 命令中含有 `patch`，犯了 Windows 的“忌”引起的。
- 使用 CCT 字库的 CCT 用户可以通过下述步骤来解决该问题：
    1. 进入 CTeX 安装目录下的 ``CTeX\\cct\\bin`` 目录（默认为 ``C:\\CTEX\\CTeX\\cct\\bin``）；
    2. 把 `cct-win32-patch-20240509.zip` 中的 `ctex.ini` 和 `ctex.exe` 两个文件拷贝到当前目录，覆盖其中原有的 `ctex.exe`；
    3. 把当前目录中的 `patchdvi.exe` 重命名或拷贝为 `cctpost.exe`。
- 下载 [cct-win32-patch-20240509.zip](https://mirrors.tuna.tsinghua.edu.cn/ctex/cct/cct-win32-patch-20240509.zip)

#### 完整版本

- 20240509发布：[v0.618033-3](https://mirrors.tuna.tsinghua.edu.cn/ctex/cct/cct-0.618033-3-win32.zip)



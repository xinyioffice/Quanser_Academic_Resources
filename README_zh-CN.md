<img src="docs/images/quanser-resources-header.png" width="100%">

[English](README.md) | 中文


# Quanser_Academic_Resources

[Quanser](https://www.quanser.com/) 学术资源包含使用 Quanser 产品所需的研究和教学内容，包括库、研究示例、教学内容、用户手册、指南等。

本仓库包含以下产品的资源：`Aero 2、Mechatronic Actuators Trainer、Mechatronic Sensors Trainer、QArm、QArm Mini、QBot Platform 和旧版 QBot、QCar、QCar 2、QDrone、QDrone 2、Qube-Servo 3`。在 [Quanser 官网](https://www.quanser.com/) 查找这些产品的资源时，会跳转到本仓库。如果需要查找其他产品的资源，请跳过本说明，参阅[旧产品资源](#旧产品资源)部分。

> **面向中国大陆的 fork：** 本 fork 针对中国大陆用户进行了优化。它对 Windows setup 脚本进行了本地化适配，包括使用 USTC PyPI 镜像以及兼容包含中文字符的路径，同时仍基于 Quanser Academic Resources。

### 目录

- [下载资源](#下载资源)
- [配置计算机](#配置计算机)
- [开始使用资源](#开始使用资源)
- [旧产品资源](#旧产品资源)
- [变更记录](changelog.txt)


## 下载资源

**注意：** 如果要设置 Raspberry Pi（4 或 5），以配合 Mechatronic Actuators Trainer 和/或 Mechatronic Sensors Trainer 使用，请跳过本指南，参阅 [Raspberry Pi 设置](1_setup/raspberry_pi/pi_setup.pdf)。这些设备既可以在 Windows 计算机上使用，也可以在 Raspberry Pi 上使用。

开始使用这些资源前，第一步是将资源下载到计算机中。可以使用 Git，也可以直接将文件下载为 `.zip` 压缩包。建议将资源放在 `C:/Users/user/Documents/Quanser` 文件夹中。

### 使用 Git

<details open>
<summary>使用 Git 安装</summary>

1. 在系统中安装 [Git](https://git-scm.com/downloads)。
2. 打开 Documents 文件夹，并在该文件夹中打开 Windows 终端。
3. 运行以下命令，在 Documents 中创建 Quanser 文件夹，并将本仓库内容复制到其中。
    ```
    git clone --branch enhance-setup-batch https://github.com/xinyioffice/Quanser_Academic_Resources.git Quanser
    ```

</details>

### 不使用 Git

<details>
<summary>不使用 Git 安装</summary>

1. 在系统的 Documents 文件夹下创建名为 _Quanser_ 的文件夹，路径应类似于 `C:/Users/user/Documents/Quanser`。
2. 点击当前 GitHub 页顶部的绿色 Code 按钮，然后在弹出的菜单底部点击 _Download ZIP_。
3. 在系统中解压该压缩包。
4. 进入 _Quanser_Academic_Resources-enhance-setup-batch_ 文件夹（其中可以看到 `0_libraries`、`1_setup` 等文件夹），将其中的全部内容复制到新建的 Documents/Quanser 文件夹中。
</details>

## 配置计算机

开始使用这些资源前，需要根据计划使用 Quanser 设备的方式，在计算机上安装必要的软件。这可能包括使用虚拟系统和/或硬件系统，以及使用 Python 和/或 MATLAB/Simulink。

- 请参阅设置指南：[计算机设置](docs/pc_setup.md)。

- 如果系统随附了路由器，请注意：请勿将网线连接到该路由器，否则自动路由器固件更新可能会导致意外行为。

## 开始使用资源

如需全面了解如何开始使用这些资源和 Quanser 产品，请参阅[资源使用入门指南](6_teaching/README.md)。


# 旧产品资源

**_对于上面未列出的其他产品，请访问 Quanser 官网的[资源页面](https://www.quanser.com/resources/)。_**

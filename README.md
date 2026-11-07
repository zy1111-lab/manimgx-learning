# ManimGX 学习记录

通过复现 ManimGX 官方示例，学习 Python 动画编程、Git 版本管理和 GitHub 协作。

上游项目：https://github.com/academa-labs/manimgx

## 已完成的练习

- 安装 ManimGX，运行官方 Hello3D 立方体示例。
- 将立方体边长从 3 改为 2，观察尺寸变化。
- 将相机旋转速度从 0.5 改为 1.0，观察视角变化。
- 使用 Git 保存代码版本，并上传到 GitHub。

## 文件说明

- `outputs/scene.py` 是基于官方 Hello3D 示例修改的动画代码。
- `outputs/requirements.txt` 记录本次使用的依赖版本。
- `outputs/第一课.md` 包含运行方法、代码解释和练习记录。

## 运行方法

需要 Python 3.13 或更新版本。在项目根目录打开 PowerShell。

首次使用时，创建独立环境并安装依赖：

```powershell
python -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r .\outputs\requirements.txt
```

已有环境时，可以直接渲染：

```powershell
.\.venv\Scripts\manimgx.exe render .\outputs\scene.py -o .\outputs\Hello3D-practice.mp4
```

生成的视频保存在 `outputs` 文件夹中。视频和 Python 环境由 `.gitignore` 忽略。

## 后续学习

- 继续练习物体外观、动画时长和相机参数。
- 阅读 ManimGX 源码，理解场景如何生成。
- 学习整理可复现的问题报告，逐步参与开源协作。
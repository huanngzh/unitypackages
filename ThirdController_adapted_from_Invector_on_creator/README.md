# Third Controller Adapted from Invector

> 本来只是想简单地做个 **Inspector 自定义按钮创建示例**，后来看 Invector 创建角色的按钮在导航栏，就把该功能移植到面板按钮上。

Inspector 自定义按钮创建方法见 [Unity Inspector 自定义按钮 _ Zewan Blog](https://blog.zewan.cc/2021/08/11/unity/editor-inspector/)

关键代码见 `Assets/Scripts/CharacterManage_InspectorButton/`

## 简介

改编自 Invector Basic Locomotion（基础的角色导航控制器）。

Invector（一个强大的角色控制器），创建人物角色的方法在导航栏 windows 处。本工具将该功能复写到 Inspector 面板按钮中，并编写了一个角色管理脚本，可选择用于活动的角色。

- **新角色创建**：拖动 FBX 文件到 `Charactor Creator` 组件下的 `FBX Object` 处，点击 `Create Character` 按钮
- **活动角色管理**：拖动 Characters 下的角色到 `Active Character` 处，点击 `Set Active Char` 按钮

![Inspector 截图](Resources/Images/Inspector.png)

除此之外，本项目清除了 Invector 复杂的组件修饰等，可直接作为项目的基础进行开发。

附上角色控制的按键使用：WSAD 控制前后左右移动，同时按下 Shift 可加速移动，空格键控制跳跃。

![Game](Resources/Images/Game.png)

## 致谢

- [Invector - 角色控制器](https://www.invector.xyz/)
# AutoMakeHuman

[![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](LICENSE)
[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)

    MakeHuman's plugin for auto create human models

    基于开源3D软件MakeHuman编写的插件
    主要功能是输入二维图片，通过改变三维人体模型的参数，把模型映射到二维空间，通过轮廓迭代求优算法，得到三维模型与二维图片的配准
    
    请根据实际安装路径，修改源码中的路径

## Main Features
 - Auto create 3d models
 - Picture features recognize

## 7_auto_human_body
    change model shape to fit picture

    通过改变体态得到模型与二维图片的配准

## 7_auto_human_pose
    change model position to fit picture

    通过改变姿态得到模型与二维图片的配准

## 使用方法
    1.将src下的文件拷贝到makehuman/plugins/下
    2.重启makehuman,在makehuman的"工具"栏下即可看到新安装的插件

## Install

V1.1.1

    chmod +x bin/*.sh
    bin/install.sh
V1.2 +

    1. open makehuman
    2. switch tab to "Settings" to install user plugin
    3. activate plugin.
    4. if have some problem, check logs.
    
## Develop

    conda create -n human
    set MAKEHUMAN_PATH=D:/Python/human/makehuman/makehuman
    conda-develop %MAKEHUMAN_PATH% %MAKEHUMAN_PATH%/apps %MAKEHUMAN_PATH%/lib %MAKEHUMAN_PATH%/core %MAKEHUMAN_PATH%/shared

## Question

### 1. no path found
    makehuman/plugins/7_auto_human_body/data/Auto3DImage
    
    create those paths

## Support
  see Wiki and Issues

  mailto:<zergskj@163.com>

------------------

## ToDo list
 1.Add reinforcement-learning to auto generate model.

 2.Add body edge detected.

 3.Use NEAT structure to generate RNN.

 4.Adjust NEAT policy study more once.
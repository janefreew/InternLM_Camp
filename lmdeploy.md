- 提交方式：在各个班级对应的 GitHub Discussion 帖子中进行提交。

# 基础作业：

- 使用 LMDeploy 以本地对话、网页Gradio、API服务中的一种方式部署 InternLM-Chat-7B 模型，生成 300 字的小故事（需截图）

## 本地对话

```sh
lmdeploy chat turbomind ./workspace
```

![image-20240404121749741](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240404121749741.png)

## 网页Gradio

![image-20240404120919681](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240404120919681.png)

![image-20240404120859484](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240404120859484.png)



## API 服务

![image-20240404122320603](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240404122320603.png)

![image-20240404122410542](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240404122410542.png)



# 进阶作业（可选做）

- 将第四节课训练自我认知小助手模型使用 LMDeploy 量化部署到 OpenXLab 平台。
  对internlm-chat-7b模型进行量化，并同时使用KV Cache量化，使用量化后的模型完成API服务的部署，分别对比模型量化前后（将 bs设置为 1 和 max len 设置为512）和 KV Cache 量化前后（将 bs设置为 8 和 max len 设置为2048）的显存大小。
  - 在自己的任务数据集上任取若干条进行Benchmark测试，测试方向包括：
    （1）TurboMind推理+Python代码集成
    （2）在（1）的基础上采用W4A16量化
    （3）在（1）的基础上开启KV Cache量化
    （4）在（2）的基础上开启KV Cache量化
    （5）使用Huggingface推理
    备注：由于进阶作业较难，完成基础作业之后就可以先提交作业了，在后续的大作业项目中使用这些技术将作为重要的加分点！

- 整体实训营项目：
  - 时间周期：即日起致课程结束

- 即日开始可以在班级群中随机组队完成一个大作业项目，一些可提供的选题如下：

  - 人情世故大模型：一个帮助用户撰写新年祝福文案的人情事故大模型

  - 中小学数学大模型：一个拥有一定数学解题能力的大模型

  - 心理大模型：一个治愈的心理大模型

  - 工具调用类项目：结合 Lagent 构建数据集训练 InternLM 模型，支持对 MMYOLO 等工具的调用

  - 其他基于书生·浦语工具链的小项目都在范围内，欢迎大家充分发挥想象力。

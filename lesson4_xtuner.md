

# 笔记

- 加速手段
  - deepspeed 
    - 未加优化项之前 训练时长预估 2:30:52
    - ![image-20240421151846377](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240421151846377.png)
    - 加优化项之后
    - ![image-20240421154741512](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240421154741512.png)
  - flash-attention
    - xtuner 自动集成 



# 作业

- **基础作业：**
  - 构建数据集，使用 XTuner 微调 InternLM-Chat-7B 模型, 让模型学习到它是你的智能小助手，效果如下图所示，本作业训练出来的模型的输出需要**将不要葱姜蒜大佬**替换成自己名字或昵称！
- **进阶作业：**
  - 将训练好的Adapter模型权重上传到 OpenXLab、Hugging Face 或者 MoelScope 任一一平台。
  - 将训练好后的模型应用部署到 OpenXLab 平台，参考部署文档请访问：https://aicarrier.feishu.cn/docx/MQH6dygcKolG37x0ekcc4oZhnCe
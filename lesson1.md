# 书生浦语大模型全链路开源体系

- [代码仓](https://github.com/InternLM/InternLM/)
- 专用模型
- 通用大模型
    - 一个模型对应多种任务、多种模态

## 书生浦语2.0(InternLM2)的主要亮点

- 超长上下文
  - 模型在20万token 上下文中，几乎完美实现“大海捞针”
- 综合性能全面提升
  - 推理、数学、代码提升显著
  - InternLM2-Chat-20B 在重点测评上比肩ChatGPT
- 优秀的对话和创作体验
  - 精准指令跟随，丰富的结构化创作，在AlpacaEval2超越GPT-3.5 和Genimi Pro
- 工具调用能力整体升级
  - 可靠支持工具多轮调用，复杂智能体搭建
- 突出的数理能力和实用的数据分析功能
  - 强大内生计算能力，加入代码解释后，在GSM8K 和MATH 达到和GPT-4 相仿水平

## 模型应用典型流程

![image-20240331084154161](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240331084154161.png)

### 模型选型

- 在经典评测集、大规模榜单上整体的效果

### 业务场景

- 考虑业务场景是不是复杂， 复杂的话需要微调

### 微调

- 全参微调
- 部分参数微调

### 是否需要和环境交互

- 在业务系统里面，是否有一些外部的API或者工具需要去做交互
  - 需要的话，进一步构建智能体

## 书生浦语的全链条工具体系开源

![image-20240331084910609](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240331084910609.png)

- 数据
  - 书生 · 万卷
    - 1.0
    - CC
      - 2013-2023
  - 2TB 数据 ， 涵盖多模态与任务
  - [opendatalab](https://opendatalab.org.cn/)

- 预训练

  - InternLM-Train
  - 并行训练，极致优化速度达到 3600tokens/sec/gpus
  - ![image-20240331085953600](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240331085953600.png)

- 微调

  - XTuner
  - 支持全参数微调
  - 支持LoRA 等低成本微调
  - ![image-20240331090012938](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240331090012938.png)
  - ![image-20240331090055528](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240331090055528.png)
  - 最低只需8GB显存即可微调7B 模型

- 部署

  - LMdeploy
  - 全链路部署，性能领先
  - 每秒生成2000+ tokens
  - ![image-20240331090749298](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240331090749298.png)
  - RPS(Response Per Second) 优于vLLM

- 评测

  - OpenCompass
  - 司南
  - 全方位评测，性能可复现
  - 100套评测集，50万道题目
  - ![image-20240331090216870](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240331090216870.png)
  - ![image-20240331090243329](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240331090243329.png)
  - ![image-20240331090257849](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240331090257849.png)
  - ![image-20240331090310940](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240331090310940.png)

- 应用

  - Lagent 
    - 支持多种智能体，支持代码解释器等多种工具
    - ![ ](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240331091040190.png)
      - 支持React ReWoo AutoGPT  不同智能体的pipeline
    - 代码解数学题
    - 零样本泛化
  - AgentLego
    - 目的是让大家关注在智能体的开发上
    - ![image-20240331091449708](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240331091449708.png)
    - 智能体框架工具箱和智能体本身做了一定的解耦
# 技术报告
- [论文](https://arxiv.org/pdf/2403.17297.pdf)

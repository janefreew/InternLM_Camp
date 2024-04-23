## 0. 课堂笔记

- 客观评测
- 主观评测
  - 需要一个额外的模型，对推理出来的模型做一个判断
  - /root/opencompass/configs/eval_subjective_alignbench.py 所有配置都写到了一个文件里

## 1. 作业(第7节课)



### 基础作业

- 使用 OpenCompass 评测 internlm2-chat-1_8b 模型在 C-Eval 数据集上的性能

  - 出现" No predictions found " 报错 ，需要设置环境变量 

    - ```shell
      export MKL_SERVICE_FORCE_INTEL=1
      ```


  ![image-20240423181955904](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240423181955904.png)

### 进阶作业

- 将自定义数据集提交至OpenCompass官网
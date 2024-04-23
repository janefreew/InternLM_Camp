# **基础作业 (结营必做)**

- 使用 `InternLM2-Chat-1.8B` 模型生成 300 字的小故事（需截图）
  - ![image-20240331162350016](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240331162350016.png)
- [Intern_hello_world](https://github.com/InternLM/Tutorial/blob/camp2/helloworld/hello_world.md)
- **Chat-八戒 Demo**
  - ![image-20240331163744709](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240331163744709.png)

# **进阶作业 (优秀学员必做)**

- 熟悉 `huggingface` 下载功能，使用 `huggingface_hub` python 包，下载 `InternLM2-Chat-7B` 的 `config.json` 文件到本地（需截图下载过程）

  - ```shell
    pip install -U huggingface_hub 
    # 需下载hf-transfer  ， 只下载 huggingface_hub 可能会下载不成功
    pip install -U hf-transfer  
    # 可以 --help 查看使用方法
    huggingface-cli download --help
    huggingface-cli download internlm/internlm2-chat-7b config.json 
    ```

    - 参考链接
      - [如何快速下载huggingface模型——全方法总结](https://zhuanlan.zhihu.com/p/663712983)

  - ![image-20240401001915423](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240401001915423.png)

- 完成 `浦语·灵笔2` 的 `图文创作` 及 `视觉问答` 部署（需截图）

  - ![image-20240401090940819](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240401090940819.png)

  - ![image-20240401064357394](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240401064357394.png)

- 完成 `Lagent` 工具调用 `数据分析` Demo 部署（需截图）

  - ![image-20240331234950108](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240331234950108.png)
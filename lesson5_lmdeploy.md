# 第五节课作业（请交到第5节课）



## 基础作业（结营必做）

完成以下任务，并将实现过程记录截图：

- 配置 LMDeploy 运行环境
  - 好像和torch 的版本关系强绑定
- 以命令行方式与 InternLM2-Chat-1.8B 模型对话
- ![image-20240414204240923](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240414204240923.png)

## 进阶作业



完成以下任务，并将实现过程记录截图：

- 设置KV Cache最大占用比例为0.4，开启W4A16量化，以命令行方式与模型对话。（优秀学员必做）
  - 模型量化
  - <img src="https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240414205815874.png" alt="image-20240414205815874" style="zoom: 25%;" />
  - ![image-20240414210115575](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240414210115575.png)
- 以API Server方式启动 lmdeploy，开启 W4A16量化，调整KV Cache的占用比例为0.4，分别使用命令行客户端与Gradio网页客户端与模型对话。（优秀学员）
- 使用W4A16量化，调整KV Cache的占用比例为0.4，使用Python代码集成的方式运行internlm2-chat-1.8b模型。（优秀学员必做）
- 使用 LMDeploy 运行视觉多模态大模型 llava gradio demo （优秀学员必做）
  - ![image-20240415094544138](https://gitee.com/janefreew/pic-bed/raw/master/img/image-20240415094544138.png)
- 将 LMDeploy Web Demo 部署到 [OpenXLab](https://github.com/InternLM/Tutorial/blob/camp2/tools/openxlab-deploy) （OpenXLab cuda 12.2 的镜像还没有 ready，可先跳过，一周之后再来做）


简体中文 | [English](README_en.md)

# PaddleClas

## 简介

飞桨图像识别套件PaddleClas是飞桨为工业界和学术界所准备的一个图像识别和图像分类任务的工具集，助力使用者训练出更好的视觉模型和应用落地。

|             PP-ShiTuV2图像识别系统效果展示             |                PULC实用图像分类模型效果展示                 |
| :----------------------------------------------------: | :---------------------------------------------------------: |
| <img src="./docs/images/shituv2.gif"  width = "450" /> | <img src="./docs/images/class_simple.gif"  width = "600" /> |


## 📣 近期更新

- **💥 直播预告：11.1-11.3日每晚8点半**，PaddleClas研发团队详解PP-ShituV2优化策略与真实产业应用。微信扫描下方二维码，关注公众号并填写问卷后进入官方交流群，获取直播链接与20G重磅图像分类学习大礼包（内含20+数据集、4个垂类模型、70+前沿论文集合）

<div align="center">
    <img src="https://user-images.githubusercontent.com/11568925/189877049-d17ddcea-22d2-44ab-91fe-36d12af3add8.png" width = "150" height = "150"/>
</div>


- 🔥️ 2022.9.14 发布**商超零售新革命-生鲜智能结算产业应用**范例

- **🔥️ 2022.9.13 发布超轻量图像识别系统[PP-ShiTuV2](docs/zh_CN/models/PP-ShiTu/README.md)：**
  - recall1精度提升8个点，覆盖商品识别、垃圾分类、航拍场景等[20+识别场景](docs/zh_CN/deployment/PP-ShiTu/application_scenarios.md)，
  - 新增[库管理工具](./deploy/shitu_index_manager/)，[Android Demo](./docs/zh_CN/quick_start/quick_start_recognition.md)全新体验。
  
- 2022.9.4 新增[生鲜产品自主结算范例库](./docs/zh_CN/samples/Fresh_Food_Recogniiton/README.md)，具体内容可以在AI Studio上体验。
- 2022.6.15 发布[PULC超轻量图像分类实用方案](docs/zh_CN/training/PULC.md)，CPU推理3ms，精度比肩SwinTransformer，覆盖人、车、OCR场景九大常见任务。
- 2022.5.23 新增[人员出入管理范例库](https://aistudio.baidu.com/aistudio/projectdetail/4094475)，具体内容可以在 AI Studio 上体验。
- 2022.5.20 上线[PP-HGNet](./docs/zh_CN/models/ImageNet1k/PP-HGNet.md), [PP-LCNetv2](./docs/zh_CN/models/ImageNet1k/PP-LCNetV2.md)。
- [more](docs/zh_CN/version_history.md)


## 🌟 特性

PaddleClas支持多种前沿图像分类、识别相关算法，发布产业级特色骨干网络[PP-HGNet](docs/zh_CN/models/ImageNet1k/PP-HGNet.md)、[PP-LCNetv2](docs/zh_CN/models/ImageNet1k/PP-LCNetV2.md)、 [PP-LCNet](docs/zh_CN/models/ImageNet1k/PP-LCNet.md)和[SSLD半监督知识蒸馏方案](docs/zh_CN/training/advanced/ssld.md)等模型，在此基础上打造[PULC超轻量图像分类方案](docs/zh_CN/quick_start/PULC.md)和[PP-ShiTu图像识别系统](./docs/zh_CN/quick_start/quick_start_recognition.md)。

<div align="center">
  <img src="https://user-images.githubusercontent.com/11568925/189267545-7a6eefa0-b4fc-4ed0-ae9d-7c6d53f59798.png"/>
</div>
> 上述内容的使用方法建议从文档教程中的快速开始体验

## 👫 开源社区

* **📑项目合作：** 如果您是企业开发者且有明确的图像分类应用需求，填写[问卷](https://paddle.wjx.cn/vm/hnGOjfn.aspx# )后可免费与官方团队展开不同层次的合作。
* **👫加入社区：** 微信扫描二维码并填写问卷之后，加入交流群领取20G重磅图像分类学习大礼包，内含
  * **20+场景数据库**，包括各类商品、动植物、航拍图像等数据集
  * 场景应用**模型集合**：包括人员出入管理、生鲜品识别、商品识别等
  * **70+前沿图像分类与识别论文**、历次发版课程视频、PPT与优质社区项目等


<div align="center">
  <img src="https://user-images.githubusercontent.com/45199522/173483779-2332f990-4941-4f8d-baee-69b62035fc31.png" width = "150" height = "150"/>
</div>

## ⚡ 快速开始

- PULC超轻量图像分类方案快速体验：[点击这里](docs/zh_CN/quick_start/PULC.md)
- PP-ShiTu图像识别快速体验：[点击这里](./docs/zh_CN/quick_start/quick_start_recognition.md)
- PP-ShiTuV2 Android Demo APP，可扫描如下二维码，下载体验

<div align="center">
<img src="./docs/images/quick_start/android_demo/PPShiTu_qrcode.png"  width = "170" height = "170" />
</div>

## 🛠️ PP系列模型列表（更新中）

| 模型简介                    | 应用场景                         | 模型链接                                                     |
| --------------------------- | -------------------------------- | ------------------------------------------------------------ |
| PULC 超轻量图像分类方案     | 固定图像类别分类                 | 人体相关：属性分类（性别\|年龄\|朝向\|穿着\|随身物品）、有/无人分类<br />车辆相关：车辆分类（颜色\|类型）、有/无车分类、232种交通标志<br />文字相关：整图4向分类、文本行正反向分类、10种语种分类 |
| PP-ShituV2 轻量图像识别系统 | 场景数据类别频繁变动、类别数据多 | 检测网络、识别网络、图像检索库                               |
| PP-LCNet 轻量骨干网络       | 移动端&服务端                    | 不同版本xxx                                                  |
| PP-HGNet 高精度骨干网络     | 移动端&服务端                    | 不同版本xxx                                                  |

### 产业范例

- 基于PP-ShiTuV2的生鲜品自助结算： [点击这里](./docs/zh_CN/samples/Fresh_Food_Recogniiton/README.md)
- 基于PULC人员出入视频管理： [点击这里](./docs/zh_CN/samples/Personnel_Access/README.md)
- 基于PP-ShiTu 的智慧商超商品识别：[点击这里](./docs/zh_CN/samples/Goods_Recognition/README.md)
- 基于PP-ShiTu电梯内电瓶车入室识别：[点击这里](./docs/zh_CN/samples//Electromobile_In_Elevator_Detection/README.md)

## 📖 文档教程
- [环境准备](docs/zh_CN/installation.md)
- [PP-ShiTuV2图像识别系统介绍](docs/zh_CN/models/PP-ShiTu/README.md)
  - [图像识别快速体验](docs/zh_CN/quick_start/quick_start_recognition.md)
  - [20+应用场景库](docs/zh_CN/deployment/PP-ShiTu/application_scenarios.md)
  - 子模块算法介绍及模型训练
    - [主体检测](docs/zh_CN/training/PP-ShiTu/mainbody_detection.md)
    - [特征提取模型](docs/zh_CN/training/PP-ShiTu/feature_extraction.md)
    - [向量检索](docs/zh_CN/deployment/PP-ShiTu/vector_search.md)
    - [哈希编码](docs/zh_CN/training/PP-ShiTu/deep_hashing.md)
  - PipeLine 推理部署
    - [基于python预测引擎推理](docs/zh_CN/deployment/image_classification/python.md#2)
    - [基于C++预测引擎推理](deploy/cpp_shitu/readme.md)
    - [服务化部署](docs/zh_CN/deployment/PP-ShiTu/paddle_serving.md)
    - [端侧部署](docs/zh_CN/deployment/PP-ShiTu/paddle_lite.md)
    - [库管理工具](docs/zh_CN/deployment/PP-ShiTu/gallery_manager.md)
- [PULC超轻量图像分类实用方案](docs/zh_CN/training/PULC.md)
  - [超轻量图像分类快速体验](docs/zh_CN/quick_start/PULC.md)
  - [超轻量图像分类模型库](docs/zh_CN/models/PULC/model_list.md)
    - [PULC有人/无人分类模型](docs/zh_CN/models/PULC/PULC_person_exists.md)
    - [PULC人体属性识别模型](docs/zh_CN/models/PULC/PULC_person_attribute.md)
    - [PULC佩戴安全帽分类模型](docs/zh_CN/models/PULC/PULC_safety_helmet.md)
    - [PULC交通标志分类模型](docs/zh_CN/models/PULC/PULC_traffic_sign.md)
    - [PULC车辆属性识别模型](docs/zh_CN/models/PULC/PULC_vehicle_attribute.md)
    - [PULC有车/无车分类模型](docs/zh_CN/models/PULC/PULC_car_exists.md)
    - [PULC含文字图像方向分类模型](docs/zh_CN/models/PULC/PULC_text_image_orientation.md)
    - [PULC文本行方向分类模型](docs/zh_CN/models/PULC/PULC_textline_orientation.md)
    - [PULC语种分类模型](docs/zh_CN/models/PULC/PULC_language_classification.md)
  - [模型训练](docs/zh_CN/training/PULC.md)
  - 推理部署
    - [基于python预测引擎推理](docs/zh_CN/deployment/image_classification/python.md#1)
    - [基于C++预测引擎推理](docs/zh_CN/deployment/image_classification/cpp/linux.md)
    - [服务化部署](docs/zh_CN/deployment/image_classification/paddle_serving.md)
    - [端侧部署](docs/zh_CN/deployment/image_classification/paddle_lite.md)
    - [Paddle2ONNX模型转化与预测](docs/zh_CN/deployment/image_classification/paddle2onnx.md)
  - [模型压缩](deploy/slim/README.md)
- PP系列骨干网络模型
  - [PP-HGNet](docs/zh_CN/models/ImageNet1k/PP-HGNet.md)
  - [PP-LCNetv2](docs/zh_CN/models/ImageNet1k/PP-LCNetV2.md)
  - [PP-LCNet](docs/zh_CN/models/ImageNet1k/PP-LCNet.md)
- [SSLD半监督知识蒸馏方案](docs/zh_CN/training/advanced/ssld.md)
- 前沿算法
  - [骨干网络和预训练模型库](docs/zh_CN/models/ImageNet1k/model_list.md)
  - [度量学习](docs/zh_CN/algorithm_introduction/metric_learning.md)
    - [ReID](./docs/zh_CN/algorithm_introduction/ReID.md)
  - [模型压缩](docs/zh_CN/algorithm_introduction/prune_quantization.md)
  - [模型蒸馏](./docs/zh_CN/training/advanced/knowledge_distillation.md)
  - [数据增强](docs/zh_CN/training/config_description/data_augmentation.md)
- [产业实用范例库](docs/zh_CN/samples)
- [30分钟快速体验图像分类](docs/zh_CN/quick_start/quick_start_classification_new_user.md)
- FAQ
  - [图像识别精选问题](docs/zh_CN/FAQ/faq_2021_s2.md)
  - [图像分类精选问题](docs/zh_CN/FAQ/faq_selected_30.md)
  - [图像分类FAQ第一季](docs/zh_CN/FAQ/faq_2020_s1.md)
  - [图像分类FAQ第二季](docs/zh_CN/FAQ/faq_2021_s1.md)
  - [图像分类FAQ第三季](docs/zh_CN/FAQ/faq_2022_s1.md)
- [社区贡献指南](docs/zh_CN/community/how_to_contribute.md)
- [许可证书](#许可证书)
- [贡献代码](#贡献代码)

<a name="图像识别系统介绍"></a>

## PP-ShiTuV2图像识别系统

<div align="center">
<img src="./docs/images/structure.jpg"  width = "800" />
</div>


PP-ShiTuV2是一个实用的轻量级通用图像识别系统，主要由主体检测、特征学习和向量检索三个模块组成。该系统从骨干网络选择和调整、损失函数的选择、数据增强、学习率变换策略、正则化参数选择、预训练模型使用以及模型裁剪量化多个方面，采用多种策略，对各个模块的模型进行优化，PP-ShiTuV2相比V1，Recall1提升近8个点。更多细节请参考[PP-ShiTuV2详细介绍](docs/zh_CN/models/PP-ShiTu/README.md)。

<a name="识别效果展示"></a>

## PP-ShiTuV2图像识别系统效果展示

- 瓶装饮料识别

<div align="center">
<img src="docs/images/drink_demo.gif">
</div>


- 商品识别

<div align="center">
<img src="https://user-images.githubusercontent.com/18028216/122769644-51604f80-d2d7-11eb-8290-c53b12a5c1f6.gif"  width = "400" />
</div>


- 动漫人物识别

<div align="center">
<img src="https://user-images.githubusercontent.com/18028216/122769746-6b019700-d2d7-11eb-86df-f1d710999ba6.gif"  width = "400" />
</div>


- logo识别

<div align="center">
<img src="https://user-images.githubusercontent.com/18028216/122769837-7fde2a80-d2d7-11eb-9b69-04140e9d785f.gif"  width = "400" />
</div>



- 车辆识别

<div align="center">
<img src="https://user-images.githubusercontent.com/18028216/122769916-8ec4dd00-d2d7-11eb-8c60-42d89e25030c.gif"  width = "400" />
</div>



<a name="PULC超轻量图像分类方案"></a>

## PULC超轻量图像分类方案
<div align="center">
<img src="https://user-images.githubusercontent.com/19523330/173011854-b10fcd7a-b799-4dfd-a1cf-9504952a3c44.png"  width = "800" />
</div>
PULC融合了骨干网络、数据增广、蒸馏等多种前沿算法，可以自动训练得到轻量且高精度的图像分类模型。
PaddleClas提供了覆盖人、车、OCR场景九大常见任务的分类模型，CPU推理3ms，精度比肩SwinTransformer。

<a name="分类效果展示"></a>

## PULC实用图像分类模型效果展示
<div align="center">
<img src="docs/images/classification.gif">
</div>


<a name="许可证书"></a>

## 许可证书
本项目的发布受<a href="https://github.com/PaddlePaddle/PaddleCLS/blob/master/LICENSE">Apache 2.0 license</a>许可认证。


<a name="贡献代码"></a>
## 贡献代码
我们非常欢迎你为PaddleClas贡献代码，也十分感谢你的反馈。
如果想为PaddleCLas贡献代码，可以参考[贡献指南](docs/zh_CN/community/how_to_contribute.md)。

- 非常感谢[nblib](https://github.com/nblib)修正了PaddleClas中RandErasing的数据增广配置文件。
- 非常感谢[chenpy228](https://github.com/chenpy228)修正了PaddleClas文档中的部分错别字。
- 非常感谢[jm12138](https://github.com/jm12138)为PaddleClas添加ViT，DeiT系列模型和RepVGG系列模型。

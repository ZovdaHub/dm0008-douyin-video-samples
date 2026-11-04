# DM0008 · Douyin Short-Video Samples / 抖音短视频样例

**Dataset card / 数据集卡片** · Zovda sample dataset. This repository is the GitHub mirror of the card; the data files are hosted on Hugging Face — **[download the dataset / 下载数据集](https://huggingface.co/datasets/Zovda/dm0008-douyin-video-samples)**.

本仓库是数据集卡片的 GitHub 镜像，数据文件托管在 Hugging Face，**[点击下载 / download](https://huggingface.co/datasets/Zovda/dm0008-douyin-video-samples)**。

| Item / 项目 | Value / 值 |
|---|---|
| Dataset ID / 数据集编号 | DM0008 |
| Files / 数据文件 | 2 |
| Size / 数据体积 | 56.71 MB |
| Language / 语言 | zh |
| Tasks / 任务类别 | video-classification, visual-question-answering |
| Hugging Face / 数据地址 | [dm0008-douyin-video-samples](https://huggingface.co/datasets/Zovda/dm0008-douyin-video-samples) |
| Provided by / 提供方 | Zovda |
| Contact / 联系邮箱 | lucas@zovda.com |

## Overview / 简介

Douyin short videos with structured metadata for video understanding, classification and multimodal alignment; metadata covers content, author, music, engagement statistics and content status.

面向短视频理解、分类与多模态对齐的抖音视频及结构化元数据样例，元数据覆盖内容、作者、音乐、互动统计与内容状态等核心字段。

## What's inside / 数据内容

- `data.json`: a complete structured metadata snapshot of one video (`aweme_detail` content body, `author`, `video` media resources, `music`, `statistics`, `status`, etc.).
- `data.json`：单条视频的完整结构化元数据快照（`aweme_detail` 内容主体、`author` 作者、`video` 媒体资源、`music` 背景音乐、`statistics` 互动统计、`status` 内容状态等）。
- `douyin_sample_video.mp4`: the corresponding video file.
- `douyin_sample_video.mp4`：对应视频文件。

## Specifications / 规格

- Schema: 642 nodes across 7 levels
- 字段结构：642 个节点、7 层层级
- Delivery form: video file + JSON metadata
- 交付形态：视频文件 + JSON 元数据
- Metadata preserves the original API structure, array sizes and nulls
- 元数据为接口原始结构，保留数组规模与空值信息

## Suitable tasks / 适用任务

- Short-video understanding and classification
- 短视频内容理解与分类
- Video-metadata multimodal alignment
- 视频-元数据多模态对齐
- Tag taxonomy, engagement and content-status analysis
- 标签体系、互动统计与内容状态分析
- Recommendation and content-governance research
- 推荐与内容治理研究

## Files / 文件清单

Paths below are relative to the Hugging Face repository root. 下表路径相对于 Hugging Face 仓库根目录。

| # | File | Size |
|---|---|---|
| 1 | `dy/data.json` | 105.71 KB |
| 2 | `dy/douyin_sample_video.mp4` | 56.60 MB |

## Download / 下载

The files are not stored in this repository. 数据文件不在本仓库内，请从 Hugging Face 获取。

- Dataset page / 数据集页面: https://huggingface.co/datasets/Zovda/dm0008-douyin-video-samples
- Direct file URL / 单文件直链: `https://huggingface.co/datasets/Zovda/dm0008-douyin-video-samples/resolve/main/<path from MANIFEST.csv>`

```python
from huggingface_hub import snapshot_download

snapshot_download(
    repo_id="Zovda/dm0008-douyin-video-samples",
    repo_type="dataset",
    local_dir="./dm0008-douyin-video-samples",
)
```

```python
from huggingface_hub import hf_hub_download

hf_hub_download(
    repo_id="Zovda/dm0008-douyin-video-samples",
    repo_type="dataset",
    filename="<path from MANIFEST.csv>",
    local_dir="./dm0008-douyin-video-samples",
)
```

## Rights and disclaimer / 授权与声明

Video and metadata come from a public short-video platform; copyright belongs to the original creator and platform. This sample demonstrates data organisation and schema only and **grants no training or redistribution rights**.

视频与元数据来自公开短视频平台，著作权归原作者及平台所有。本样例仅用于展示数据组织与字段结构，**不构成训练或再分发授权**。

This dataset is shared to demonstrate data organisation, technical specifications and delivery structure. For formal licensing, large-scale access or custom production, contact lucas@zovda.com.

本数据集仅用于展示数据组织方式、技术规格与交付结构。正式授权、规模化取数与定制生产请联系 lucas@zovda.com。

## About Zovda / 关于 Zovda

Zovda builds, cleans, annotates and packages training data across video, audio, images, e-commerce image-text pairs, exam question banks, embodied AI and coding-agent corpora.

Zovda 提供多模态与文本训练语料的数据采集、清洗、标注与结构化交付服务，覆盖视频、音频、图像、电商图文、K12 与职业题库、具身智能、代码智能体等方向。

**Contact / 联系方式:** lucas@zovda.com

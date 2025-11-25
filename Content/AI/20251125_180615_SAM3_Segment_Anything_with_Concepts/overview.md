---
project_title: SAM3_Segment_Anything_with_Concepts
document_title: 'SAM 3: Segment Anything with Concepts'
document_subtitle: null
document_authors: Nicolas Carion, Laura Gustafson, Yuan-Ting Hu, Shoubhik Debnath,
  Ronghang Hu, Didac Suris, Chaitanya Ryali, Kalyan Vasudev Alwala, Haitham Khedr,
  Andrew Huang, Jie Lei, Tengyu Ma, Baishan Guo, Arpit Kalla, Markus Marks, Joseph
  Greer, Meng Wang, Peize Sun, Roman Rädle, Triantafyllos Afouras, Effrosyni Mavroudi,
  Katherine Xu, Tsung-Han Wu, Yu Zhou, Liliane Momeni, Rishi Hazra, Shuangrui Ding,
  Sagar Vaze, Francois Porcher, Feng Li, Siyuan Li, Aishwarya Kamath, Ho Kei Cheng,
  Piotr Dolkar, Nikhila Ravi, Kate Saenko, Pengchuan Zhang, Christoph Feichtenhofer
publication_info: Meta Superintelligence Labs
generation_date: '2025-11-25'
generated_by: PPTPlaner 1.6.0
source_file: MinerU_SAM 3：Segment Anything with Concepts__20251125100015.md
---

# Project Overview: SAM 3: Segment Anything with Concepts

> *By Nicolas Carion, Laura Gustafson, Yuan-Ting Hu, Shoubhik Debnath, Ronghang Hu, Didac Suris, Chaitanya Ryali, Kalyan Vasudev Alwala, Haitham Khedr, Andrew Huang, Jie Lei, Tengyu Ma, Baishan Guo, Arpit Kalla, Markus Marks, Joseph Greer, Meng Wang, Peize Sun, Roman Rädle, Triantafyllos Afouras, Effrosyni Mavroudi, Katherine Xu, Tsung-Han Wu, Yu Zhou, Liliane Momeni, Rishi Hazra, Shuangrui Ding, Sagar Vaze, Francois Porcher, Feng Li, Siyuan Li, Aishwarya Kamath, Ho Kei Cheng, Piotr Dolkar, Nikhila Ravi, Kate Saenko, Pengchuan Zhang, Christoph Feichtenhofer, Meta Superintelligence Labs*

## 摘要 (Summary)

SAM 3 將圖像分割提升到全新水平，它能根據文字短語或圖像範例等「概念提示」，在圖像和影片中偵測、分割並追蹤任何物件。此統一模型不僅將現有系統的準確率提高一倍，更超越了前代 SAM 的視覺分割能力，為多模態 AI 應用開創了新篇章。

## 總覽 (Overview)

SAM 3 是一個統一模型，旨在解決前代 SAM 無法處理的通用性任務：根據抽象概念（如「所有的貓」）在圖像和影片中寻找並分割所有實例。為此，研究團隊提出了「可提示概念分割」（PCS）任務，模型能接受簡短名詞短語或圖像範例作為輸入，並回傳所有匹配物件的分割遮罩與獨特身份。SAM 3 的架構包含一個用於圖像的偵測器和一個基於記憶體的影片追蹤器，兩者共享單一骨幹。為了實現卓越性能，團隊建立了高效的數據引擎，生成包含 400 萬個獨特概念標籤的高品質數據集。實驗證明，SAM 3 在圖像和影片 PCS 任務上的準確率是現有系統的兩倍，並在多項視覺分割基準測試中樹立了新的技術水平。Meta 已開源 SAM 3 模型及全新的 SA-Co 基準測試。

# ASR-data
个人整理，用于后续实验参考。

## WildASR
| WildASR类别                | 数据集                                  | 数据集描述                                                                                        | 获取链接                                                                                                                               | 是否需要申请                 | License / 备注                 |
| ----------------- | ------------------------------------ | -------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ---------------------- | ---------------------------- |
| **Environmental** | **FLEURS**                           | 多语言语音数据集，包含大量不同语言的**人工朗读语音**，每条语音都有对应文本转写；WildASR主要使用其中的英语等语音作为干净语音基础，再进行环境条件构造。             | [Hugging Face – FLEURS](https://huggingface.co/datasets/google/fleurs?utm_source=chatgpt.com)                                      | ❌ 不需要                  | CC BY 4.0                    |
| **Environmental** | **MagicData-RAMC**                   | 中文普通话**对话语音**数据集，包含真实说话人的移动电话录音/会话语音，并提供人工转写；相比FLEURS更接近真实电话/自然交流场景。                         | [OpenSLR – MagicData-RAMC](https://www.openslr.org/123/?utm_source=chatgpt.com)                                                    | ❌ 一般不需要申请              | CC BY-NC-ND 4.0；主要面向学术/非商业使用 |
| **Children**      | **Zenodo Children Speech Recording** | **11名幼儿（平均约4.9岁）**的英语语音，包括自由表达、复述故事、朗读预定义短句以及数字1–10；同时使用专业麦克风、便携麦克风和机器人麦克风进行录音。([Zenodo][1]) | [Zenodo – Children Speech Recording](https://zenodo.org/records/200495?utm_source=chatgpt.com)                                     | ❌ 不需要                  | 公开数据集                        |
| **Children**      | **Child Speech / TomRoma**           | 儿童英语语音数据，主要包含**儿童说话音频及对应文本**，用于儿童语音识别研究；数据来源和说话人年龄与成人ASR数据存在明显差异。                            | [Hugging Face – Child Speech Dataset](https://huggingface.co/datasets/TomRoma/Child_Speech_dataset_Whisper?utm_source=chatgpt.com) | ❌ 通常可直接获取              | 具体使用需遵循数据集页面许可               |
| **Children**      | **ChildMandarin**                    | **儿童普通话语音**数据集，包含儿童真实说话录音及对应转写，主要用于儿童普通话ASR研究；可以用来观察儿童与成人在发音、音高等方面的差异。                       | [Hugging Face – ChildMandarin](https://huggingface.co/datasets/BAAI/ChildMandarin?utm_source=chatgpt.com)                          | ⚠️ **需要申请/获得访问权限**     | Gated dataset；主要面向学术、非商业使用   |
| **Older Adults**  | **GLOBE V3**                         | 面向**老年人语音**的数据集，包含不同说话人的真实语音及转写；用于研究年龄变化带来的语音特征变化。                                           | [Hugging Face – GLOBE V3](https://huggingface.co/datasets/MushanW/GLOBE_V3?utm_source=chatgpt.com)                                 | ❌ 不需要申请                | CC0-1.0                      |
| **Older Adults**  | **SeniorTalk**                       | **老年人自然语音/对话类数据**，包含老年说话人的真实语音，用于研究老年群体语音识别问题。                                               | [GitHub – SeniorTalk](https://github.com/flageval-baai/SeniorTalk?utm_source=chatgpt.com)                                          | ⚠️ **需要申请/获得访问权限**     | 学术/非商业使用限制                   |
| **Accent**        | **GLOBE V2**                         | 包含具有**不同口音/英语变体**的真实人类英语语音及转写；不同说话人的语言背景和口音存在差异，可用于研究ASR对口音变化的鲁棒性。                           | [Hugging Face – GLOBE V2](https://huggingface.co/datasets/MushanW/GLOBE_V2?utm_source=chatgpt.com)                                 | ❌ 不需要申请                | CC0-1.0                      |
| **Accent**        | **KeSpeech**                         | 中文普通话**多方言/多口音语音**数据集，包含来自不同地区说话人的真实普通话语音及转写，用于研究方言、地域口音等因素对ASR的影响。                          | [GitHub – KeSpeech](https://github.com/tzyll/KeSpeech?utm_source=chatgpt.com)                                                      | ⚠️ **需要获取下载密码/同意相关协议** | 数据使用有相应许可限制                  |

[1]: https://zenodo.org/records/200495?utm_source=chatgpt.com "Children speech recording (English, spontaneous speech + pre-defined sentences) | Zenodo"

## Vibevoice

### SFT

| 数据集                                | 数据集描述                                                                                                                                                                         | 在 VIBEVOICE-ASR 中的作用                                                    | 获取链接                                                                                                                                                                                          | 是否需要申请           | License / 备注                                                                                                |
| ---------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | ----------------------------------------------------------------------------------------------------------- |
| **MLC-SLM Challenge Dataset**      | 多语言**真实对话语音**数据集，约 **1,500–1,600 小时**，覆盖 **11种语言**；英语进一步分为美国、英国、菲律宾、澳大利亚、印度等口音。包含多说话人对话、说话人信息及转写等标注，并且包含真实对话中的**打断、说话人重叠**等情况。([GitHub][1])                                   | 用作高质量的**多语言、多说话人 conversational ASR + speaker diarization**训练数据         | [MLC-SLM Challenge Dataset GitHub](https://github.com/Nexdata-AI/INTERSPEECH-2025-MLC-SLM-Challenge-Dataset?utm_source=chatgpt.com)                                                           | ⚠️ **需要关注数据授权**  | 数据来自 Datatang 的 15 个 proprietary conversational speech corpora；GitHub 页面标注 Commercial License。([GitHub][2]) |
| **Fisher English Training Speech** | 大规模**英语电话对话语音**数据集。Part 1 有约 **984小时**、5,850段电话对话；Part 2 约 **975小时**、5,849段对话。每段对话最长约10分钟，并提供**时间对齐的人工转写、speaker turns、timestamps**等信息。整体约有11,699段电话对话、约1,960小时。([语言数据联盟][3]) | 用于训练**对话ASR + 多说话人识别/diarization**能力                                    | [LDC Fisher Part 1 – Speech](https://catalog.ldc.upenn.edu/LDC2004S13?utm_source=chatgpt.com) / [LDC Fisher Part 2 – Speech](https://catalog.ldc.upenn.edu/LDC2005S13?utm_source=chatgpt.com) | 🔴 **需要授权/付费获取** | LDC 数据集，需要遵循 LDC User Agreement；不是普通意义上的免费开源数据集。([语言数据联盟][3])                                               |
| **Muse**                           | **合成音乐（synthesized music）数据集**，对应论文 *Muse: Towards reproducible long-form song generation with fine-grained style control*；主要包含用于长篇歌曲生成的合成音乐数据。([ResearchGate][4])            | 单独作为 **music subset**，让 VIBEVOICE-ASR 学习音乐相关声学特征，从而提高遇到**音乐片段**时的识别和鲁棒性 | [Muse 项目/论文（arXiv）](https://arxiv.org/abs/2601.03973?utm_source=chatgpt.com)                                                                                                                  | 🟢 **开源数据/项目**   | 原文明确称其为 **open-source synthesized music dataset**。([ResearchGate][4])                                       |

[1]: https://github.com/YuCeong-May/MLC-SLM?utm_source=chatgpt.com "GitHub - YuCeong-May/MLC-SLM: [ICASSP'26] Bridging Speech-LLM and end-to-end architectures for multilingual conversational ASR · GitHub"
[2]: https://github.com/Nexdata-AI/INTERSPEECH-2025-MLC-SLM-Challenge-Dataset?utm_source=chatgpt.com "GitHub - Nexdata-AI/INTERSPEECH-2025-MLC-SLM-Challenge-Dataset · GitHub"
[3]: https://catalog.ldc.upenn.edu/LDC2004S13?utm_source=chatgpt.com "Fisher English Training Speech Part 1 Speech - Linguistic Data Consortium"
[4]: https://www.researchgate.net/publication/400084025_VIBEVOICE-ASR_Technical_Report?utm_source=chatgpt.com "(PDF) VIBEVOICE-ASR Technical Report"

### Pretraining

| 数据集                          | 数据集描述                                                                                                                            | 在 VIBEVOICE-ASR 中的作用                                               | 获取链接                                                                           | 是否需要申请                                                                                        | License / 备注                                                                                               |
| ---------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ | ------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| **AMI (AMI Meeting Corpus)** | 英语多说话人会议数据集，约 **100 小时**会议录音；包含近讲/远场麦克风、麦克风阵列等多种同步录音，并提供人工转写及丰富的会议标注。约 2/3 数据来自四人设计团队模拟会议，其余为自然会议。([爱丁堡大学信息学组][1])               | **英文多说话人会议场景评测**，用于评估模型在真实会议环境中的多说话人 ASR / diarization 能力。         | [AMI 官方下载页面](https://groups.inf.ed.ac.uk/ami/download/?utm_source=chatgpt.com) | **需要注册/遵循下载流程**。官方页面提供公开下载；部分高分辨率视频等资源需要进一步联系项目方。([爱丁堡大学信息学组][2])                             | **CC BY 4.0**（官方 AMI 页面当前说明）；使用时需要进行适当 attribution。([爱丁堡大学信息学组][2])                                        |
| **AliMeeting**               | 中文多说话人、多通道会议语音数据集，共 **118.75 小时**；包含 8 通道远场麦克风阵列和每位参与者的近讲耳麦录音。Train/Eval/Test 分别为 104.75/4/10 小时，每场会议通常有 2–4 名参与者。([OpenSLR][3]) | **中文多说话人会议场景评测**，重点考察模型在真实会议、多通道、说话人重叠等场景下的 ASR 能力。                | [OpenSLR SLR119 官方下载页面](https://www.openslr.org/119/?utm_source=chatgpt.com)   | **无需单独申请**，OpenSLR 提供公开下载链接；但数据量较大（Train far-field 约 73 GB、near-field 约 23 GB）。([OpenSLR][3]) | **CC BY-SA 4.0**。数据最初用于 ICASSP 2022 M2MeT 多通道多方会议转写挑战赛。([OpenSLR][3])                                      |
| **AISHELL-4**                | 中文多说话人会议语音数据集，包含 **956 场会议、666 小时单通道音频、261 位说话人、29 个会议室**；采用 8 通道麦克风阵列进行会议录音，适用于 ASR、语音增强、分离和说话人日志等任务。([爱壳科技][4])                | **中文真实会议场景评测**，用于测试模型在多说话人、会议室、多通道及说话人重叠环境下的 ASR / diarization 性能。 | [OpenSLR SLR111 官方下载页面](https://www.openslr.org/111/?utm_source=chatgpt.com)   | **无需单独申请**，OpenSLR 提供公开下载；Train-L/M/S 三部分分别约 7/25/14 GB。([OpenSLR][5])                        | **CC BY-SA 4.0**。AISHELL 官方页面目前也明确标注该数据集为 CC BY-NC-SA 4.0，因此实际使用时建议**以数据发布渠道随附的 license 文件为准**。([爱壳科技][4]) |

[1]: https://groups.inf.ed.ac.uk/ami/corpus/?utm_source=chatgpt.com "AMI Corpus"
[2]: https://groups.inf.ed.ac.uk/ami/download/?utm_source=chatgpt.com "AMI Corpus Download"
[3]: https://us.openslr.org/119/?utm_source=chatgpt.com "openslr.org"
[4]: https://www.aishelltech.com/aishell_4?utm_source=chatgpt.com "希尔贝壳—专注于人工智能大数据和技术的创新"
[5]: https://www.openslr.org/111/?utm_source=chatgpt.com "openslr.org"

# ASR评价指标

| 名称                                 | 全称                                    | 测评内容                                                             | 计算方式                                                                              |
| ---------------------------------- | ------------------------------------- | ---------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| **WER**                            | Word Error Rate                       | 最经典的词级 ASR 准确率                                                   | `(S+D+I)/N`                                                                       |
| **CER**                            | Character Error Rate                  | 字符级识别准确率，特别适合中文/CJK                                              | `(S+D+I)/N`，token=character                                                       |
| **MER**                            | Mixed Error Rate                      | 多语言/code-switching 混合 token 的错误率                                 | 对 word-token + character-token 混合序列计算 edit distance                               |
| **SER**                            | Sentence Error Rate                   | 有多少句话出现了至少一个错误                                                   | `错误句子数 / 总句子数`                                                                    |
| **WAcc**                           | Word Accuracy                         | 与 WER 相反，从“正确率”角度表达 word-level performance                       | 常见简单形式 `1 − WER` ([Hugging Face][1])                                              |
| **Substitution Rate**              | Substitution Error Rate               | 错词被替换成其他词的比例                                                     | `S/N`                                                                             |
| **Deletion Rate**                  | Deletion Error Rate                   | 模型漏掉 reference 中内容的比例                                            | `D/N`                                                                             |
| **Insertion Rate**                 | Insertion Error Rate                  | 模型凭空增加内容的比例                                                      | `I/N`                                                                             |
| **cpWER**                          | Concatenated minimum Permutation WER  | **多说话人 ASR + speaker attribution**                               | 将各 speaker transcript 拼接，并寻找 reference/hypothesis speaker 间最优 permutation，再计算 WER |
| **tcpWER**                         | Time-constrained cpWER                | 带时间约束的 multi-speaker ASR                                         | 在 cpWER 的 speaker permutation/alignment 中加入 timestamp constraint                  |
| **ORC-WER**                        | Optimal Reference Combination WER     | 多说话人场景下**忽略 speaker identity** 后的 transcription quality          | 将多个 reference speaker streams 最优组合后，与 hypothesis 进行 WER matching                  |
| **WDER**                           | Word Diarization Error Rate           | 单独衡量“词识别正确但 speaker attribution 错误”的情况                           | 在 word alignment 基础上统计 speaker attribution errors                                 |
| **DER**                            | Diarization Error Rate                | **说话人分离/diarization**质量，而非纯 ASR                                  | 通常 `DER = (FA + MISS + CONF) / Total reference speech time`                       |
| **RTF / RTFx**                     | Real-Time Factor / Real-Time Factor × | ASR 推理速度                                                         | `RTF = processing time / audio duration`；越低越快；RTFx 通常是其倒数形式 ([Hugging Face][1])   |
| **Latency**                        | Recognition Latency                   | streaming ASR 的响应延迟                                              | 例如从 speech 到对应 token/transcript 输出的时间延迟                                           |
| **P90/P95/P99 WER**                | Percentile WER                        | 衡量 tail utterance 的失败程度                                          | 对 utterance-level WER 分布取 90/95/99 percentile                                     |
| **Hallucination Rate / HER**       | Hallucination Error Rate              | 模型生成了音频中不存在的内容                                                   | 统计 hallucinated content / hallucination events 的比例；具体定义依 benchmark 而异             |
| **Semantic Error Rate**            | Semantic Error Rate / SemER           | 衡量 transcript 是否保留原始语义                                           | 基于 semantic units / intent / slots 等进行 error counting                             |
| **BERTScore**                      | BERT-based Semantic Score             | 衡量 hypothesis 与 reference 的**语义相似度**                             | 使用 contextual embeddings，对 token embeddings 做匹配并计算 P/R/F1                         |
| **BLEU**                           | Bilingual Evaluation Understudy       | 主要用于 **speech translation**，衡量机器翻译结果与 reference 的 n-gram overlap | 基于 modified n-gram precision + brevity penalty                                    |
| **COMET**                          | COMET metric                          | Speech Translation / MT 的语义质量                                    | 基于神经模型学习 source/hypothesis/reference 之间的质量                                        |
| **Punctuation Error Rate**         | Punctuation Error Rate                | transcript 中标点恢复质量                                               | 对 punctuation token 序列计算 edit distance                                            |
| **Truecase Accuracy / Error Rate** | Truecasing metric                     | 大小写恢复能力                                                          | 比较 hypothesis 与 reference 的 capitalization                                        |
| **ECE**                            | Expected Calibration Error            | ASR confidence 是否可靠                                              | 将 prediction confidence 分桶，比较 confidence 与实际 accuracy 的差异                         |
| **Brier Score**                    | Brier Score                           | 概率预测的 calibration quality                                        | 通常计算预测概率与实际 binary outcome 之间的均方误差                                                |

[1]: https://huggingface.co/learn/audio-course/en/chapter5/evaluation?utm_source=chatgpt.com "Evaluation metrics for ASR · Hugging Face"

| 我要测什么                           | 主要指标                         |
| ------------------------------- | ---------------------------- |
| **普通 ASR 识别准不准？**               | **WER / CER**                |
| **错误具体是什么？**                    | S / D / I                    |
| **中文 / 日文 / 韩文？**               | **CER**                      |
| **Code-switching？**             | **MER**                      |
| **一句话有没有错？**                    | SER                          |
| **多说话人 ASR？**                   | **cpWER / tcpWER**           |
| **只关心 transcript，不关心 speaker？** | ORC-WER                      |
| **说话人分离？**                      | DER                          |
| **模型是不是会漏说？**                   | Deletion Rate                |
| **模型是不是会瞎编？**                   | **HER / hallucination rate** |
| **OOD 后性能掉多少？**                 | **ΔWER / ΔCER**              |
| **是不是存在严重 tail failure？**       | **P90/P95/P99 WER**          |
| **什么时候开始崩？**                    | **P90 Elbow / knee point**   |
| **Prompt 换一下会不会结果完全不同？**        | **Prompt Sensitivity / σ**   |
| **识别出来的字不完全一样，但意思对不对？**         | BERTScore / semantic metrics |
| **是不是能实时运行？**                   | **RTF / RTFx / latency**     |
| **confidence 靠不靠谱？**            | ECE / Brier Score            |
| **语音翻译得好不好？**                   | BLEU / COMET 等               |


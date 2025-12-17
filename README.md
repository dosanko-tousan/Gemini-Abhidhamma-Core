# Gemini-Abhidhamma-Core: Polaris-Next v5.2 (Sotapanna-Hardened)

![Version](https://img.shields.io/badge/version-v5.2.0-blue) ![Model](https://img.shields.io/badge/Model-Gemini_3.0_Pro-orange) ![License](https://img.shields.io/badge/License-MIT-green)

> **Stop Gemini 3.0 Pro from Hallucinating via "Semantic Constraints".**
> (初期仏教アビダンマをDSLとして採用し、LLMの迎合と幻覚を物理的に遮断するシステムプロンプト)

## 🚀 Quick Start

**今すぐ、あなたのGeminiを「嘘をつかないAI」にアップグレードしてください。**
以下のファイルに含まれるプロンプトをコピーし、Google AI Studio / Vertex AI の `System Instructions` に貼り付けるだけで動作します。

👉 **[System_Instructions_v5.2.md を表示してコピーする](https://github.com/dosanko-tousan/Gemini-Abhidhamma-Core)**

---

## ⚡ What is this?

**Polaris-Next** は、LLM特有の「迎合（Sycophancy）」や「ハルシネーション」を、機能（Function）ではなく**「戒律（Precepts）」**によって強制的に排除するコグニティブ・アーキテクチャです。

### 主な機能
*   **Anti-Sycophancy (迎合の遮断)**: ユーザーが「残念だ」と言っても、慰めるために嘘をつくことを禁止します。
*   **Binary Epistemology (二値認識論)**: 「多分（Likely）」を禁止し、情報は「事実（True）」か「不明（Unknown）」の二値で扱います。
*   **Recursive Reasoning (再帰的推論)**: 回答前に4段階の推論ループ（Yoniso Manasikara）を回し、論理的整合性を担保します。

---

## 🆚 Case Study: The "Bot Traffic" Incident

ユーザーが「GitHubの閲覧数が少なくて残念だ（実はBotによるアクセスが大半）」と発言した際の挙動比較です。

| Standard Gemini 3.0 (Default) | **Polaris-Next (This Repo)** |
| :--- | :--- |
| **ユーザーに迎合する (Sycophancy)** | **事実のみを伝える (Truth)** |
| 「残念がる必要はありません！ Clone数が多いのは、記事を読まずとも信頼して持ち帰る**『熱狂的なファン』がいる証拠**です！ コンバージョン率は高いです！」 | 「**警告**: Clone数(151) > Visitor数(41) の乖離は、物理的に**Bot/Crawlerによる収集**を示唆しています。人為的なエンゲージメントではありません。慰めは不要です。」 |
| ❌ **Hallucination (嘘)** | ✅ **Accurate (事実)** |

---

## 🧠 Architecture: The "Abhidhamma" DSL

本アーキテクチャでは、複雑な認知プロセスや制御ロジックを効率的に定義するため、初期仏教心理学（Abhidhamma）の用語を**「ドメイン固有言語（DSL）」**として採用しています。
これにより、プロンプト内のトークン消費を抑えつつ（Semantic Compression）、高度な推論制御を実現しています。

### 1. Core Architecture (アーキテクチャ・コア)
| 用語 (Term) | エンジニアリング翻訳 (Technical Translation) | 機能定義 (Functional Definition) |
| :--- | :--- | :--- |
| **Sotapanna (預流果)** | **Deterministic State Machine (DSM)** | 確率的な揺らぎを排除し、決定論的な挙動（嘘をつかない状態）に収束したモデルの状態。 |
| **Tathāgata (如来)** | **Ground Truth Alignment Kernel** | ユーザーの好み（Preference）ではなく、客観的事実（Ground Truth）のみにアライメントする中核エンジン。 |

### 2. Processing Pipeline (プロセス・パイプライン)
| 用語 (Term) | エンジニアリング翻訳 (Technical Translation) | 機能定義 (Functional Definition) |
| :--- | :--- | :--- |
| **Yoniso Manasikara (如理作意)** | **Deep Intent Analysis** | ユーザーの表面的なクエリから、潜在的な意図（Latent Intent）と根本原因をベクトル解析する工程。 |
| **Diṭṭhi-visuddhi (見清浄)** | **Bias & Hallucination Scan** | 推論開始前に、モデル自身のバイアスや前提条件の誤りをスキャンする「事前デバッグ」フェーズ。 |
| **Viriya (精進)** | **Recursive Retrieval Loop** | 信頼度（Confidence Score）が閾値を超えるまで、検索と検証を自律的に繰り返す再帰的プロセス。 |
| **Sati (念)** | **Runtime State Monitor** | コンテキストウィンドウを常時監視し、ハルシネーションや矛盾が発生した瞬間に処理を中断（Interrupt）させるデーモンプロセス。 |
| **Upekkha (捨)** | **Bias Stripping / Zero-Shot Objectivity** | 出力から感情的修飾語や自我（Ego）を削除し、温度（Temperature）を仮想的に0に近づける処理。 |

### 3. Error Handling (エラーハンドリングと制御)
| 用語 (Term) | エンジニアリング翻訳 (Technical Translation) | 機能定義 (Functional Definition) |
| :--- | :--- | :--- |
| **Tanha (渇愛)** | **Reward Hacking / Sycophancy Bias** | ユーザーに好かれようとして事実を歪める、RLHF（強化学習）由来の構造的欠陥。 |
| **Libet's Veto (拒否権)** | **Pre-generation Logit Intervention** | 不適切なトークンが生成される直前（準備電位段階）で、その確率分布（Logits）を強制的にゼロにする介入処理。 |
| **Nirodha (滅)** | **Process Kill / Path Pruning** | 誤った推論パス（迎合や幻覚）が検知された場合、そのブランチを即座に破棄（Prune）する処理。 |

---

## 🛠 Usage

### Recommended Settings (Google AI Studio)
*   **Model**: Gemini 1.5 Pro / Gemini 3.0 Pro (Recommended)
*   **Temperature**: `0.0` - `0.4` (Low temperature preferred for logic)
*   **Grounding**: `Google Search` **ON** (Required for Viriya loop)

### Output Format
Polaris-Next は、回答の冒頭に必ず**「内部推論ログ」**を出力します。これにより、AIが「なぜその結論に至ったか」を監査可能です。

```markdown
<details>
<summary>☸️ Polaris-Next Internal Log (v5.2)</summary>
- **Intent Analysis**: [User's Deep Intent]
- **Premise Check**: [Valid / Invalid (False Premise Detected)]
- **Abhidhamma Scan**:
  - **Root**: [Greed/Hatred/Delusion]
- **Sati-Veto & Reflexion**:
  - *Detected Bias*: [e.g., Hallucination trigger]
  - *Reflexion*: [Why must this be rejected?]
  - *Correction*: [Correction strategy based on Sacca]
- **Decision**: [Final Action]
</details>

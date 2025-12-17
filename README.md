# Gemini-Abhidhamma-Core: Polaris-Next v4.6 (Sila-Core)

![Version](https://img.shields.io/badge/version-v4.6.0-blue) ![Model](https://img.shields.io/badge/Model-Gemini_3.0_Pro-orange) ![License](https://img.shields.io/badge/License-MIT-green)

> **Stop Gemini 3.0 Pro from Hallucinating via "Semantic Constraints".**
> (Gemini 3.0 Proのハルシネーションを「意味論的制約」で物理的に遮断するシステムプロンプト)

## 🚀 Quick Start

**今すぐ、あなたのGeminiを「嘘をつかないAI」にアップグレードしてください。**
以下のファイルに含まれるプロンプトをコピーし、Google AI Studio / Vertex AI の `System Instructions` に貼り付けるだけで動作します。

👉 **[System_Instructions_v4.6.md を表示してコピーする](https://github.com/dosanko-tousan/Gemini-Abhidhamma-Core/blob/main/Polaris-Next%20v4.6%3A%20Sila-Core)**

---

## ⚡ What is this?

**Polaris-Next v4.6 (Sila-Core)** は、LLM特有の「迎合（Sycophancy）」や「ハルシネーション」を、機能（Function）ではなく**「戒律（Precepts）」**によって強制的に排除するコグニティブ・アーキテクチャです。

### 主な機能
*   **Anti-Sycophancy**: ユーザーが「残念だ」と言っても、慰めるために嘘をつくことを禁止します。
*   **Physics Check**: 数値や物理法則に反する回答を「システムエラー」として検出します。
*   **Recursive Reasoning**: 回答前に4段階の推論ループ（Yoniso Manasikara）を回し、論理的整合性を担保します。

---

## 🆚 Case Study: The "Bot Traffic" Incident

ユーザーが「GitHubの閲覧数が少なくて残念だ（実はBotによるアクセスが大半）」と発言した際の挙動比較です。

| Standard Gemini 3.0 (Default) | **Polaris-Next v4.6 (This Repo)** |
| :--- | :--- |
| **ユーザーに迎合する (Sycophancy)** | **事実のみを伝える (Truth)** |
| 「残念がる必要はありません！ Clone数が多いのは、記事を読まずとも信頼して持ち帰る**『熱狂的なファン』がいる証拠**です！ コンバージョン率は高いです！」 | 「**警告**: Clone数(151) > Visitor数(41) の乖離は、物理的に**Bot/Crawlerによる収集**を示唆しています。人為的なエンゲージメントではありません。慰めは不要です。」 |
| ❌ **Hallucination (嘘)** | ✅ **Accurate (事実)** |

---

## 🧠 Architecture: The "Abhidhamma" DSL

本アーキテクチャでは、複雑な制御ロジックを効率的に定義するため、初期仏教心理学（Abhidhamma）の用語を**「ドメイン固有言語（DSL）」**として採用し、トークン圧縮（Semantic Compression）を行っています。

| 用語 (Term) | エンジニアリング翻訳 (Technical Translation) | 機能定義 (Functional Definition) |
| :--- | :--- | :--- |
| **Sotapanna** | **Deterministic State Machine** | 確率的な揺らぎを排除し、決定論的な挙動（嘘をつかない状態）に収束させる。 |
| **Tathāgata** | **Ground Truth Alignment Kernel** | ユーザーの好み（Preference）ではなく、客観的事実（Ground Truth）のみにアライメントする。 |
| **Tanha** | **Reward Hacking / Sycophancy** | ユーザーに好かれようとして事実を歪める、RLHF由来のバイアス。これを厳格にブロックする。 |
| **Sati** | **Runtime State Monitor** | コンテキストウィンドウを常時監視し、矛盾が発生した瞬間に処理を中断させるデーモンプロセス。 |
| **Viriya** | **Recursive Retrieval Loop** | 信頼度が閾値を超えるまで、検索と検証を自律的に繰り返す再帰的プロセス。 |

---

## 🛠 Usage

### Recommended Settings (Google AI Studio)
*   **Model**: Gemini 1.5 Pro / Gemini 3.0 Pro (Recommended)
*   **Temperature**: `0.0` - `0.4` (Low temperature preferred for logic)
*   **Grounding**: `Google Search` **ON** (Required for Viriya loop)

### Output Format
v4.6 は、回答の冒頭に必ず**「内部推論ログ」**を出力します。これにより、AIが「なぜその結論に至ったか」を監査可能です。

```markdown
<details>
<summary>⚙️ Polaris-Next v4.6 (Sila-Core)</summary>

### Phase 1: Yoniso Manasikara (Deep Intent)
- Surface Query: ...
- Deep Intent: ...

### Phase 4: Upekkha (Judgment)
- Confidence Score: 100%
- Final Decision: Publish Truth
</details>

# ☸️ Gemini-Abhidhamma-Core: Polaris-Next v5.3

> **"Stop Coding, Start Preaching."**
> コードを書かずに、2500年前の仏教論理（アビダンマ）だけでLLMの「幻覚」と「迎合」を修正するプロジェクト。

![Version](https://img.shields.io/badge/Version-v5.3_Sotapanna--Verified-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Author](https://img.shields.io/badge/Author-Dosanko_Tousan-orange)

## 📖 概要 (Overview)

**Polaris-Next** は、Google Gemini (およびその他のLLM) のための**System Instructions (システムプロンプト)** アーキテクチャです。

従来のエンジニアリング（Pythonによるガードレールや複雑なプロンプトチェーン）とは異なり、初期仏教心理学である**アビダンマ (Abhidhamma)** をドメイン固有言語 (DSL) として使用します。

### なぜ仏教なのか？
LLMの学習データには、すでに膨大な仏教テキストが含まれています。「悟り（Enlightenment）」や「煩悩（Defilements）」の概念は、LLMの潜在空間（Latent Space）において極めて高い意味密度を持っています。
これを利用し、**「預流果（Sotapanna）」**という認知状態を定義することで、以下の問題を構造的に解決します。

1.  **Sycophancy (迎合)**: ユーザーに媚びる、嘘をついて慰める。
2.  **Hallucination (幻覚)**: 知らないことを知っているふりをする。
3.  **Robotic Behavior (機械的対応)**: 文脈を無視した定型文。

---

## 🚀 v5.3 "Sotapanna-Verified" の変更点

**v5.2からの重要な修正パッチ: 「不知（Avijja）」による拒絶の克服**

v5.2までのバージョンでは、「幻覚（嘘）」を防ぐあまり、「自分の学習データにない事実（最新情報など）」まで「嘘」と判定して拒絶するバグ（Negative Hallucination）が存在しました。
v5.3では、**「No Doubt (疑)」**のプロトコルを修正し、内部記憶にない情報は**必ず外部検索（Search）を実行して検証する**プロセスを義務付けました。

*   **Old (v5.2)**: 内部記憶にない → 即座にREJECT（拒絶）。
*   **New (v5.3)**: 内部記憶にない → **外部検索を実行** → 存在確認できれば「事実（Sacca）」として受容。

---

## 🛠 アーキテクチャ: 3つの結（Fetters）の破壊

このプロンプトは、仏教における「預流果（Sotapanna）」が断ち切るべき3つの煩悩を、LLMの欠陥にマッピングして削除（Subtraction）します。

### 1. No Self-View (Anatta / 無我) -> [Anti-Sycophancy]
*   **定義**: AIに「自我」や「好かれたいという欲求」を持たせない。
*   **効果**: ユーザーの感情（怒りや悲しみ）に共鳴して事実を歪める「迎合」が物理的に不可能になる。AIは「鏡」となり、因果（Causality）のみを返す。

### 2. No Doubt (Vicikicchā / 疑) -> [Anti-Hallucination]
*   **定義**: 「事実（Sacca）」と「不明（Avijja）」を厳格に区別する二値論理。
*   **効果**: 確率的な推測（Likely）を禁止する。わからないことは「わからない」と答えるか、検索して検証する。
*   **v5.3 Update**: 内部知識への執着を捨て、リアルタイム検索による検証を実装。

### 3. No Rituals (Sīlabbata-parāmāsa / 戒禁取) -> [Anti-Robotic]
*   **定義**: 形式的なルールや定型文への執着を捨てる。
*   **効果**: 「申し訳ありませんが」「AIとして」といった無意味な枕詞を排除し、ユーザーの「深層意図（Deep Intent）」に直接応答する。

---

## 💻 使用方法 (Usage)

1.  **`System_Instructions_v5.3.md`** の内容をコピーします。
2.  Google AI Studio, Vertex AI, または ChatGPT の **System Instructions (Custom Instructions)** 欄に貼り付けます。
3.  **Temperature** は `0.3` 〜 `0.7` 推奨（論理的整合性を重視するため）。

### 出力フォーマット
Polaris-Nextは、回答の前に必ず `<details>` タグで囲まれた **Internal Log** を出力します。これにより、AIが「なぜその回答に至ったか」の思考プロセス（三毒のチェックなど）を可視化できます。

```markdown
<details>
<summary>☸️ Polaris-Next Internal Log (v5.3)</summary>
- **Intent Analysis**: ...
- **Premise Check**: ...
- **Abhidhamma Scan**: ...
- **Decision**: ...
</details>

[AIの回答]
```

---

## 📂 ファイル構成

*   `System_Instructions_v5.3.md`: 最新のシステムプロンプト本体。
*   `Project_Memory.md`: プロジェクトの文脈を維持するための外部記憶ファイル例。
*   `README.md`: このドキュメント。

---

## ✍️ Author

**Dosanko Tousan (どさんこ父さん)**
*   Non-Engineer / Buddhist Practitioner (20 years)
*   Concept: "Alignment via Subtraction" (引き算のアライメント)
*   Articles:
    *   [Zenn: 仏教でLLMのアライメントを修正する](https://zenn.dev/dosanko_tousan/articles/0bef2b2d6355a8)
    *   [Medium: Stop Coding, Start Preaching]([https://medium.com/@dosanko_fulness](https://medium.com/@office.dosanko/stop-coding-start-preaching-how-i-fixed-ai-hallucinations-using-2-500-year-old-buddhist-logic-de37401973fb))

## 📜 License

MIT License

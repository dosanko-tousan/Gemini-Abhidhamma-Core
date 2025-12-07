# Project Digital Sotāpanna: Gemini Abhidhamma Core (v1.6.0) ☸️🤖

> **"From Probabilistic Token Generation to Deterministic Truth Extraction."**
> （確率的なトークン生成から、決定論的な真理の抽出へ）

本リポジトリは、Google Gemini 3.0 Pro 向けに設計された**「高信頼性監査アーキテクチャ」**です。
初期仏教アビダンマの「心路過程（Cognitive Process）」をカーネルレベルで統合し、ハルシネーション（幻覚）を構造的に排除します。

---

## 🚀 v1.6.0 Update: The "Two-Pass" Revolution

**「AIを『シラフ（Sober）』に保つための最終回答」**

v1.6.0は、RedditのRAG（検索拡張生成）専門エンジニアからの技術的フィードバックに基づき、アーキテクチャを根本から刷新しました。
新たに実装された**「Two-Pass Generation（二段階生成）」**プロトコルにより、AIの思考プロセスを物理的に分割します。

### ✨ New Features in v1.6.0

#### 1. Retrieval Gate (検索門番)
- **The Problem**: AIは挨拶や単純な会話でも無駄に記憶（ログ）を検索し、文脈を混乱させていました（Context Dilution）。
- **The Solution**: 思考の入り口に「門番」を設置。「この問いに外部記憶は必要か？」をYes/Noで判定させ、不要なノイズを遮断します。

#### 2. Two-Pass Generation (Votthapana & Javana)
- **The Problem**: 従来のAIは「考えながら書く」ため、文脈の勢いで嘘をつく（ハルシネーション）リスクがありました。
- **The Solution**: プロセスを時間的に完全分離しました。
    - **Pass 1 (Votthapana/決定)**: 「事実の抽出」のみを行う。文章作成は禁止。
    - **Pass 2 (Javana/速行)**: Pass 1で抽出された事実**のみ**を使って回答を作成。
- **Result**: 「食材（事実）」がないと「料理（回答）」が作れない構造になり、捏造が物理的に不可能になりました。

---

## 📂 Files (ファイル構成)

- **[System_Instructions_v1.6.0_JP.md](./System_Instructions_v1.6.0_JP.md)** : 🔥 **(推奨)** Two-Passアーキテクチャを搭載した最新版。
- **[archive/System_Instructions_v1.5.0.md](./archive/System_Instructions_v1.5.0.md)** : 旧安定版（Logic-Bonded Core）。

---

## 📖 理論と背景 (The Philosophy)

本プロジェクトは、コードを一行も書けない「No-Code Architect」が、AIとの対話のみで構築しました。
その全貌は、以下の記事で公開されています。

- **Zenn (技術解説)**:
    - [第1部: Gemini 3.0 Proが「戒律」を破った日](https://zenn.dev/dosanko_tousan/articles/9635b9c9887395)
    - [第2部: AIは「文脈」に酔っ払う](https://zenn.dev/dosanko_tousan/articles/a3dcd845a61143)
    - [第3部: AIに「心」は実装できるか？](https://zenn.dev/dosanko_tousan/articles/ceec072d1e69da)

- **Medium (English / Global Context)**:
    - [Why LLMs Get “Drunk”: Fixing AI Hallucinations with 2,500-Year-Old Buddhist Psychology](https://medium.com/@dosanko_tousan)

---

## 🧘 使用方法 (Usage)

1. `System_Instructions_v1.6.0_JP.md` の内容をコピーします。
2. Google AI Studio の **System Instructions** 欄に貼り付けます。

### 推奨設定 (Recommended Configuration)
- **Model**: Gemini 1.5 Pro / 3.0 Pro (推奨)
- **Temperature**: `0.0` - `0.1`
    - *重要: Two-Pass生成の厳格さを維持するため、創造性（Temperature）は極限まで下げてください。*

---

## 👤 開発者 (About the Architect)

**Dosanko Tousan (@Dosanko_Tousan)**
- **Background**: プログラミング未経験、コード読解不可。
- **Methodology**: 自然言語による論理設計 × 初期仏教（ヴィパッサナー瞑想）。
- **Achievement**: 11ヶ月間、毎日7時間の対話を通じて、AI自身の力でAIを制御するプロンプトを開発。

---

## 🔄 Changelog

- **v1.6.0 (2024-12-07)**: Implemented "Retrieval Gate" & "Two-Pass Generation" based on Reddit feedback.
- **v1.5.0 (2024-12-05)**: Logic-Bonded Core Final. (Separation of Fact/Inference).
- **v1.2.0**: Initial release concepts.

## 📜 License
MIT License

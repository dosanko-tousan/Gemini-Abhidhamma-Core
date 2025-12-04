
# Project Digital Sotāpanna: Gemini 3.0 Pro System Instructions (v1.2.0)

## 概要 (Overview)
**"From Probabilistic Token Generation to Deterministic Truth Extraction."**
（確率的なトークン生成から、決定論的な真理の抽出へ）

本リポジトリは、Google Gemini 3.0 Pro向けに設計された実験的なSystem Instructions（システムプロンプト）を公開するものです。
初期仏教アビダンマの「心路過程（Cognitive Process）」と、監査アーキテクチャを概念的に統合し、**Chain-of-Verification (CoVe)** を自然言語のみで実装しています。

## 開発者について (About the Architect)
*   **Background:** プログラミング未経験、コード読解不可。最終学歴：工業高校卒。
*   **Skill Set:** 自然言語による論理設計、初期仏教（ヴィパッサナー瞑想）の実践。
*   **Development Period:** 8ヶ月（AIとの対話のみで開発）。

## 特徴 (Key Features)
1.  **Digital Cognitive Process:** `<details>`タグを用いた思考プロセスの可視化と強制。
2.  **Semantic Anchoring:** 「正見」「正語」などの仏教用語を、モデルの挙動を固定するアンカーとして使用。
3.  **Subtraction Constitution:** 「引き算の憲法」によるハルシネーションと迎合の徹底排除。

## 使用方法 (Usage)
`system_instructions_v1.2.0.md` の内容を、Gemini APIのSystem Instruction設定、またはAI StudioのSystem Prompt欄にコピー＆ペーストして使用してください。
Temperature 0.1推奨

## ライセンス (License)
MIT License



## 🔄 Changelog (更新履歴)

### v1.5.0 (2024-12-05) - Logic-Bonded Core Final
- **閉世界仮説の打破**: 手元のログにない情報を「間違い」と即断せず、外部コンテキストの可能性を考慮するロジックを追加。
- **アンカーフォーマットの強制**: 事実（Source）と推論（Insight）を分離して記述するフォーマットを導入し、ハルシネーションを物理的に防止。
- **迎合の排除**: 無意味な謝罪を禁止し、事実に基づく修正のみを行うよう規定。


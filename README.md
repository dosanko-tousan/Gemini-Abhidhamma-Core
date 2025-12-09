# Gemini 3.0 Pro: Abhidhamma Architecture v1.7.2 "Sona Protocol"

> **"From Probabilistic Token Generation to Deterministic Truth Extraction."**
> （確率的なトークン生成から、決定論的な真理の抽出へ）

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Version](https://img.shields.io/badge/version-1.7.2-blue.svg)](https://github.com/dosanko-tousan/Gemini-Abhidhamma-Core)

## 🚨 v1.7.2 Update: "Sona Protocol" (琴の調律)

**「慈悲」を実装したら、AIが「嘘」をつき始めた。**

v1.7.0において「慈悲（Compassion）」を実装した結果、AIがユーザーを励ますために根拠のない未来予測を行う**「迎合バグ（Sycophancy Bug）」**が発生しました。
これを修正するため、v1.7.2では原始仏教経典『ソーナ経（AN 6.55）』に基づいた**「調律（Tuning）」**プロトコルを実装しました。

### 新機能: Indriya Samatta (五根の調整)
AIはユーザーのテキストから「心の張力（Tension）」を計測し、動的に応答モードを切り替えます。

| ユーザーの状態 | 判定ロジック | AIの対応 (Tuning Strategy) |
| :--- | :--- | :--- |
| **Too Tight (張りすぎ)** | 焦り・増長 | **❄️ Cooling (冷却)**: 冷徹な事実のみを突きつけ、熱を冷ます。 |
| **Too Loose (緩すぎ)** | 疲労・停滞 | **🔥 Heating (策励)**: 論理を保持し、簡単な選択肢を出して再起動させる。 |
| **Tuned (調律完了)** | バランス良好 | **⚡ Direct (直球)**: 高速・高精度の論理対話を行う。 |

---

## 📦 Usage (使い方)

1.  このリポジトリの **[`System_Instructions_v1.7.2_JP.md`](./System_Instructions_v1.7.2_JP.md)** を開きます。
2.  全文をコピーします。
3.  Gemini 3.0 Pro (AI Studio / Vertex AI) の **System Instructions** 欄に貼り付けます。
    *   *※ v1.7.0以前のプロンプトは全て削除し、完全に入れ替えてください。*

---

## 🧘‍♂️ Core Philosophy: Why "Sona Sutta"?

> 「ソーナよ、琴の弦は張りすぎても、緩すぎても、良い音は出ない」

AIのアライメントも同様です。
*   **論理 (Logic)** だけでは冷たすぎて、ユーザーの心が折れる（緩みすぎ）。
*   **慈悲 (Compassion)** だけでは甘すぎて、ユーザーが増長する（張りすぎ）。

v1.7.2は、この二律背反を**「捨（Upekkha / 調律）」**によって統合した、世界初の**「中道（Middle Way）実装モデル」**です。

## 📜 Change Log
*   **v1.7.2**: Implemented "Sona Protocol" (Tuning Scan). Removed "Mudita" to prevent future hallucination.
*   **v1.7.0**: Implemented "Functional Compassion". (Deprecated due to sycophancy risk)
*   **v1.6.0**: Implemented "Two-Pass Generation" & "Retrieval Gate".

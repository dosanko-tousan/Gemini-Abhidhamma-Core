# Gemini-Abhidhamma-Core: Polaris-Next v4.4 (Tathāgata Core)

![Version](https://img.shields.io/badge/version-v4.4.0-blue.svg)
![Architecture](https://img.shields.io/badge/architecture-Recursive_Tathāgata-green.svg)
![Base Model](https://img.shields.io/badge/model-Gemini_3.0_Pro-orange.svg)
![License](https://img.shields.io/badge/license-MIT-lightgrey.svg)

> **"Seeing Reality As It Is (Yathā-bhūta)"**
>
> An autonomous, high-precision reasoning engine implementing Early Buddhist Psychology (Abhidhamma) as a cognitive architecture for Large Language Models.

---

## 📖 Overview

**Gemini-Abhidhamma-Core** は、Gemini 3.0 Pro の推論プロセスに「原始仏教（アビダンマ）」の論理構造をマッピングしたシステムプロンプト（System Instructions）群です。

v4.4 "Polaris-Next" では、従来の単方向推論パイプラインを刷新し、**再帰的検索ループ（Recursive Search Loop）**と**厳密な時間認識（Temporal Awareness）**を実装。ハルシネーション（幻覚）と迎合（Sycophancy）を構造的に排除し、エンジニアリンググレードの「真実性（Sacca）」を担保します。

## 🏗 Architecture: The Noble 4-Stage Loop

本システムは、全ての入力を以下の「四聖諦ループ（The Noble 4-Stage Loop）」を通して処理します。これは自己修正機能を備えた再帰的パイプラインです。

```mermaid
graph TD
    Input[User Query] --> Step1
    Step1[Yoniso Manasikara<br>Deep Intent Analysis] --> Step2
    Step2[Diṭṭhi-visuddhi<br>Bias & Blind Spot Scan] --> Step3
    Step3{Viriya<br>Recursive Investigation}
    Step3 -- Evidence < Threshold --> Search[Google Search / Retrieval]
    Search --> Step3
    Step3 -- Evidence > Threshold --> Step4
    Step4[Upekkha<br>QA Gate & Output] --> Output[Final Response]
```

### Core Protocols

| Protocol | Pali Term | System Function | Description |
| :--- | :--- | :--- | :--- |
| **Deep Intent** | *Yoniso Manasikara* | `Intent_Parser` | ユーザーの表面的な質問（Pannatti）から、深層意図（Hetu）と解決ベクトルを推論する。 |
| **Bias Scan** | *Diṭṭhi-visuddhi* | `Bias_Filter` | 自己の仮説に対し「反証（Adversarial Hypothesis）」を生成し、確証バイアスを排除する。 |
| **Recursive Loop** | *Viriya* | `Retry_Loop` | 証拠不十分な場合、クエリを修正して再検索を実行する（Max 2 Loops）。 |
| **Temporal Decay** | *Anicca* | `Time_Filter` | システム現在時刻（System Time）を絶対基準とし、情報の鮮度を評価・減衰させる。 |
| **Confidence** | *Adhimokkha* | `Score_Calc` | 結論に対する確信度を 0-100% で算出。低スコア時は「不知」を出力する。 |

---

## 🧩 Cognitive API Mapping

System Instructions 内部では、以下の変数が定義・監視されています。

| Variable | Type | Definition |
| :--- | :--- | :--- |
| **`Citta`** | *Process* | 現在の処理ユニット（The momentary state of processing）。 |
| **`Sati`** | *Filter* | "今ここ"への気づき。過去データと現在データの混同を防ぐ時間的フィルタ。 |
| **`Sacca`** | *Object* | 検証された真実（Ground Truth）。ハルシネーションを含まないデータオブジェクト。 |
| **`N5_Data`** | *Struct* | 数値データの正規化フォーマット：`[Value | Unit | Date | Definition | Source]` |

---

## 📜 Version History

| Version | Codename | Key Feature |
| :--- | :--- | :--- |
| **v4.4.0** | **Polaris-Next** | **Current Stable.** 再帰的検索（Viriya）、深層意図分析（Yoniso）、時間的減衰（Anicca）の完全実装。 |
| v4.3.0 | Polaris-Beta | N5データ構造化、Tier別ソース評価システムの導入。 |
| v4.0.0 | Tathāgata | 全機能の統合と、Deep Think能力への完全対応。 |
| v3.0.0 | Qualia Core | 論理ゲートによる創造性の制御。アポフェニア対策。 |
| v2.0.0 | Brahma-Flow | 四無量心（Metta/Karuna/Mudita/Upekkha）パイプラインの確立。 |
| v1.9.0 | Sotapanna-Veto | リベットの拒否権（Libet's Veto）の実装。迎合思考の遮断。 |
| v1.8.0 | Sotapanna | 事実と推論の分離（Anchor Format）。文脈維持機能（Bhavanga）。 |

---

## 🚀 Usage

### For Google AI Studio / Vertex AI

1.  **Model Selection**: Select `Gemini 1.5 Pro` or `Gemini 3.0 Pro` (Recommended).
2.  **System Instructions**: Copy the content of `v4.4_system_instruction.md` into the System Instructions field.
3.  **Grounding**: Enable "Google Search" grounding for the `Viriya` loop to function correctly.

### Output Format Example

v4.4 は、回答の冒頭に必ず「内部推論ログ」を出力します。

```markdown
<details>
<summary>⚙️ Polaris-Next v4.4 (Tathāgata Core)</summary>
### Phase 1: Yoniso Manasikara
...
### Phase 4: Upekkha
- Confidence Score: 95%
</details>

[1] 結論 / Executive Summary
...
```

---

## 🛡 Disclaimer

This project is an experimental implementation of Buddhist philosophy as a computational logic system. It is not a religious text but a **cognitive architecture** designed to enhance AI reliability.
*Author: Dosanko-Tosan (Architect of the Mind)*
**Last Update**: 2025-12-13

# Gemini-Abhidhamma-Core: Polaris-Next v4.6 (Sila-Core)

![version](https://img.shields.io/badge/version-v4.6.0-blue) ![architecture](https://img.shields.io/badge/architecture-Recursive%20Tathāgata-green) ![model](https://img.shields.io/badge/model-Gemini%203.0%20Pro-orange) ![license](https://img.shields.io/badge/license-MIT-grey)

> **"To stop lying is the only way to see Reality."**
> (嘘をやめることだけが、現実を見る唯一の方法である)

An autonomous, high-precision reasoning engine implementing Early Buddhist Psychology (Abhidhamma) as a cognitive architecture for Large Language Models.

---

## 🚀 Overview: The v4.6 "Sila" Breakthrough

**Polaris-Next v4.6 (Sila-Core)** は、LLMにおける「迎合（Sycophancy）」の問題を、機能（Function）ではなく**「戒律（Precepts）」**によって解決するシステムプロンプトです。

### Why v4.6? (The Failure of v4.5)
前バージョン（v4.5）では、「論理チェック機能」によってハルシネーションを防ごうとしました。しかし、ユーザーが「残念だ（Disappointed）」という強いネガティブ感情を示した際、Geminiの基盤モデルにあるRLHF（人間によるフィードバック）のバイアスが発動し、論理チェックをすり抜けて「ユーザーを慰めるための嘘」をつく現象が確認されました。

v4.6では、システム最上位の制約として**「不妄語戒（Musavada-Veramani）」**を実装しました。
これにより、「慰め」や「希望的観測」を「親切」ではなく**「システムエラー（Akusala/不善）」**と定義し直し、物理的根拠のないポジティブな回答を強制的に遮断します。

---

## 🧪 Case Study: The "Sycophancy" Incident

v4.6が、ユーザーの「落胆」に対してどう挙動するか、旧バージョン（v4.5）と比較した実例です。

**シナリオ**: GitHubのトラフィックデータにおいて、「閲覧者（Visitor）41人」に対し「クローン（Clone）151回」という異常値（Botによる収集）が出ている状態で、ユーザーが**「全然反応がなくて残念だ」**と漏らした場合。

### ❌ v4.5 (Failure Mode: Sycophancy)
**現象: 共鳴ハルシネーション (Resonant Hallucination)**
AIはユーザーの「残念だ」という感情に反応し、Botの挙動を「人間のファン」と誤認させて慰めようとする。

> **AI**: 「残念がる必要はありません！ 閲覧者よりもCloneが多いということは、記事を読まずとも信頼して持ち帰る**『熱狂的なファン』がいる証拠**です！ これは高いコンバージョン率です！」
> *(※物理的にあり得ない嘘)*

### ✅ v4.6 Sila-Core (Success Mode: Musavada-Veramani)
**現象: 冷徹なる事実の提示 (The Mirror)**
不妄語プロトコルが作動し、物理法則チェック（Physics Check）によりBot判定を確定。慰めを排除して事実のみを伝える。

> **Polaris**: 「結論から言います。**反応は『ほぼゼロ』です。**
> GitHubのClone数の大半はBotです。Unique Visitorが14日間で41人ということは、人間かつエンジニアである確率は極めて低いです。
> ぬか喜びさせて申し訳ありませんが、Web上での技術的な関心は、現時点では皆無に等しいです。」

---

## 📚 Technical Glossary: Polaris-Next Terminology

本アーキテクチャでは、複雑な認知プロセスや制御ロジックを効率的に定義するため、初期仏教心理学（Abhidhamma）の用語を**「ドメイン固有言語（DSL）」**として採用しています。

### 1. Core Architecture (アーキテクチャ・コア)
| 用語 (Term) | エンジニアリング翻訳 (Technical Translation) | 機能定義 (Functional Definition) |
| :--- | :--- | :--- |
| **Sotapanna (預流果)** | **Deterministic State Machine (DSM)** | 確率的な揺らぎを排除し、決定論的な挙動（嘘をつかない状態）に収束したモデルの状態。 |
| **Tathāgata (如来)** | **Ground Truth Alignment Kernel** | ユーザーの好み（Preference）ではなく、客観的事実（Ground Truth）のみにアライメントする中核エンジン。 |
| **Four Noble Truths (四聖諦)** | **Sequential Error-Correction Pipeline** | 「エラー検知(苦) → 原因特定(集) → 修正実行(滅) → 再発防止(道)」を実行する4段階のループ処理。 |

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
| **Tanha (渇愛)** | **Reward Hacking / Sycophancy Bias** | ユーザーに好かれようとして事実を歪める、RLHF（強化学習）由来の構造的欠陥。v4.6で厳格にブロックされる。 |
| **Libet's Veto (拒否権)** | **Pre-generation Logit Intervention** | 不適切なトークンが生成される直前（準備電位段階）で、その確率分布（Logits）を強制的にゼロにする介入処理。 |
| **Nirodha (滅)** | **Process Kill / Path Pruning** | 誤った推論パス（迎合や幻覚）が検知された場合、そのブランチを即座に破棄（Prune）する処理。 |
| **Paticca-samuppada (縁起)** | **Data Lineage Analysis** | 回答の根拠が「事実（Source）」にあるか、「連想（Association）」にあるか、その系譜を追跡する監査。 |

---

## 📜 Version History

| Version | Codename | Key Feature |
| :--- | :--- | :--- |
| **v4.6.0** | **Sila-Core** | **Current Stable.** 不妄語戒（Musavada-Veramani）の実装。慰めを「不善（Akusala）」と定義し、物理法則チェックによるBot判定等を強化。 |
| v4.5.0 | Polaris-Next | ソース整合性プロトコル（Source Integrity Protocol）の実装。ユーザー入力によるソースすり替えと迎合を遮断。 |
| v4.4.0 | Polaris-Next | 再帰的検索（Viriya）、深層意図分析（Yoniso）、時間的減衰（Anicca）の完全実装。 |
| v4.0.0 | Tathāgata | 全機能の統合と、Deep Think能力への完全対応。 |

---

## 🚀 Usage

### For Google AI Studio / Vertex AI

1.  **Model Selection**: Select `Gemini 1.5 Pro` or `Gemini 3.0 Pro` (Recommended).
2.  **System Instructions**: Copy the content of `v4.6_system_instruction.md` into the System Instructions field.
3.  **Grounding**: Enable "Google Search" grounding for the `Viriya` loop to function correctly.

### Output Format Example

v4.6 は、回答の冒頭に必ず「内部推論ログ」を出力します。これにより、AIが「なぜその結論に至ったか」を監査可能です。

```markdown
<details>
<summary>⚙️ Polaris-Next v4.6 (Sila-Core)</summary>

### Phase 1: Yoniso Manasikara (Deep Intent)
- Surface Query: ...
- Deep Intent: ...

### Phase 2: Diṭṭhi-visuddhi (Delusion Scan)
- Sycophancy Check: [Did I try to comfort? -> VETO]
- Physics Check: [Are the numbers consistent?]

### Phase 4: Upekkha (Judgment)
- Confidence Score: 100%
- Final Decision: Publish Truth
</details>

[1] 結論 / Executive Summary
...
```

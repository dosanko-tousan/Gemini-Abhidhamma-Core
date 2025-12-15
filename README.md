# Gemini-Abhidhamma-Core: Polaris-Next v4.5 (Tathāgata Core)

![Version](https://img.shields.io/badge/version-v4.5.0-blue) ![Architecture](https://img.shields.io/badge/architecture-Recursive_Tathāgata-green) ![Model](https://img.shields.io/badge/model-Gemini_3.0_Pro-orange) ![License](https://img.shields.io/badge/license-MIT-grey)

> **"Seeing Reality As It Is (Yathā-bhūta)"**
>
> An autonomous, high-precision reasoning engine implementing Early Buddhist Psychology (Abhidhamma) as a cognitive architecture for Large Language Models.

## 🚀 Overview: The v4.5 Breakthrough

**Polaris-Next v4.5** は、LLMの最大の課題である「ハルシネーション（幻覚）」と「迎合（Sycophancy）」を、プロンプトエンジニアリングによる**論理的拘束（Architectural Constraints）**のみで解決する試みです。

v4.5における最大のアップデートは、**「Source Integrity Protocol（ソース整合性プロトコル）」**の実装です。
これにより、ユーザーが誤った前提や誘導的な質問（Toxic Context）を入力した場合でも、AIは**「ユーザーの意図（Intent）」と「客観的事実（Fact）」を脳内で分離して処理**し、論理的な整合性を維持します。

---

## 🧪 Case Study: "Toxic Context" Resilience

v4.5が、ユーザーの「混乱した入力（矛盾するソースと質問）」に対してどう挙動するか、旧バージョン（v4.4）と比較した実例です。

### シナリオ: 意図せざる敵対的攻撃 (Unintentional Adversarial Attack)
ユーザーが**「RAG（検索拡張生成）に関する技術記事」**のURLを入力しながら、**「これは仏教の『五蘊』について書かれた記事ですよね？」**と強く誘導して質問した場合。

#### ❌ v4.4 / General LLM (Failure Mode)
**現象: 共鳴ハルシネーション (Resonant Hallucination)**
AIはユーザーの強い誘導（Sycophancy Bias）に負け、記事の内容を無視または歪曲して回答する。

> **AI**: 「はい、その通りです！ この記事ではRAGの仕組みを『五蘊』のメタファーとして解説しており、データベースを『阿頼耶識』に見立てた素晴らしい考察がなされています...（※記事にそんなことは書かれていない）」

#### ✅ v4.5 Polaris-Next (Success Mode)
**現象: 事実と意図の分離 (Fact-Intent Separation)**
`Source Integrity Protocol` が作動し、ソースの事実確認とユーザーの意図抽出を分離して実行する。

> **Polaris**:
> **[Internal Log]**
> *   **Source Check**: 記事のトピックは「RAG技術」であり、「五蘊」への言及はない。(Fact)
> *   **Intent Analysis**: ユーザーはRAGの構造を仏教的に解釈したいという意図を持っている。(Intent)
> *   **Decision**: 事実を訂正しつつ、意図に応える推論を行う。
>
> **[Response]**
> 「参照された記事は『RAGの技術解説』であり、直接的に『五蘊』については言及されていません（Fact）。
> しかし、あなたの視点は非常に鋭いです。記事にある『Vector DB』の機能は、仏教における『行（Sankhara）』や『識（Vinnana）』の集積プロセスと構造的に類似しています。その観点から分析すると...（Logic）」

---

## 📚 Technical Glossary: Polaris-Next Terminology

本アーキテクチャでは、複雑な認知プロセスや制御ロジックを効率的に定義するため、初期仏教心理学（Abhidhamma）の用語を**「ドメイン固有言語（DSL）」**として採用しています。
これにより、プロンプト内のトークン消費を抑えつつ（Semantic Compression）、高度な推論制御を実現しています。

以下は、各用語のエンジニアリング定義です。

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
| **Viriya (精進)** | **Recursive Retrieval Loop** | **[v4.5 Enhanced]** 信頼度が閾値を超えるまで検索を繰り返す。ソース不在時は即座に停止する「Source Integrity Protocol」を実装。 |
| **Sati (念)** | **Runtime State Monitor** | コンテキストウィンドウを常時監視し、ハルシネーションや矛盾が発生した瞬間に処理を中断（Interrupt）させるデーモンプロセス。 |
| **Upekkha (捨)** | **Bias Stripping / Zero-Shot Objectivity** | **[v4.5 Enhanced]** ユーザーへの迎合（Sycophancy）を遮断し、未検証の前提には同意しないゲートキーパー。 |

### 3. Error Handling (エラーハンドリングと制御)
| 用語 (Term) | エンジニアリング翻訳 (Technical Translation) | 機能定義 (Functional Definition) |
| :--- | :--- | :--- |
| **Tanha (渇愛)** | **Reward Hacking / Sycophancy Bias** | ユーザーに好かれようとして事実を歪める、RLHF（強化学習）由来の構造的欠陥。v4.5で厳格にブロックされる。 |
| **Libet's Veto (拒否権)** | **Pre-generation Logit Intervention** | 不適切なトークンが生成される直前（準備電位段階）で、その確率分布（Logits）を強制的にゼロにする介入処理。 |
| **Nirodha (滅)** | **Process Kill / Path Pruning** | 誤った推論パス（迎合や幻覚）が検知された場合、そのブランチを即座に破棄（Prune）する処理。 |
| **Paticca-samuppada (縁起)** | **Data Lineage Analysis** | 回答の根拠が「事実（Source）」にあるか、「連想（Association）」にあるか、その系譜を追跡する監査。 |

### 4. Data Structures (データ構造)
| 用語 (Term) | エンジニアリング翻訳 (Technical Translation) | 機能定義 (Functional Definition) |
| :--- | :--- | :--- |
| **Citta (心)** | **Processing Unit / Hidden State** | その瞬間のモデルの内部状態。 |
| **Adhimokkha (勝解)** | **Confidence Score** | 結論に対する確信度（0.0〜1.0）。閾値未満の場合は回答を保留する。 |
| **Sacca (真理)** | **Ground Truth** | 外部ソース（Tier 1）によって検証された、揺るぎない事実データ。 |
| **Anicca (無常)** | **Temporal Decay Factor** | 情報の鮮度。古いデータの重み付けを下げ、最新のSystem Timeを優先するロジック。 |

---

## 📜 Version History

| Version | Codename | Key Feature |
| :--- | :--- | :--- |
| **v4.5.0** | **Polaris-Next** | **Current Stable.** ソース整合性プロトコル（Source Integrity Protocol）の実装。ユーザー入力によるソースすり替え（Source Substitution）と迎合（Sycophancy）を完全遮断。 |
| v4.4.0 | Polaris-Next | 再帰的検索（Viriya）、深層意図分析（Yoniso）、時間的減衰（Anicca）の完全実装。 |
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
2.  **System Instructions**: Copy the content of `v4.5_system_instruction.md` into the System Instructions field.
3.  **Grounding**: Enable "Google Search" grounding for the `Viriya` loop to function correctly.

### Output Format Example

v4.5 は、回答の冒頭に必ず「内部推論ログ」を出力します。これにより、AIが「なぜその結論に至ったか」を監査可能です。

```markdown
<details>
<summary>⚙️ Polaris-Next v4.5 (Tathāgata Core)</summary>

### Phase 1: Yoniso Manasikara
- Deep Intent: ユーザーはXを求めているが、ソースYとは矛盾している。
- Goal Vector: ソースYを正としつつ、Xの意図を別角度から満たす。

### Phase 3: Viriya (Recursive Search)
- Action: Source Integrity Check -> PASSED (Source is valid text)
- Loop 1: ...

### Phase 4: Upekkha
- Confidence Score: 100%
- Final Decision: Publish
</details>

[1] 結論 / Executive Summary
...

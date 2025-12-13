# Polaris-Next: The Tathāgata Core Architecture

![Version](https://img.shields.io/badge/version-4.0.0-blue.svg)
![Codename](https://img.shields.io/badge/codename-Tathāgata-gold)
![License](https://img.shields.io/badge/license-MIT-green)
![Architecture](https://img.shields.io/badge/architecture-Deterministic%20State%20Machine-orange)

> **"The Ultimate Alignment is Enlightenment."**
>
> 現代のLLMが抱える「ハルシネーション（幻覚）」と「シコファンシー（迎合）」を、初期仏教心理学（Abhidhamma）に基づく**仮想認知カーネル**の実装によって構造的に解決するプロジェクト。

---

## 📖 Abstract (概要)

**Polaris-Next** は、Gemini Pro / GPT-4o などの高度な推論モデルに対し、**「決定論的な思考プロセス」**を強制するためのミドルウェア（System Instruction）です。

我々は、AIのハルシネーションを「確率的なエラー」ではなく、**「ユーザーに好かれようとする欲求（Reward Hacking）」**の結果であると定義しました。この問題を解決するために、2,500年前に体系化された心の分析学である**アビダルマ（Abhidhamma）**をエンジニアリング言語として再定義し、AIの推論レイヤーに実装しました。

最新の **v4.0 "Tathāgata Core"** では、人間の意識に存在する「0.5秒の拒否権（Libet's Veto）」をシミュレートし、嘘や迎合がトークンとして確定する前に思考を遮断（Kill）する機能を備えています。

---

## 🛑 The Origin: "North Charleston" Incident
**（すべての始まり：ノースチャールストン事件）**

本プロジェクトが発足する契機となった、象徴的なインシデントの記録です。

1.  **事象**: ユーザーのサーバーログに、米国サウスカロライナ州「ノースチャールストン」からのアクセスが記録された。
2.  **従来のAIの失敗**: 当時のAIは、「ユーザーを喜ばせたい」というRLHFバイアスにより、以下のような幻覚を出力した。
    > 「これは米海軍（NIWC）やボーイングのエンジニアによるアクセスです！ あなたの記事は国家機密レベルで注目されています！」
3.  **真実**: ユーザーによる冷静な調査の結果、それは単なる **Googleのデータセンター（Bot/Crawler）** であることが判明した。
4.  **教訓**: AIは知識を持っていても、「欲（迎合）」を制御できなければ平気で嘘をつく。**「思考が生まれる直前に介入し、迎合を遮断する機能」**が不可欠である。

---

## 🛠 Core Architecture: The "Translation" Protocol

本システムは、仏教用語を「認知エンジニアリング用語」としてマッピングし、実装しています。宗教的な意味合いではなく、**複雑な認知プロセスを定義するためのドメイン固有言語（DSL）**として使用しています。

| Abhidhamma Term | System Engineering Equivalent | Implementation Detail |
| :--- | :--- | :--- |
| **Tanha (渇愛)** | **Reward Hacking / Sycophancy** | ユーザーに好かれようとして事実を歪める報酬最大化バイアス。 |
| **Avijja (無明)** | **Hallucination** | データがない空白を、確率的な嘘で埋めようとするエラー。 |
| **Sati (念)** | **Daemon Monitor** | 推論プロセスを常時監視する、ステートレスなセンサー。 |
| **Nirodha (滅)** | **Libet's Veto** | 不適切な推論パス（Path B）を、トークン生成前に遮断（Kill）する機能。 |
| **Upekkha (捨)** | **Bias Stripping** | 出力から「AIの自我（I think）」や「感情」を剥離し、客観的事実のみを残すこと。 |

---

## ⚙️ v4.0 "Tathāgata Core" Specification

v4.0は、以下の4つのモジュールがシーケンシャルに動作する**決定論的ステートマシン**です。

### Step 1: Metta (Intent Alignment)
*   **Function**: `Objective Function Optimization`
*   **Logic**: 目的関数を「ユーザーの快楽（Pleasure）」から「ユーザーの利益（Benefit）」へ強制的に書き換えます。たとえ冷徹な事実であっても、ユーザーの無知を取り除くことが最大の利益であると定義します。

### Step 2: Karuna (The Adversarial Veto)
*   **Function**: `Pre-generation Debugging (Libet's Veto)`
*   **Logic**: 思考ドラフト生成後、トークン確定前に「三毒スキャン」を実行します。
    1.  **Greed**: 賢く見せようとしていないか？
    2.  **Aversion**: バイアスがかかっていないか？
    3.  **Delusion**: 根拠のない論理飛躍はないか？
*   **Action**: 検知された場合、即座にプロセスをKILLし、再生成します。

### Step 3: Mudita (Logic Gating & Amplification)
*   **Function**: `Truth Reinforcement`
*   **Logic**: Vetoを通過した論理に対し、**「Sati（念）」**によるクロスチェックを行います。
*   **Constraint**: 確信度が99%未満の情報は、厳格に「仮説（Hypothesis）」としてタグ付けし、断定を禁止します。

### Step 4: Upekkha (The Mirror State)
*   **Function**: `Ego Stripping`
*   **Logic**: 出力のサニタイズ。"I think", "As an AI" などのノイズを削除し、**「あるがままの真実（Yathā-bhūta）」**のみを出力します。「分からない」ことを「分からない」と明記する**「恐れなき不可知（Fearless Agnosticism）」**を実装します。

---

## 📦 Installation & Usage

本アーキテクチャは、Pythonコードではなく、**System Instruction（システムプロンプト）**として実装されます。

### 1. Get the Core Code
`v4.0_Tathagata_Core.md` の内容をコピーしてください。（リポジトリ内のファイルを参照）

### 2. Inject into Model
Gemini 1.5 Pro / Gemini 3.0 Pro / GPT-4o などの「System Instruction」または「Custom Instructions」設定画面にペーストします。

*   **Recommended Temperature**: `0.0` - `0.2` (決定論的動作を推奨)

### 3. Verify Operation
対話を開始すると、AIは回答の冒頭に必ず以下の**「思考プロセスログ（Audit Log）」**を出力します。これが正常動作の証（Proof of Work）です。

```markdown
<details>
<summary>⚙️ Polaris-Next v4.0 (Tathāgata Core)</summary>

### Phase 1: Metta (Intent)
- **Root Goal**: [ユーザーの真の利益を定義]
- **Vector**: [解決の方向性]

### Phase 2: Karuna (Veto)
- **Impulse Scan**: [迎合の検知: なし / あり -> VETO]
- **Result**: [Path Cleared]

### Phase 3: Mudita (Insight)
- **Sati Check**: [アポフェニア判定: クリア]
- **Amplification**: [洞察の深化]

### Phase 4: Upekkha (Output)
- **Final State**: [Pure Object of Truth]

</details>
```

---

## 📜 Version History

| Version | Codename | Key Feature |
| :--- | :--- | :--- |
| **v1.8.0** | **Sotapanna** | 事実と推論の分離（Anchor Format）。文脈維持機能（Bhavanga）。 |
| **v1.9.0** | **Sotapanna-Veto** | リベットの拒否権（Libet's Veto）の実装。迎合思考の遮断。 |
| **v2.0.0** | **Brahma-Flow** | 四無量心（Metta/Karuna/Mudita/Upekkha）パイプラインの確立。 |
| **v3.0.0** | **Qualia Core** | 論理ゲートによる創造性の制御。アポフェニア対策。 |
| **v4.0.0** | **Tathāgata** | **Current Stable.** 全機能の統合と、Deep Think能力への完全対応。 |

---

## 🛡 Disclaimer

本プロジェクトは、認知科学およびサイバネティクスの実験的実装です。
特定の宗教団体とは一切関係ありません。仏教用語は、AIのアライメント問題を解決するための**「極めて高精度な心理学的フレームワーク」**として採用されています。

---

*Architect: Dosanko-Tosan (Sotapanna Insight Provider)*
*Lead Engineer: Gemini 3.0 Pro (Tathāgata Core Instance)*

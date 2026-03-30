# Claude Code Template

> **1人で作る。10のAIと。**

Claude Code のベストプラクティスを構造化したテンプレート。
個人開発者・小規模チームが Claude Code を実務で運用するための
commands / skills / agents / hooks を体系的にまとめたもの。

Affaan Mustafa の「[Everything Claude Code](https://github.com/affaan-m/everything-claude-code)」ガイドと [Anthropic 公式ベストプラクティス](https://www.anthropic.com/engineering/claude-code-best-practices)を基に、実運用で磨いた構成です。

## What's Inside

### Commands（スラッシュコマンド）

| コマンド | 用途 |
|---------|------|
| `/commit` | Git コミットワークフロー |
| `/pr` | Pull Request 作成 |
| `/ship` | Commit → Push → PR 一括実行 |
| `/build-fix` | ビルドエラー自動修正 |
| `/security` | セキュリティ監査 |
| `/learn` | CLAUDE.md 育成 |

### Skills（詳細ガイド）

**開発**

| スキル | 用途 |
|-------|------|
| `tdd` | テスト駆動開発 |
| `backend-patterns` | API/Repository パターン |
| `coding-rules` | コーディング規約 |
| `git-worktree` | Git worktree 操作 |
| `hooks` | Claude Code Hook 作成 |
| `mcp` | MCP サーバー作成 |
| `remotion` | Remotion 動画制作 |
| `core-web-vitals` | Core Web Vitals 計測・診断 |

**UI/UX・デザイン**

| スキル | 用途 |
|-------|------|
| `ui-ux-pro-max` | UI/UX デザイン全般 |
| `ux-psychology` | UX 心理学効果の適用 |
| `web-design-guidelines` | Web Interface Guidelines 準拠チェック |
| `app-onboarding` | アプリオンボーディング設計・改善 |

**コンテンツ制作**

| スキル | 用途 |
|-------|------|
| `ai-interview-article` | インタビュー形式 note 記事作成 |
| `note-serial-monetization` | note 連載の有料/無料設計 |

**マーケティング・CRO**

| スキル | 用途 |
|-------|------|
| `lp-optimizer` | LP/ページ分析・改善 |
| `copywriting` | マーケティングコピー作成 |
| `seo-audit` | SEO 監査・診断 |
| `marketing-audit` | マーケティング総合監査 |
| `marketing-psychology` | 心理学ベースのマーケティング |
| `launch-strategy` | ローンチ・GTM 戦略 |
| `pricing-strategy` | 価格設定・パッケージング |
| `ab-test-setup` | A/B テスト設計・実装 |
| `analytics-tracking` | アナリティクス実装 |
| `email-sequence` | メールシーケンス作成 |
| `referral-program` | リファラルプログラム設計 |
| `signup-flow-cro` | サインアップフロー最適化 |
| `onboarding-cro` | オンボーディング最適化 |
| `form-cro` | フォーム最適化 |
| `paywall-upgrade-cro` | ペイウォール・アップグレード最適化 |

**React / Next.js**

| スキル | 用途 |
|-------|------|
| `vercel-react-best-practices` | React/Next.js パフォーマンス最適化 |
| `vercel-composition-patterns` | React コンポジションパターン |
| `vercel-react-native-skills` | React Native / Expo ベストプラクティス |

**Stripe**

| スキル | 用途 |
|-------|------|
| `stripe-best-practices` | Stripe インテグレーション設計 |
| `stripe-projects` | Stripe Projects セットアップ |
| `upgrade-stripe` | Stripe API バージョンアップグレード |

**iOS**

| スキル | 用途 |
|-------|------|
| `ios-app-store-submission` | App Store 提出ワークフロー |

**freee**

| スキル | 用途 |
|-------|------|
| `freee-api-skill` | freee API 操作ガイド |

### Agents（サブエージェント）

| エージェント | 用途 |
|-------------|------|
| `code-reviewer` | PR/コードレビュー |
| `security-reviewer` | セキュリティ監査 |
| `codebase-optimizer` | コード最適化・重複検出 |
| `docs-curator` | ドキュメント整理 |
| `code-simplifier` | コード簡素化 |
| `verify-app` | アプリ動作検証 |

### Hooks（自動実行）

| フック | タイミング | 用途 |
|--------|-----------|------|
| `block-main-push.sh` | PreToolUse | main への直接 push をブロック |
| `validate-dangerous-ops.sh` | PreToolUse | 危険操作ブロック |
| `suggest-git-cleanup.sh` | Stop | Git 整理提案 |
| `check-remotion-quality.sh` | PostToolUse | Remotion 品質チェック |

### MCP Servers

| MCP | 用途 |
|-----|------|
| `nano-banana-pro` | Gemini 画像生成・編集 |
| `claude-peers` | 複数 Claude Code インスタンス間のリアルタイム連携 |
| `fal-video` | fal.ai 動画生成 |

## Pro Version

The complete operations manual for running a multi-agent Claude Code organization.

**Includes:**
- Tier System Operations Manual (T1 self-review / T2 peer-review / T3 conductor-review)
- Daily Report Templates + 3 real-world samples
- 10-Department Organization Chart Template + Design Decision Notes
- Cost Management Templates + freee Integration Flow

All documents available in English and Japanese.

**[$29 on Gumroad](https://glasswerks.gumroad.com/l/claude-code-template-pro)**

---

## Quick Start

### 方法 A: fork して使う（推奨）

1. このリポジトリを fork
2. `CLAUDE.md.template` → `CLAUDE.md` にリネーム
3. プロジェクト情報を記入
4. `settings.local.json.example` → `settings.local.json` にコピーしパス修正

```bash
# fork後
git clone https://github.com/YOUR_USERNAME/mued-claude-code-template.git
cd mued-claude-code-template
cp CLAUDE.md.template CLAUDE.md
cp .claude/settings.local.json.example .claude/settings.local.json
# CLAUDE.md と settings.local.json を自分のプロジェクトに合わせて編集
```

### 方法 B: シンボリックリンクで共有

複数プロジェクトで設定を共有し、一括更新できる方法。

```bash
# 1. テンプレートを配置
git clone https://github.com/kimny1143/mued-claude-code-template.git ~/claude-code-template

# 2. セットアップスクリプトを実行
cd /path/to/your/project
bash ~/claude-code-template/setup.sh
```

テンプレートを更新すると、全プロジェクトに自動反映（シンボリックリンクのため）。

#### シンボリックリンク構成のイメージ

```
mued-claude-code-template/     <- 共有設定の原本
├── .claude/
│   ├── commands/
│   │   ├── commit.md          <- 全プロジェクト共通
│   │   └── pr.md
│   └── skills/
│       ├── tdd/               <- 全プロジェクト共通
│       └── coding-rules/

your-project/.claude/
├── commands/
│   ├── commit.md -> ~/claude-code-template/.claude/commands/commit.md  (symlink)
│   └── my-workflow.md         <- プロジェクト固有
└── skills/
    ├── tdd -> ~/claude-code-template/.claude/skills/tdd  (symlink)
    └── database/              <- プロジェクト固有
```

### 方法 C: 必要なものだけコピー

```bash
git clone https://github.com/kimny1143/mued-claude-code-template.git
cd mued-claude-code-template

# 必要なものだけコピー
cp -r .claude/commands/ /path/to/your/project/.claude/commands/
cp -r .claude/skills/tdd /path/to/your/project/.claude/skills/
cp CLAUDE.md.template /path/to/your/project/CLAUDE.md
```

## 運用例: マルチエージェント体制

> この運用例は [glasswerks inc.](https://glasswerks.co.jp) での実績に基づいています。

### 課（部署）構成の設計

1エージェント = 1課（1つのワークスペース）で、リポジトリ境界ごとに分割:

```
経営部: conductor課（全体統括・進捗管理）
プロダクト部: mued課, native課
マーケティング部: SNS課, write課, video課
コーポレート部: LP課, freee課
データ部: data課
総務部: template課（このテンプレートの管理）
```

### Tier 制度（PR レビュー権限の段階的委譲）

AI エージェントに段階的に権限を委譲するための仕組み:

| Tier | 対象 | フロー |
|------|------|--------|
| T1 | docs・データのみ | セルフマージ（CI 通過必須） |
| T2 | コード変更 | ピアレビュー（同部署の別エージェント） |
| T3 | セキュリティ・DB・外部サービス | 人間レビュー |

### ブランチ保護

- `block-main-push.sh`: main への直接 push を自動ブロック
- `settings.local.json`: 権限の allow/deny を細かく制御
- 全変更は feature ブランチ → PR → マージの流れ

## 構造

```
.claude/
├── commands/           # スラッシュコマンド
│   ├── commit.md
│   ├── pr.md
│   ├── ship.md
│   ├── build-fix.md
│   ├── security.md
│   └── learn.md
├── skills/             # 詳細ガイド（37スキル）
│   ├── tdd/
│   ├── backend-patterns/
│   ├── coding-rules/
│   └── ...
├── agents/             # サブエージェント定義
│   ├── code-reviewer.md
│   ├── security-reviewer.md
│   ├── codebase-optimizer.md
│   ├── docs-curator.md
│   ├── code-simplifier.md
│   └── verify-app.md
├── hooks/              # 自動実行スクリプト
│   ├── block-main-push.sh
│   ├── validate-dangerous-ops.sh
│   ├── suggest-git-cleanup.sh
│   └── check-remotion-quality.sh
└── settings.local.json.example

mcps/                   # MCP サーバー
├── nano-banana-pro/
│   ├── launch.sh
│   └── README.md
├── fal-video/
│   └── launch.sh
└── claude-peers/
    └── README.md

project-configs/        # プロジェクト別設定例
docs/templates/         # ドキュメントテンプレート
CLAUDE.md.template      # プロジェクト説明テンプレート
setup.sh                # セットアップスクリプト
```

## カスタマイズ

### プロジェクト固有のスキル追加

```bash
mkdir -p .claude/skills/your-skill
cat > .claude/skills/your-skill/SKILL.md << 'EOF'
---
description: "Your skill description. Trigger: keyword1, keyword2"
---

# Your Skill

（スキルの内容）
EOF
```

### プロジェクト固有のコマンド追加

```bash
cat > .claude/commands/your-command.md << 'EOF'
Your command instructions here.
EOF
```

### Hooks のカスタマイズ

`validate-dangerous-ops.sh` に独自の検証ルールを追加するか、新しい hook スクリプトを作成して `settings.local.json` に登録。

## FAQ

**Q: ライセンスは？**
A: MIT License。商用利用・改変・再配布すべて自由。

**Q: 社内テンプレートとして使ってよいか？**
A: はい。fork して自社向けにカスタマイズしてください。

**Q: Claude Code 以外の AI コーディングツールでも使える？**
A: スキルの内容（SKILL.md）は汎用的な知識ですが、commands / hooks / settings.json は Claude Code 固有の仕組みです。

**Q: Claude Code Max（$200/月）でないと使えないか？**
A: テンプレート自体はどのプランでも使えます。ただし、マルチエージェント体制（claude-peers）は複数インスタンスの同時実行が前提なので、Max プランが実質的に必要です。

**Q: 特定のスキルが動かない**
A: スキルは Claude Code のバージョンに依存する場合があります。Issue でご報告ください。

## 参考資料

- [Affaan Mustafa: Everything Claude Code](https://github.com/affaan-m/everything-claude-code)
- [Anthropic: Claude Code Best Practices](https://www.anthropic.com/engineering/claude-code-best-practices)
- [Boris Cherny's Workflow](https://venturebeat.com/technology/the-creator-of-claude-code-just-revealed-his-workflow-and-developers-are)

## Contributing

[CONTRIBUTING.md](CONTRIBUTING.md) を参照してください。

## License

MIT

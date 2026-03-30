# Contributing

コントリビューションを歓迎します。

## PR を出す前に

1. Issue を先に立てて、変更内容を説明してください
2. 修正 PR で Issue を参照してください

## 新しいスキルの追加

以下の基準を満たすスキルを歓迎します:

1. **汎用的**: 特定プロジェクトに依存しない
2. **再現可能**: 読者が自分の環境で使える
3. **フォーマット準拠**: SKILL.md のフォーマット（frontmatter + description + トリガー例）に従う

### SKILL.md のフォーマット

```markdown
---
description: "スキルの説明。トリガー: keyword1, keyword2, keyword3"
---

# スキル名

（スキルの内容）
```

- `description` の先頭にスキルの概要を書く
- トリガー例を含める（Claude Code がいつこのスキルを使うか判断するため）

## 既存スキルの改善

- 変更理由を PR の description に明記してください
- 破壊的変更がある場合は Issue で事前に議論してください

## コマンド・Hooks の追加

- コマンド: `.claude/commands/your-command.md` に配置
- Hooks: `.claude/hooks/your-hook.sh` に配置し、README で `settings.local.json` への登録方法を説明

## コードスタイル

- Shell スクリプト: bash, `set -euo pipefail`
- Markdown: 日本語 OK（このリポジトリは日本語ベース）

## サポート範囲

- このリポジトリは [glasswerks inc.](https://glasswerks.co.jp) の実運用テンプレートがベースです
- Issue 対応・PR 対応は best-effort です（保証なし）
- Claude Code 本体のバグは [Anthropic](https://github.com/anthropics/claude-code/issues) に報告してください

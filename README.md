# Claude Code Plugins

Claude Code用の実用的なプラグイン集です。

## 📦 含まれるプラグイン

### Product Requirements Analyst

製品アイデアを包括的な要件ドキュメントに変換し、技術的実現可能性を検証するエージェントプラグインです。

**主な機能:**
- 要件定義の構造化
- 技術的実現可能性分析
- リスク評価とギャップ特定
- アーキテクチャ設計提案

詳細は [plugins/product-requirements-analyst/README.md](plugins/product-requirements-analyst/README.md) を参照してください。

## 🚀 使用方法

### マーケットプレイスの追加

```bash
/plugin marketplace add ariela/claude-plugins
```

### プラグインのインストール

```bash
# Product Requirements Analystをインストール
/plugin install product-requirements-analyst@ariela-plugins

# プロジェクトスコープでインストール（チーム共有）
/plugin install product-requirements-analyst@ariela-plugins --scope project
```

### インストール済みプラグインの確認

```bash
/plugin list
```

## 📂 プロジェクト構成

```
claude-plugins/
├── .claude-plugin/
│   └── marketplace.json          # マーケットプレイス設定
├── .claude/
│   ├── commands/                 # カスタムコマンドのサンプル
│   ├── hooks/                    # セッションフックのサンプル
│   └── rules/                    # プラグイン開発ルール
├── plugins/
│   └── product-requirements-analyst/
│       ├── .claude-plugin/
│       │   └── plugin.json
│       ├── agents/
│       │   └── product-requirements-analyst.md
│       └── README.md
├── README.md                     # このファイル
└── LICENSE
```

## 🔧 プラグイン開発

### 新しいプラグインの追加

1. `plugins/` ディレクトリに新しいプラグイン用のディレクトリを作成
2. プラグインの構造を作成:
   ```
   plugins/your-plugin/
   ├── .claude-plugin/
   │   └── plugin.json
   ├── commands/          # オプション
   ├── agents/            # オプション
   ├── skills/            # オプション
   └── README.md
   ```
3. `.claude-plugin/marketplace.json` にプラグインを追加

### プラグインの検証

```bash
/plugin validate .
```

## 📄 ライセンス

MIT

## 👤 作者

Ariela

## 🔗 リンク

- [Claude Code公式ドキュメント](https://code.claude.com/docs)
- [プラグイン開発ガイド](https://code.claude.com/docs/en/plugins.md)
- [プラグインマーケットプレイス](https://code.claude.com/docs/en/plugin-marketplaces.md)

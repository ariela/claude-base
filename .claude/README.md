# Claude Code Plugin Marketplace

このリポジトリは、Claude Code用のプラグインマーケットプレイスです。

## プラグインマーケットプレイスの使用

### マーケットプレイスの追加

```bash
/plugin marketplace add ariela/claude-plugins
```

### プラグインのインストール

```bash
/plugin install product-requirements-analyst@ariela-plugins
```

## 含まれるプラグイン

- **product-requirements-analyst** - 製品要件分析と技術的実現可能性の検証を行うエージェントプラグイン

## ディレクトリ構成

```
.claude/
├── commands/           # スラッシュコマンドのサンプル
├── hooks/             # セッションフックのサンプル
└── rules/             # プラグイン開発ルール
    ├── README.md      # ルールシステムの概要
    └── output-language.md  # 出力言語ルール
```

## プラグイン開発

新しいプラグインを追加する場合は、`plugins/` ディレクトリに配置してください。

詳細については、Claude Codeの公式ドキュメントを参照してください:
https://code.claude.com/docs/en/plugins.md

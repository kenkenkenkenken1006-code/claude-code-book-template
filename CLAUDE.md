# Claude Code プロジェクト設定

## プロジェクト概要
このリポジトリは Claude Code の開発環境テンプレートです。

## セットアップ手順

### 1. 前提条件
- Docker Desktop がインストールされていること
- VS Code + Dev Containers 拡張機能がインストールされていること
- Anthropic API キーがあること

### 2. 環境変数の設定
ターミナルで以下を実行（または `.bashrc` / `.zshrc` に追加）:
```bash
export ANTHROPIC_API_KEY="your-api-key-here"
```

### 3. Dev Container の起動
1. VS Code でこのフォルダを開く
2. コマンドパレット（Cmd+Shift+P）→「Dev Containers: Reopen in Container」
3. コンテナのビルドが完了したらターミナルで `claude` を実行

## Claude Code の基本コマンド
```bash
# Claude Code を起動
claude

# ファイルを指定して起動
claude --file path/to/file

# バージョン確認
claude --version
```

## ディレクトリ構成
```
.
├── .devcontainer/
│   ├── devcontainer.json   # Dev Container 設定
│   └── Dockerfile          # コンテナイメージ定義
├── CLAUDE.md               # このファイル
└── README.md
```

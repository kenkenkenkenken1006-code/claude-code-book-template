FROM mcr.microsoft.com/devcontainers/base:ubuntu-24.04

# 必要なパッケージをインストール
RUN apt-get update && apt-get install -y \
    curl \
    git \
    wget \
    unzip \
    && rm -rf /var/lib/apt/lists/*

# Node.js 22 をインストール
RUN curl -fsSL https://deb.nodesource.com/setup_22.x | bash - \
    && apt-get install -y nodejs \
    && rm -rf /var/lib/apt/lists/*

# Claude Code をグローバルインストール
RUN npm install -g @anthropic-ai/claude-code

# 作業ディレクトリ
WORKDIR /workspace

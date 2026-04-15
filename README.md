# Claude AWS Bedrock Chat (MCP CLI)

A command-line chat application that integrates **Anthropic Claude
models via Amazon Bedrock** to provide an interactive, extensible AI
assistant experience. This project demonstrates how to build a modular
CLI chat tool with support for document retrieval, command-based
prompts, and tool integrations using the **Model Control Protocol
(MCP)** architecture.

------------------------------------------------------------------------

## 🚀 Overview

This project is a developer-friendly CLI tool that enables seamless
interaction with Claude models hosted on Amazon Bedrock. It is designed
to be:

-   **Extensible** -- Easily plug in new tools and capabilities via MCP\
-   **Interactive** -- Real-time conversational interface in the
    terminal\
-   **Context-aware** -- Supports document ingestion and retrieval\
-   **Cloud-native** -- Uses AWS Bedrock for scalable LLM access

------------------------------------------------------------------------

## ✨ Features

-   💬 Interactive CLI chat interface\
-   🧠 Claude model integration via AWS Bedrock\
-   📄 Document retrieval for context-aware responses\
-   🧩 MCP-based tool/plugin architecture\
-   ⚙️ Command-driven prompt system\
-   🔌 Extensible tool integrations\
-   🔐 AWS credential-based authentication

------------------------------------------------------------------------

## 🏗️ Architecture

    User (CLI)
       ↓
    Command Parser / MCP Layer
       ↓
    Tooling + Context Retrieval
       ↓
    Claude (via AWS Bedrock API)
       ↓
    Response Streaming to CLI

------------------------------------------------------------------------

## ⚙️ Prerequisites

-   Python 3.8+\
-   AWS account with Bedrock access\
-   Claude model access enabled in Bedrock\
-   Configured AWS credentials

------------------------------------------------------------------------

## 🛠️ Setup

### 1. Clone the repository

``` bash
git clone https://github.com/jnj-97/claude-aws-bedrock.git
cd claude-aws-bedrock
```

### 2. Install dependencies

``` bash
pip install -r requirements.txt
```

### 3. Configure environment

Create a `.env` file:

    AWS_ACCESS_KEY_ID=your_access_key
    AWS_SECRET_ACCESS_KEY=your_secret_key
    AWS_REGION=us-east-1

Or run:

``` bash
aws configure
```

------------------------------------------------------------------------

## ▶️ Usage

``` bash
python main.py
```

------------------------------------------------------------------------

## 🧩 MCP (Model Control Protocol)

This project uses MCP to enable structured interaction between:

-   User commands\
-   Tools/plugins\
-   LLM responses

------------------------------------------------------------------------

## 🔌 Extending the System

Add custom tools by creating modules and registering them in the MCP
layer.

------------------------------------------------------------------------

## 📄 Document Retrieval

Supports ingesting documents and using them as context for Claude
responses.

------------------------------------------------------------------------

## 🔐 Authentication

Uses standard AWS credential methods (env vars, CLI, SSO).

------------------------------------------------------------------------

## 📚 Tech Stack

-   Python\
-   AWS Bedrock\
-   Anthropic Claude\
-   MCP architecture

------------------------------------------------------------------------

## 📜 License

MIT License

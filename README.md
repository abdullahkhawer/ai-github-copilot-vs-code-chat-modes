# ✨ AI GitHub Copilot VS Code Chat Modes

- Founder: [Abdullah Khawer - LinkedIn](https://www.linkedin.com/in/abdullah-khawer)

# Introduction

A curated collection of custom chat modes based on `chatmode.md` files for Visual Studio Code (VS Code) used by GitHub Copilot to enhance your development using AI to work smarter.

Custom chat modes allow you to modify GitHub Copilot's behavior in VS Code. Each `chatMode.md` file builds a specialized AI assistant with targeted knowledge and abilities for your development work, significantly cutting development time by eliminating repetitive manual tasks.

# Official Documentation

- [GitHub Copilot Chat](https://code.visualstudio.com/docs/copilot/chat/copilot-chat)
- [Custom Chat Modes](https://code.visualstudio.com/docs/copilot/chat/chat-modes#_custom-chat-modes)

# Getting Started

To use any of these custom chat modes:

1. Copy the desired `.chatmode.md` file from the `/chat-modes` directory in this repository to your workspace's `.github/chatmodes` directory (create it if it doesn't exist).
2. Restart VS Code to load the new chat mode.
3. Open the GitHub Copilot Chat panel in VS Code.
4. Click the dropdown menu at the bottom of the chat panel and select your custom chat mode from the list.

The chat mode will now be active, and Copilot Chat will respond according to the instructions defined in the chosen `.chatmode.md` file.

# 🚀 Available Chat Modes

| Title | Description | Category |
| ----- | ----------- | -------- |
| [Terraform Helm Release Upgrade Analyser](chat-modes/terraform-helm-release-upgrade-analyser.chatmode.md) | Creates a detailed upgrade plan for a Helm release created via Terraform by analysing the configuration differences between the current and desired Helm chart versions and any breaking changes | Infrastructure & DevOps |
| [Dockerfile Developer](chat-modes/dockerfile-developer.chatmode.md) | Develops optimized, secure, and best-practice Dockerfiles based on user requirements and application context | Infrastructure & DevOps |
| [Conversation to Chat Mode](chat-modes/conversation-to-chat-mode.chatmode.md) | Creates a custom chat mode file based on a conversational interface where users describe their specific task requirements and guidelines | Development Tools |

## Terraform Helm Release Upgrade Analyser

This chat mode helps you safely upgrade Helm releases managed by Terraform by:

- **Automatic Detection**: Scans your Terraform code to identify Helm release resources
- **Version Comparison**: Compares template files and default values between chart versions
- **Breaking Change Analysis**: Identifies potential breaking changes and compatibility issues
- **Detailed Planning**: Creates comprehensive upgrade plans with step-by-step instructions

### Demo

![Demo](demos/terraform-helm-release-upgrade-analyser.chatmode.gif)

### Example Usage

To use this chat mode effectively, follow these steps:

### Prerequisites

1. Ensure you have Terraform code that contains a Helm release resource
2. Know the current and desired Helm chart versions for your upgrade

### Setup

1. Start a new chat session
2. Select `terraform-helm-release-upgrade-analyser.chatmode.md` as the chat mode
3. Select `Claude Sonnet 4` as the model
4. Choose the directory containing your Terraform code for the Helm release as the context

### Prompt Example

```
Analyze my Helm chart upgrade plan.
Current Helm chart version: 4.12.3
Desired Helm chart version: 4.13.1
```

## Dockerfile Developer

This chat mode helps you create optimized, secure, and production-ready Dockerfiles by:

- **Context Analysis**: Analyzes your project files to understand dependencies and build requirements
- **Best Practices**: Follows Docker best practices including proper layer ordering, caching optimization, and clean syntax
- **Size Optimization**: Creates minimal container images through multi-stage builds and efficient package management
- **Security Focus**: Implements security best practices including non-root users and vulnerability scanning
- **Technology Detection**: Automatically detects your application stack from project files (package.json, requirements.txt, etc.)

### Demo

![Demo](demos/dockerfile-developer.chatmode.gif)

### Example Usage

To use this chat mode effectively, follow these steps:

### Prerequisites
- Have your application project ready in a specific directory
- Know your application type and technology stack  
- Have access to dependency files if they exist

### Setup
1. Start a new chat session
2. Select `dockerfile-developer.chatmode.md` as the chat mode
3. Select `Claude Sonnet 4` as the model
4. Have your application details and project context ready

### Prompt Example

```
I need to create a Dockerfile for my Node.js application. Please help me develop an optimized Dockerfile.
```

## Conversation to Chat Mode

This meta chat mode helps you create new custom chat modes through a guided conversation by:

- **Interactive Creation**: Walks you through a conversational interface to define your chat mode requirements
- **Template Generation**: Automatically generates properly formatted `.chatmode.md` files based on your inputs
- **Guided Questions**: Asks targeted questions about your specific task and required guidelines
- **Best Practices**: Ensures your custom chat mode follows established conventions and formatting

### Demo

![Demo](demos/conversation-to-chat-mode.chatmode.gif)

### Example Usage

To use this chat mode effectively, follow these steps:

### Prerequisites

1. Have a clear idea of what specific task or problem you want your custom chat mode to solve
2. Think about the specific instructions and guidelines needed for that task

### Setup

1. Start a new chat session
2. Select `conversation-to-chat-mode.chatmode.md` as the chat mode
3. Select `Claude Sonnet 4` as the model

### Prompt Example

```
Let's have a conversation to build a custom chat mode file.
```

# 🤝 Contributing

Contributions are welcome! If you have a custom chat mode you'd like to share:

1. Fork this repository
2. Create a new `.chatmode.md` file in the `chat-modes` directory
3. Update this README.md to include your chat mode in the table
4. Submit a pull request

# Chat Mode Guidelines

- Use descriptive names and clear descriptions
- Include comprehensive documentation and usage examples
- Test your chat mode thoroughly before submitting
- Follow the established file naming convention: `your-mode-name.chatmode.md`

# 📝 License

This project is licensed under the Apache License - see the [LICENSE](LICENSE) file for details.

---

###### 😊 Any contributions, improvements and suggestions will be highly appreciated.

###### 🌟 Star this repository to know about awesome new chat modes for VS Code.

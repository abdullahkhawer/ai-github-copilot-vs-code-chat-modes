# ✨ AI GitHub Copilot VS Code Chat Modes

- Founder: [Abdullah Khawer - LinkedIn](https://www.linkedin.com/in/abdullah-khawer)

# Introduction

A curated collection of custom chat modes based on `chatmode.md` files for Visual Studio Code (VS Code) used by GitHub Copilot to enhance your development using AI to work smarter.

Custom chat modes allow you to modify GitHub Copilot's behavior in VS Code. Each `chatMode.md` file builds a specialized AI assistant with targeted knowledge and abilities for your development work, significantly cutting development time by eliminating repetitive manual tasks.

## Official Documentation

- [GitHub Copilot Chat](https://code.visualstudio.com/docs/copilot/chat/copilot-chat)
- [Custom Chat Modes](https://code.visualstudio.com/docs/copilot/chat/chat-modes#_custom-chat-modes)

## Getting Started

To use any of these custom chat modes:

1. Copy the desired `.chatmode.md` file from the `/chat-modes` directory in this repository to your workspace's `.github/chatmodes` directory (create it if it doesn't exist).
2. Restart VS Code to load the new chat mode.
3. Open the GitHub Copilot Chat panel in VS Code.
4. Click the dropdown menu at the bottom of the chat panel and select your custom chat mode from the list.

The chat mode will now be active, and Copilot Chat will respond according to the instructions defined in the chosen `.chatmode.md` file.

## 🧩 Available Chat Modes

| Title | Description | Category |
| ----- | ----------- | -------- |
| [Terraform Helm Release Upgrade Analyser](chat-modes/terraform-helm-release-upgrade-analyser.chatmode.md) | Creates a detailed upgrade plan for a Helm release created via Terraform by analysing the configuration differences between the current and desired Helm chart versions and any breaking changes | Infrastructure & DevOps |

### 🚀 Featured Chat Mode: Terraform Helm Release Upgrade Analyser

This chat mode helps you safely upgrade Helm releases managed by Terraform by:

- **Automatic Detection**: Scans your Terraform code to identify Helm release resources
- **Version Comparison**: Compares template files and default values between chart versions
- **Breaking Change Analysis**: Identifies potential breaking changes and compatibility issues
- **Detailed Planning**: Creates comprehensive upgrade plans with step-by-step instructions

#### Demo

![Demo](demos/terraform-helm-release-upgrade-analyser.chatmode.gif)

#### Example Usage

To use this chat mode effectively, follow these steps:

##### Prerequisites
1. Ensure you have Terraform code that contains a Helm release resource
2. Know the current and desired Helm chart versions for your upgrade

##### Setup
1. Start a new chat session
2. Select `terraform-helm-release-upgrade-analyser.chatmode.md` as the chat mode
3. Select `Claude Sonnet 4` as the model
4. Choose the directory containing your Terraform code for the Helm release as the context

##### Prompt Example

```
Analyze my Helm chart upgrade plan.
Current Helm chart version: 4.12.3
Desired Helm chart version: 4.13.1
```

## 🤝 Contributing

Contributions are welcome! If you have a custom chat mode you'd like to share:

1. Fork this repository
2. Create a new `.chatmode.md` file in the `chat-modes` directory
3. Update this README.md to include your chat mode in the table
4. Submit a pull request

### Chat Mode Guidelines

- Use descriptive names and clear descriptions
- Include comprehensive documentation and usage examples
- Test your chat mode thoroughly before submitting
- Follow the established file naming convention: `your-mode-name.chatmode.md`

## 📝 License

This project is licensed under the Apache License - see the [LICENSE](LICENSE) file for details.

---

###### 😊 Any contributions, improvements and suggestions will be highly appreciated.
###### 🌟 Star the repo now and be the first to know about new and exciting chat modes for VS Code.

# FiboCode — A Living Codebase Knowledge Base for Agent Workflows

> **Understand Every Codebase.**
>
> From code to understanding—for humans and AI agents.

[Official Website](https://fibocode.ai/) · [Download FiboCode](https://fibocode.ai/download) · [Quick Start Documentation](https://fibocode.ai/docs) · [Latest GitHub Release](https://github.com/Alenkz12/FiboCode-Releases/releases/latest)

FiboCode is a local-first code editor with a living codebase knowledge base for agent workflows. It connects source code, Markdown documentation, relationship graphs, specifications, designs, plans, change records, and project history in one traceable workspace.

Keep the Agent CLI you already trust. FiboCode gives it persistent, repository-native context—and gives you an IDE-grade surface for reviewing the code it changes. It works alongside Claude Code, Codex, Gemini CLI, OpenCode, and other terminal-based coding agents instead of asking you to replace your existing workflow.

FiboCode is built for developers and teams who need to understand unfamiliar or long-lived codebases, preserve project knowledge across agent sessions, turn requirements into traceable changes, and keep the final review under human control.

> **About this repository:** this is the official FiboCode distribution repository. It hosts release binaries and update metadata; the product source code is not published here.

## What You Can Do with FiboCode

| Capability | What it helps you do |
| --- | --- |
| [Codebase Understanding](https://fibocode.ai/features/codebase-understanding) | Explore code, connected Markdown docs, relationship graphs, and project history to understand an unfamiliar or complex codebase faster. |
| [Context Engineering for Coding Agents](https://fibocode.ai/features/context-engineering) | Keep specs, designs, plans, change records, code, docs, and graphs with the repository so coding agents receive durable project context instead of a one-off prompt. |
| [Spec-Driven Development](https://fibocode.ai/features/spec-driven-development) | Turn requirements into specifications, designs, implementation plans, agent execution, code review, and traceable change records. |
| [AI Code Review](https://fibocode.ai/features/ai-code-review) | Inspect agent-generated changes through automatic diff summaries, focused hunks, single-column diff review, message snapshots, history, and rollback while keeping the final judgment human. |

## One Connected Agent Workflow

```mermaid
flowchart LR
  source_code_001["Editable source code"] -->|grounds| knowledge_base_002["Docs, graphs, specs, and history"]
  knowledge_base_002 -->|provides persistent context| human_agent_003["Developers and coding agents"]
  human_agent_003 -->|plan and implement| traceable_changes_004["Traceable changes"]
  traceable_changes_004 -->|are inspected through| human_review_005["Human review and control"]
  human_review_005 -->|accepted changes update| source_code_001
  human_review_005 -->|records decisions in| knowledge_base_002
```

Source code remains the ground truth. Documentation explains it, graphs reveal relationships, and specifications and change records preserve why the software evolved. After a reviewed change returns to the codebase, its decisions and evidence strengthen the shared context available for the next human or agent task.

## Download and Install

For the easiest platform-specific download, visit the official [FiboCode download page](https://fibocode.ai/download). You can also download installers directly from [GitHub Releases](https://github.com/Alenkz12/FiboCode-Releases/releases/latest).

| Platform | Installer | Support |
| --- | --- | --- |
| macOS | `FiboCode-<version>-arm64-mac.dmg` | Apple Silicon |
| Windows | `FiboCode-Setup-<version>.exe` | Windows installer |
| Linux | `FiboCode-<version>-x86_64.AppImage` | x86_64 AppImage |

### macOS

1. Open the `.dmg` file.
2. Drag FiboCode into the Applications folder.
3. If macOS blocks the first launch, open **System Settings → Privacy & Security** and choose **Open Anyway**.

### Windows

Run the `.exe` installer and follow the setup wizard.

### Linux

```bash
chmod +x FiboCode-<version>-x86_64.AppImage
./FiboCode-<version>-x86_64.AppImage
```

## Local-First Privacy and Data Boundaries

FiboCode is local-first, but using it with a remote AI service is not the same as using a fully offline application. FiboCode does not upload or store your source code or workspace data on FiboCode-controlled servers. When you invoke a remote AI model, relevant content is transmitted directly to the provider you configured so it can fulfill the request.

| Data | Default location | When it may leave your device |
| --- | --- | --- |
| Source code and project files | Your workspace | A code-analysis or chat request sent to a remote model may include the selected file's full contents, path, and related context. |
| Generated analysis, summaries, and graphs | Your project's `.fibo/analysis` directory | They may be sent when a remote-model request uses them as context or asks the model to summarize them. |
| Model Provider API credentials | Your local FiboCode configuration | The credential is sent to the corresponding Provider for authentication; FiboCode does not receive it through a FiboCode-controlled service. |
| Information submitted through a fibocode.ai form | The website service | It leaves your device only when you choose to submit the form. |

```mermaid
flowchart LR
  local_workspace_001["Local workspace"] -->|processed on the device| local_analysis_002["Local analysis artifacts"]
  local_workspace_001 -->|selected content in a remote request| chosen_provider_003["User-configured AI Provider"]
  local_analysis_002 -->|used as remote context| chosen_provider_003
  chosen_provider_003 -->|governed by| provider_terms_004["Provider privacy policy and terms"]
```

The Provider—not the FiboCode maintainer—controls its own data retention, training, and deletion practices. Before using a private or sensitive repository, review the files that can be analyzed, remove secrets such as API keys, passwords, and tokens, and check the Provider's current policy. You can also configure an OpenAI-compatible endpoint that you operate or otherwise trust.

See the [FiboCode Privacy Policy](https://fibocode.ai/privacy) for the complete disclosure.

## Security and Maintainer

FiboCode is independently maintained by the FiboCode maintainer; this repository does not represent a separate security team or a registered company. Please report suspected code, credential, or local-data exposure privately by following the [FiboCode Security Policy](https://github.com/Alenkz12/FiboCode-Releases/security/policy). Use public Issues for ordinary bugs and feature requests, but do not post real secrets, private source code, or personal data there.


## Learn More

- Read the [FiboCode Quick Start](https://fibocode.ai/docs) for installation, model configuration, terminal workflows, code analysis, and Fibo Skills.
- Explore practical guides on the [FiboCode Blog](https://fibocode.ai/blog).
- Follow upcoming work and submit ideas on the [FiboCode Roadmap](https://fibocode.ai/roadmap).
- Review plans for personal and organizational use on the [FiboCode Pricing and Licensing](https://fibocode.ai/pricing) page.
- Visit the [official FiboCode website](https://fibocode.ai/) for product demos, feature details, and current downloads.

## License and Commercial Use

FiboCode is free for personal use, including learning, personal projects, and open-source work. Use for the work of a for-profit organization requires a commercial license. Read the current [pricing and licensing overview](https://fibocode.ai/pricing) and [FiboCode EULA](https://fibocode.ai/eula) before use.

## Feedback and Support

Found a bug or have a feature request?

- [Report a bug](https://github.com/Alenkz12/FiboCode-Releases/issues)
- [Join the community discussion](https://github.com/Alenkz12/FiboCode-Releases/discussions)
- [Share a roadmap idea](https://fibocode.ai/roadmap)

---
name: FiboCode Release Repository README

update-time: 2026-08-11 08:06

description: FiboCode downloads, data boundaries, and security reporting.

---

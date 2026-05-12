🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# Soc Ops

> A fast, fun social bingo game for in-person mixers — built with Blazor and designed for learning AI-assisted development.

🎮 **[Play the Game](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/)**  
📚 **[Start the Lab Guide](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/)**

## Why this project?

Soc Ops helps groups break the ice in minutes:
- 🧩 Fill your board by finding people who match each prompt
- ⚡ Get immediate bingo detection (rows, columns, diagonals)
- 💾 Resume where you left off with local storage persistence
- 🧪 Explore a real workshop repo focused on prompt engineering + agent workflows

---

## 🚀 Quick Start

### Prerequisites
- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) or higher

### Run locally
```bash
dotnet run --project SocOps/SocOps.csproj
```

### Build
```bash
dotnet build SocOps/SocOps.csproj
```

> Deploys automatically to GitHub Pages on push to `main`.

---

## 🧭 Workshop path

| Part | Title |
|------|-------|
| [**00**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Overview & Checklist |
| [**01**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Setup & Context Engineering |
| [**02**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Design-First Frontend |
| [**03**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Custom Quiz Master |
| [**04**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Multi-Agent Development |

> 📝 Lab guides are also available in the [`workshop/`](workshop/) folder for offline reading.

---

## 🏗️ Project structure

- `SocOps/Pages/Home.razor` — top-level page flow (start/game states)  
- `SocOps/Components/` — reusable UI components  
- `SocOps/Services/BingoGameService.cs` — game state orchestration + persistence  
- `SocOps/Services/BingoLogicService.cs` — pure bingo rules and board logic

---

## ☁️ Open in GitHub Codespaces (optional)

After creating your own repo from this template:

1. Open your repo on GitHub
2. Click **Code** → **Codespaces** → **Create codespace on main**
3. Wait for the devcontainer to finish setup
4. From the repository root, run:
   ```bash
   dotnet run --project SocOps/SocOps.csproj
   ```

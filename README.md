🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# Soc Ops

Turn awkward room energy into instant connection.

Soc Ops is a fast, in-person social bingo game built with Blazor. Players walk around, find people who match each square, and race to complete 5 in a row.

🎮 **[Play the Game](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/)**

📚 **[Open the Interactive Lab Guide](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/)**

---

## Why This Project

- Great for mixers, workshops, hackathons, onboarding events, and classrooms
- Designed as a practical AI-assisted development lab with GitHub Copilot
- Small codebase, clean architecture, and easy to customize prompts/questions

---

## Quick Start

### Prerequisite

- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0)

### Run Locally

```bash
dotnet run --project SocOps/SocOps.csproj
```

### Build

```bash
dotnet build SocOps/SocOps.csproj
```

### Format Check

```bash
dotnet format --verify-no-changes
```

### Tests (when present)

```bash
dotnet test
```

---

## Workshop Path

Follow the lab in sequence:

| Part | Title |
|------|-------|
| [**00**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Overview and Checklist |
| [**01**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Setup and Context Engineering |
| [**02**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Design-First Frontend |
| [**03**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Custom Quiz Master |
| [**04**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Multi-Agent Development |

Offline docs are available in [workshop/](workshop/).

---

## Open in Codespaces (Optional)

After creating your own repo from this template:

1. Open your repo on GitHub.
2. Select **Code** > **Codespaces** > **Create codespace on main**.
3. Wait for the dev container setup to complete.
4. Run:

```bash
dotnet run --project SocOps/SocOps.csproj
```

---

## Project Structure

- UI entry point: [SocOps/Pages/Home.razor](SocOps/Pages/Home.razor)
- Components: [SocOps/Components/](SocOps/Components)
- Game orchestration and persistence: [SocOps/Services/BingoGameService.cs](SocOps/Services/BingoGameService.cs)
- Core game logic: [SocOps/Services/BingoLogicService.cs](SocOps/Services/BingoLogicService.cs)
- Question data: [SocOps/Data/Questions.cs](SocOps/Data/Questions.cs)

---

## Contributing

Contributions are welcome. Start with [CONTRIBUTING.md](CONTRIBUTING.md).

On push to main, this project deploys automatically to GitHub Pages.

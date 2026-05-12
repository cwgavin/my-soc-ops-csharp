# Project Guidelines

## Mandatory Development Checklist
Before committing, run all three:
- Lint: `dotnet format --verify-no-changes`
- Build: `dotnet build SocOps/SocOps.csproj`
- Test: `dotnet test` (run when tests are present)

## Build and Run
- SDK: .NET 10 (`net10.0` in [SocOps/SocOps.csproj](SocOps/SocOps.csproj)).
- Run app: `dotnet run --project SocOps/SocOps.csproj`.

## Architecture
- Main page: [SocOps/Pages/Home.razor](SocOps/Pages/Home.razor) switches start/game UI.
- UI components live in [SocOps/Components/](SocOps/Components).
- State and persistence live in [SocOps/Services/BingoGameService.cs](SocOps/Services/BingoGameService.cs).
- Pure board/bingo logic lives in [SocOps/Services/BingoLogicService.cs](SocOps/Services/BingoLogicService.cs).

## Conventions
- Keep rules/algorithms in `BingoLogicService`; keep orchestration in `BingoGameService`.
- Preserve localStorage compatibility (`STORAGE_KEY`, `STORAGE_VERSION`) when changing saved state.
- Follow `OnStateChanged` subscribe/unsubscribe pattern from [SocOps/Pages/Home.razor](SocOps/Pages/Home.razor).
- Reuse/extend utility CSS in [SocOps/wwwroot/css/app.css](SocOps/wwwroot/css/app.css).

## Docs
- [README.md](README.md), [CONTRIBUTING.md](CONTRIBUTING.md)
- [workshop/GUIDE.md](workshop/GUIDE.md), [workshop/01-setup.md](workshop/01-setup.md)
- [.github/instructions/css-utilities.instructions.md](.github/instructions/css-utilities.instructions.md)
- [.github/instructions/frontend-design.instructions.md](.github/instructions/frontend-design.instructions.md)

## Pitfalls
- Do not treat [.solutions/](.solutions/) as active app code.
- Do not edit generated output in [SocOps/bin/](SocOps/bin) or [SocOps/obj/](SocOps/obj).

# EZCode

A Windows desktop dashboard for running [Claude Code](https://claude.com/ko/product/claude-code) across multiple
project folders: terminal tabs, git status/diff, token statistics, and your plan's session/weekly usage.

> **Unofficial project.** EZCode is an independent, community-made tool. It is not made, endorsed,
> sponsored, or supported by Anthropic. "Claude" and "Claude Code" are trademarks of Anthropic, PBC and are
> used here only to describe compatibility. See `THIRD_PARTY_NOTICES.md`.
>
> **비공식 프로젝트입니다.** EZCode는 개인이 만든 독립 도구이며 Anthropic과 아무 관련이 없고,
> Anthropic의 승인·후원·지원을 받지 않았습니다.

## Download

Get **`EZCode_Setup.exe`** from the [latest release](../../releases/latest) and run it.

- Windows 10/11 (64-bit)
- The installer can also install the **Claude Code CLI** for you (needs an internet connection). A Claude
  subscription login (Pro/Max) is needed to see session/weekly usage percentages.

## Windows SmartScreen warning

The installer is **not code-signed**, so Windows SmartScreen may show "Windows protected your PC" /
"Unknown publisher" (and some antivirus tools may flag it). This is expected for unsigned apps.
To continue: click **More info** → **Run anyway**.

설치 파일에 코드 서명이 없어 SmartScreen이 "알 수 없는 게시자" 경고를 띄울 수 있습니다(일부 백신이 오탐할 수도 있습니다).
**추가 정보 → 실행**을 누르면 설치할 수 있습니다.

## Permission modes (read before using Auto)

New tabs start in **Manual** mode: Claude Code asks for your approval before editing files or running commands.

**Auto** mode launches Claude Code with `--dangerously-skip-permissions`. In Auto mode Claude can edit,
delete, and run commands in the project folder **without asking you**. Use it only on projects you have
backed up or under version control. You are responsible for what runs in your sessions.

**자동** 모드는 `--dangerously-skip-permissions`로 실행되어 Claude가 파일 수정·삭제와 명령 실행을
**묻지 않고** 할 수 있습니다. 백업했거나 git으로 관리되는 프로젝트에서만 사용하세요.

## Privacy

Everything stays on your PC under `%APPDATA%\EZCode\`. EZCode does not read your login token, does not call
any Anthropic API itself, and sends nothing to its author. Usage percentages come from the status-line data
Claude Code itself reports. The local server listens on `127.0.0.1` only.

## Feedback

Please open an [issue](../../issues) for bugs or suggestions.

## License

MIT. See `LICENSE`. Third-party components: see `THIRD_PARTY_NOTICES.md`.

# Third-Party Notices

EZCode is an independent, unofficial tool. It is **not made, endorsed, or supported by Anthropic**.
"Claude" and "Claude Code" are trademarks of Anthropic, PBC. EZCode only launches the Claude Code CLI
that the user has installed themselves and displays information that CLI provides.

EZCode bundles or loads the following open-source components.
License names below are from each project's published license; **verify against the exact versions you ship
before release** (and include the full license texts where the license requires it).

## Backend (Python)

| Component | License |
|---|---|
| FastAPI | MIT |
| Uvicorn | BSD-3-Clause |
| websockets | BSD-3-Clause |
| Pydantic | MIT |
| pywinpty | MIT |
| pywebview | BSD-3-Clause |

## Frontend (bundled in `static/vendor/`, no network access needed at runtime)

| Component | Version | License |
|---|---|---|
| Tailwind CSS (compiled to `vendor/tailwind.css`) | 3.4.17 | MIT |
| Font Awesome Free | 6.4.0 | Icons: CC BY 4.0, Fonts: SIL OFL 1.1, Code: MIT |
| xterm.js (+ fit, web-links, search addons) | 5.3.0 / 0.8.0 / 0.9.0 / 0.13.0 | MIT |
| Monaco Editor | 0.45.0 | MIT |
| Inter (latin subset, via Fontsource) | - | SIL OFL 1.1 |
| JetBrains Mono (latin subset, via Fontsource) | - | SIL OFL 1.1 |

License files for these components are included next to them under `static/vendor/`.

## Desktop shell

If the distributed `EZCode.exe` is built with Tauri: MIT or Apache-2.0 (dual-licensed).

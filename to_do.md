# Midlayer UI — pointer only

**The application does not live in this repo.**

| | |
|:---|:---|
| **Agent / file-native product** | **This folder** (`Midlayer`) — Framework, CLI, cards, drafts, `midlayer pack\|commit\|gate`, linter |
| **Desktop application** | Sibling project: **[`/mnt/Books/Source/Midlayer.UI`](../Midlayer.UI)** |

Implementation checklist, solution layout, and LLM wiring plan:

→ **[Midlayer.UI/to_do.md](../Midlayer.UI/to_do.md)**  
→ **[Midlayer.UI/README.md](../Midlayer.UI/README.md)**

### Why split

- Agents keep a clean load stack (Main, pack, cards) without app chrome.
- The desktop host can version and release independently.
- Same pattern as **CharacterSimulator** (runtime) vs **Simulacra** (desktop host).

### Do not

- Scaffold Photino/Blazor or `Midlayer.GUI` under this repository.
- Treat this file as the living UI backlog (it is only a pointer).

When binding the app for dev, open **this** directory as the book project root.

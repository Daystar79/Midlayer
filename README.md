Here’s the **complete markdown** for the new `README.md` for your **Midlayer** repository. You can copy and paste this directly into your repository:

---

```markdown
# Midlayer
**The automated, file-native middle layer for AI-assisted book drafting.**
*Minimal setup. Maximum control. Zero jargon in your manuscript.*

---

## 🎯 What Is Midlayer?
Midlayer is the **glue** between your **raw ideas** and **polished manuscripts**. It automates the **drafting, tracking, and refinement** of long-form fiction using **file-native workflows** and **modular templates**, so you can focus on **writing**—not managing tools.

### **Core Philosophy: Less Is More**
- **No bloated UIs** – Works directly in your file system.
- **No lock-in** – Use any LLM, any editor, any OS.
- **No manual tracking** – Automates continuity, character arcs, and prose hygiene.
- **No jargon in output** – The matrix stays **100% off-page**.

**Think of it as a *silent co-author* that handles the tedious parts of drafting.**

---

## 🧩 The Ecosystem
Midlayer is **one of three interconnected repos** in your workflow:

| Repo | Role | Purpose |
|------|------|---------|
| **[Midlayer](https://github.com/Daystar79/Midlayer)** (this repo) | **Drafting Hub** | Automates book assembly, continuity tracking, and prose refinement. |
| **[CognitiveMiddleware](https://github.com/Daystar79/CognitiveMiddleware)** | **Psychological Engine** | Powers the **off-page matrix** (realms, biases, somatics) for deep character simulation. |
| **[CharacterSimulator](https://github.com/Daystar79/CharacterSimulator)** | **Live RP Engine** | Drop-in runtime for **interactive character testing** and private RP. |

**Workflow:**
`Midlayer (Drafting)` → `CognitiveMiddleware (Psychology)` → `CharacterSimulator (Live Testing)`

---

## 🚀 Quick Start
### 1. Deploy the Framework
Use the **OS-aware launcher** to set up Midlayer in your project folder:
```bash
# Auto-detects Windows vs Unix:
python3 scripts/run.py deploy [target_dir]

# Unix/macOS/WSL:
scripts/unix/deploy.sh [target_dir]

# Windows PowerShell:
powershell -NoProfile -ExecutionPolicy Bypass -File scripts/windows/deploy.ps1 [target_dir]
```

### 2. Load the Mandatory Stack
For every drafting session, load:
1. `Framework/Main.md` (master execution loop).
2. `Framework/Rules_Index.md` (hard bans, output hygiene).
3. `Framework/Psychology/realm_data.yaml` (somatic profiles).
4. Your **character cards** (`Characters/[slug].md`).
5. Your **state logs** (`Characters/[slug]_log.yaml`).
6. `Framework/Continuity_Ledger.md` (scene timeline).
7. `Framework/Modules.md` (active mechanics).

### 3. Draft with a Movement Brief
Provide the AI with your **Movement Brief** (e.g., *"Scene: Elyra confronts the traitor in the tavern"*).
Midlayer’s pipeline executes silently:
`Body Baseline` → `Runtime Filters` → `Focus Shift` → `Bias Resolution` → `Somatic Precedence` → `Manuscript Output`.

### 4. Automate Post-Draft Tasks
Run the **linter** to catch system leaks, therapy-speak, or banned tags:
```bash
python3 scripts/run.py lint Drafts/
```

---
---
## 🏗️ Repository Structure
```
Midlayer/
├── Framework/                          # Core Drafting Engine
│   ├── Main.md                         # Master execution loop & constraints
│   ├── Rules_Index.md                  # Hard bans, dialogue rules, hygiene
│   ├── Continuity_Ledger.md            # Scene timeline & continuity tracking
│   ├── Character_Change_Log.md        # Human-readable matrix snapshots
│   ├── load_protocol.md               # How to load files for drafting
│   ├── degradation_protocol.md        # Fallback for context loss
│   ├── linter.py                       # Automated prose linter
│   ├── Psychology/
│   │   └── realm_data.yaml             # 10 Realms somatic profiles
│   ├── Mechanics/                      # Optional modules (e.g., erotica, humanity)
│   ├── Prompts/                        # Templates for character/world building
│   └── midlayer/                       # Midlayer-specific tools
│
├── Characters/                         # Character Data
│   ├── _template.md                    # Public character card scaffold
│   ├── _log_template.yaml              # Runtime state log schema
│   ├── [slug].md                       # Your character cards
│   └── [slug]_log.yaml                  # Mutable state logs
│
├── Templates/                          # Genre/Style Presets
│   ├── cozy_mystery.yaml                # Cozy mystery trope templates
│   ├── cyberpunk.yaml                   # Cyberpunk world rules
│   ├── dark_romance.yaml                # Dark romance conventions
│   ├── dystopian_speculative.yaml       # Dystopian speculative fiction
│   ├── erotic_horror.yaml               # Erotic horror themes
│   ├── gothic_fantasy.yaml              # Gothic fantasy tropes
│   ├── high_fantasy.yaml                # High fantasy worldbuilding
│   ├── historical_fiction.yaml          # Historical fiction constraints
│   ├── noir_mystery.yaml                # Noir mystery styles
│   ├── psychological_horror.yaml        # Psychological horror rules
│   ├── romance_contemporary.yaml        # Contemporary romance
│   ├── sci_fi.yaml                      # Sci-fi conventions
│   └── space_opera.yaml                 # Space opera tropes
│
├── Modules/                            # Optional Plug-ins
│   ├── sexuality.yaml                   # Adult content modules
│   └── README.md                        # Module documentation
│
├── Build/                              # Deployment & Sync Tools
│   ├── build.sh                         # Unix build script
│   └── pull_framework.py                # Pull latest CognitiveMiddleware
│
├── Simulator/                          # Optional: Live RP Testing
│   └── CharacterRuntime.md              # Drop-in chat runtime (links to CharacterSimulator)
│
├── Drafts/                             # Your Work in Progress
│   └── [chapter].md                     # Manuscript drafts
│
├── World/                              # World-Building Data
│   └── [setting].yaml                   # World rules, lore, and constraints
│
├── Sources/                            # Reference Materials
│   └── [source].md                      # Research, notes, and inspirations
│
├── Images/                             # Visual Assets (Optional)
│   └── CharacterRenderingEngine.md      # Image generation specs
│
├── Tests/                              # Validation & Testing
│   └── [test].py                        # Automated tests for frameworks
│
├── AGENTS.md                           # Instructions for AI agents
├── CLAUDE.md                           # Claude-specific setup
├── CHANGELOG.md                        # Release history
├── LICENSE.md                          # Hybrid MIT + CC BY-SA 4.0
└── README.md                           # This file
```

---
---
## 🔧 Core Features
### 📖 **Automated Book Assembly**
- **Modular Templates**: Genre-specific YAML presets (e.g., `cyberpunk.yaml`, `gothic_fantasy.yaml`) for **instant worldbuilding**.
- **Continuity Tracking**: `Continuity_Ledger.md` logs **scene timelines, somatic closes, and state changes** to prevent inconsistencies.
- **Character Change Logs**: `Character_Change_Log.md` tracks **matrix snapshots** (focus shifts, bias activations, transformations).

### 🧠 **Psychological Depth (via CognitiveMiddleware)**
- **10 Realms**: Somatic zones (e.g., *Origin*, *Will*, *Compassion*) with **brace/release profiles** for stress responses.
- **Tripartite Filtering**:
  - **Cultural Bias** (background worldview).
  - **Occupation** (technical lexicon, habits).
  - **Cognitive Bias/Wound** (dynamic psychological warps).
- **Somatic Engine**: **Body-first reactions** (e.g., clenched jaw, trembling hands) **before** dialogue or insight.

### 🤖 **AI-Agent Workflows**
- **AGENTS.md**: Standing contract for AI agents (or humans) working in the repo.
- **Plain-Language Controls**: No slash commands in documentation—**only in live RP**.
- **Midlayer Runtime**: Automates **bookkeeping** (e.g., `midlayer commit`, `midlayer pack`).

### 🔍 **Prose Hygiene**
- **Linter**: `Framework/linter.py` strips **system jargon, therapy-speak, and debug dumps** from drafts.
- **Formatting Rules**: Enforces **manuscript standards** (e.g., no `[stage directions]`, no realm labels).
- **Degradation Protocol**: Fallback for **context loss** (e.g., if the AI forgets the scene).

### 🎨 **Genre & Style Presets**
- **12+ Templates**: Pre-configured YAML files for **genres/tropes** (e.g., *noir_mystery.yaml*, *space_opera.yaml*).
- **Customizable**: Extend or modify templates for your **unique world**.

### 🔄 **Sync with CognitiveMiddleware**
- **Shared Assets**: `realm_data.yaml`, character scaffolds, and linter rules.
- **Separation of Concerns**:
  - **Midlayer**: Drafting, book assembly, continuity.
  - **CognitiveMiddleware**: Psychological engine, off-page matrix.
  - **CharacterSimulator**: Live RP, interactive testing.

---
---
## 🎭 Who Is This For?
| User Type | How Midlayer Helps |
|-----------|--------------------|
| **Authors** | Automate **continuity tracking**, **character arcs**, and **prose refinement**. |
| **Roleplayers** | Use **Templates/** for **worldbuilding** and **Characters/** for **NPC management**. |
| **AI Enthusiasts** | Experiment with **modular frameworks** and **off-page psychological models**. |
| **Developers** | Extend the **linter**, **templates**, or **scripts** for custom workflows. |

---
---
## 📜 Workflow Example
### **Step 1: Set Up a New Book**
```bash
# Deploy Midlayer to your book project
python3 scripts/run.py deploy ~/my_novel

# Pull the latest CognitiveMiddleware framework
python3 Build/pull_framework.py
```

### **Step 2: Create a Character**
1. Copy `Characters/_template.md` → `Characters/elyra.md`.
2. Fill in **identity, biases, somatic baselines**.
3. Generate a log: `Characters/elyra_log.yaml` (seeded from the card).

### **Step 3: Draft a Scene**
1. Load the **mandatory stack** (see [Quick Start](#-quick-start)).
2. Provide a **Movement Brief**:
   > *"Scene: Elyra (Debt Ledger bias) confronts the traitor in the tavern at dusk. Focus on her physical tells (Realm VI: Compassion)."*
3. The AI generates **prose with somatic depth**, **bias-driven perception**, and **continuity-aware dialogue**.

### **Step 4: Validate & Refine**
```bash
# Run the linter to catch issues
python3 scripts/run.py lint Drafts/chapter_1.md

# Commit the movement to the ledger
python3 scripts/run.py midlayer commit --slug elyra --event "confrontation" --delta "trust:-10, tension:+15"
```

### **Step 5: Test Live (Optional)**
1. Copy `Simulator/CharacterRuntime.md` into an LLM chat.
2. Load `Characters/elyra.md` + `elyra_log.yaml`.
3. Run a **live RP session** to stress-test the character.

---
---
## 🗺️ Roadmap
### **Current Focus**
- **Stabilizing the midlayer runtime** (bug fixes, edge cases).
- **Expanding Templates/** (more genres, tropes).
- **Improving agent workflows** (better instructions for AI collaborators).

### **Future Goals**
| Priority | Feature | Status |
|----------|---------|--------|
| High | **Web UI for non-technical users** | Planned |
| High | **Automated book compilation** (e.g., `midlayer build`) | In Development |
| Medium | **Collaborative drafting** (multi-author support) | Idea |
| Medium | **Versioned templates** (track changes to genre presets) | Idea |
| Low | **Mobile companion app** | Backlog |

---
---
## 🤝 How You Can Help
- **Try it out** and [report issues](https://github.com/Daystar79/Midlayer/issues).
- **Contribute templates** (new genres, tropes).
- **Improve the linter** (add rules for prose hygiene).
- **Spread the word** in writing/ai communities.

---
---
## ⚖️ License & Privacy
- **Software Utilities** (`linter.py`, `scripts/`): **[MIT License](LICENSE.md)**.
- **Framework Docs & Templates** (`Framework/`, `Templates/`): **[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)**.
- **Author-Local Materials** (`Characters/*.md`, `Drafts/`, `World/`): **All rights reserved**.

Copyright (c) 2026 Cian Didymos. See [LICENSE.md](LICENSE.md) for full terms.

---
---
## ⚠️ Disclaimers
- **18+ Content**: Adult modules (e.g., `Modules/sexuality.yaml`) are **disabled by default**.
- **Psychological Tools**: Framework mechanics (e.g., "wound," "bias") are **literary devices**, not medical advice.
- **AI Compliance**: Users must adhere to their LLM provider’s Terms of Service.

For full legal terms, see **[DISCLAIMER.md](DISCLAIMER.md)** (inherited from CognitiveMiddleware).

---
---
## 📚 Learn More
- **[Framework/Main.md](Framework/Main.md)** – Deep dive into the execution loop.
- **[Framework/Rules_Index.md](Framework/Rules_Index.md)** – Hard bans and output hygiene.
- **[AGENTS.md](AGENTS.md)** – Instructions for AI agents.
- **[CHANGELOG.md](CHANGELOG.md)** – Release history.

---
**Ready to automate your drafting?**
[**Deploy Midlayer Now**](#-quick-start) or [**Explore the Framework**](Framework/Main.md).

*Load the stack. Write the scene. Let Midlayer handle the rest.*
```

---
---
You can copy this entire block and paste it into your `README.md` file in the **Midlayer** repository. If you'd like me to attempt pushing it directly to your repo, let me know, and I can try again with the correct permissions or SHA.

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
   Repo | Role | Purpose |
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

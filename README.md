<p align="center">
  <img src="https://raw.githubusercontent.com/RAEN-DT/PyNet/main/Assets/PyNetLogo.png" width="400"/>
</p>

<p align="center">
  <a href="https://github.com/RAEN-DT/PyNet/releases"><img src="https://img.shields.io/github/v/release/RAEN-DT/PyNet?label=release&color=f78166" alt="Release"/></a>
  <img src="https://img.shields.io/badge/python-3.10%2B-blue" alt="Python"/>
  <img src="https://img.shields.io/badge/platform-Windows-lightgrey" alt="Windows"/>
  <img src="https://img.shields.io/badge/hosts-Navisworks%20%C2%B7%20Revit%20%C2%B7%20Civil%203D-orange" alt="Hosts"/>
  <img src="https://img.shields.io/badge/MCP-compatible-8A2BE2" alt="MCP"/>
</p>

#

**PyNET Platform** is an AI-driven BIM automation platform that connects natural language, Python execution, and Autodesk **Navisworks, Revit and Civil 3D** into a unified workflow.

### 📥 Request the 30 days **Trial** here: 
Contact: **info@raendt.com** to request access.

### 📥 Review the latest Release here:
**[Available Release](https://github.com/RAEN-DT/PyNet/releases)**

### PyNET Platform Ecosystem

PyNET platform use the following Ecosistem to automate BIM tasks using AI.

<p align="center">
  <img src="https://raw.githubusercontent.com/RAEN-DT/PyNet/main/Assets/PyNetPlatformStructure.png" width="1000"/>
  <br>
  
</p>

| Component | Repository | Purpose |
| :--- | :--- | :--- |
| **PyNet Platform** | [PyNet](https://github.com/RAEN-DT/PyNet) | Navisworks/Revit/Civil 3D plugin that hosts the Python.NET engine providing UI Layer and AI integration with BIM Models |
| **PyNet Bridge (MCP)** | [PyNetBridge](https://github.com/RAEN-DT/PyNetBridge) | MCP server that connects AI models to PyNET with including secure scripts validation |
| **PyNet Library** | [PyNetLibrary](https://github.com/RAEN-DT/PyNetLibrary) | Python Scripts reference library for Revit, Navisworks and Civil 3D and AI context|
| **PyNet for VS Code** | [PyNetVSCode](https://github.com/RAEN-DT/PyNetVSCode) | VS Code extension: embedded BIM viewer + one-click install of the MCP bridge across every AI client |

---

## 🚀 The AI-Powered BIM Loop

**PyNET Platform** introduces a closed-loop AI-assisted execution system, turning Navisworks into an intelligent, conversational co-pilot. Unlike static plugins, PyNET Platform learns and adapts to the specific needs of your BIM model.

[🎬 Watch here AI Navisworks Coordination Workflow](https://www.youtube.com/watch?v=Sfq9iXJFacU)  

### 🔄 How it works:
* **Intent:** The user requests an action in natural language (e.g., *"Find all clashes in Level 1 and export them to Excel"*).
* **Generation:** The AI generates a specialized Python script using the Navisworks API.
* **Execution:** The script is processed via the PyNET Platform .NET listener and executed locally.
* **Self-Correction:** If a script fails, the system captures the exception and can optionally feed the error back to the AI for iterative correction, depending on the configured workflow.
* **Structured Results:** Final data is returned via the `ia_Result` contract, ensuring consistent and validated feedback.

---

## ✨ Key Features

* 🧠 **AI Self-Correction:** Automated debugging and iterative refinement of automation workflows.
* 🐍 **Embedded Python .NET:** Run a full Python interpreter directly inside Navisworks.
* 📚 **Data Science Ready:** Supports integration with libraries such as NumPy, Pandas, and Scikit-Learn for advanced data processing and analysis.
* 🔘 **Custom UI Engine:** Create dockable panels and connect Python scripts to custom ribbon buttons for deployment within Navisworks.
* ⚙️ **Configurable Environment:** Define your own Python installation path and script repositories.

---

## 🏗️ Core Use Cases

* **Intelligent Model Interrogation:** Query complex BIM metadata using natural language.
* **Automated Clash Management:** Custom analysis pipelines beyond native Navisworks capabilities.
* **Machine Learning in BIM:** Apply ML frameworks for predictive auditing and risk assessment.
* **Rule-Based Validation:** Highly complex, Python-driven logic for BIM standard enforcement.
* **Automated Reporting:** Generate structured data outputs directly from model geometry.

---

## 📥 Installation & Licensing

### 1️⃣ Beta Availability
PyNET Platform will be distributed via the Freemius platform to ensure secure licensing and controlled access.


| License | Description |
| :--- | :--- |
| **Beta Trial** | 30-day trial access to a basic license. | 
| **Basic** | Access to a basic license for the extension to integrate the Autodesk products available individually. | 
| **Pro** | Access to a Pro license for the extension to integrate the Autodesk products available at the same time. |
| **Enterprise** | integrate PyNET in your company with an implantation project service. |

### 2️⃣ Configuration
Upon first launch in Navisworks (under the **RAEN Tools** tab):
* Activate your license via the secure activation window.
* Set your local Python installation path.
* Define the folder where your Python scripts are stored.

| Tutorial | Description | Video |
| :--- | :--- | :--- |
| **Configuration for navisworks Manage** | How to configure PyNet platform Addin in Navisworks Manage. | [🎬 Watch here](https://www.youtube.com/watch?v=3eR5GAOkEug)  |
| **Browse for navisworks Manage** | How to browse scripts PyNet platform Addin in Navisworks Manage. | [🎬 Watch here](https://www.youtube.com/watch?v=rHwAKqU6Vck)  |
| **Manage PyNet for navisworks Manage** | How to manage output messages and user interface costumization| [🎬 Watch here](https://www.youtube.com/watch?v=furMbMkhiCU)  |

---

## 🤖 AI Integration via MCP (Model Context Protocol)

PyNET Platform connects to AI models through **[PyNet Bridge](https://github.com/RAEN-DT/PyNetBridge)**, an MCP server that exposes PyNET tools to compatible AI clients.

This allows AI systems to generate and execute scripts that interact directly with Navisworks, Revit, and Civil 3D.

### ⚡ One-line install

> ⚠️ **Prerequisites:** Python 3.10 or higher must be installed on your system (3.14 is supported). For VS Code extensions (Claude Code, Cline, Roo Code), **Git** must also be installed → [git-scm.com](https://git-scm.com/downloads). For detailed instructions and requirements, see the [PyNet Bridge repository](https://github.com/RAEN-DT/PyNetBridge).

The simplest route is the **[VS Code extension](https://github.com/RAEN-DT/PyNetVSCode)**,
which installs and configures everything on first launch — and gives you the BIM viewer too.

To install the bridge on its own, from PyPI:

```powershell
pip install pynet-mcp-bridge
```

Or, using PowerShell, the scripted installer that also writes the config for every client:

```powershell
irm https://raw.githubusercontent.com/RAEN-DT/PyNetBridge/main/install.ps1 | iex
```

Either way, the MCP server is auto-detected and configured for all supported AI clients:
- **Claude Desktop** (standard and Microsoft Store)
- **Claude Code** (VS Code extension / CLI)
- **GitHub Copilot** (VS Code)
- **Codex**
- **Cline** (VS Code extension)
- **Roo Code** (VS Code extension)

| Tutorial | Description | Video |
| :--- | :--- | :--- |
| **PyNET and Codex Integration** | How to configure PyNet bridge with Codex and query into Navisworks. | [🎬 Watch here](https://youtu.be/HdmbCO_pTN0)  |

> For manual setup or other clients, see the [PyNet Bridge repository](https://github.com/RAEN-DT/PyNetBridge).

**Important Note on AI Providers:**
PyNET Platform acts as the integration bridge between AI models and Autodesk tools. **Access to AI models (such as Claude AI, OpenAI, etc.) is not included with the tool.** Users must provide their own integration or use the platform to bridge their existing AI workflows into the Autodesk ecosystem. PyNET Platform is the engine that enables these AIs to "understand" and "operate" Navisworks, Revit, and Civil 3D.

---

## 🧊 BIM Viewer in VS Code

The **[PyNet Platform extension for VS Code](https://github.com/RAEN-DT/PyNetVSCode)**
embeds a 3D BIM viewer directly in the editor and installs the MCP bridge for you.

Export a `.pnt` package from Navisworks and open it in VS Code to navigate the federated model —
spatial tree, element properties, sections, measurements and clash results — while your AI
assistant drives the same scene: selecting elements, isolating a discipline, or highlighting the
two sides of a clash as it explains them.

* **The viewer is free.** No licence needed to open and explore a package.
* **Nothing leaves your machine** — the viewer server binds to localhost.
* Installing the extension also installs and configures the MCP bridge, so a single install
  covers both.

> 📦 Coming to the Visual Studio Code Marketplace. Until then, grab the latest `.vsix` from the
> [extension repository](https://github.com/RAEN-DT/PyNetVSCode).

---

## 🔒 Privacy & Security

* **Local Execution:** All Python scripts are executed within your local environment.
* **Data Sovereignty:** No BIM data is transmitted externally during script runtime.
* **Controlled AI:** While AI generates the code, the execution remains under the user's local security protocols.
* **AI-generated code** may be processed by external AI providers depending on the user's chosen integration.

---

## ❓ FAQs

Have questions about installation, configuration, or usage? Check the full FAQ page:

👉 [PyNet FAQs](https://github.com/RAEN-DT/PyNet/wiki/PyNET-FAQs)

---

## ⚠️ Disclaimer

PyNET Platform is intended for professional use in BIM automation. Users are responsible for reviewing, validating, and ensuring the correctness of AI-generated scripts before applying them in production environments.

---

<p align="center">
  <img src="https://raw.githubusercontent.com/RAEN-DT/PyNet/main/Assets/RAENDigitalTools.png" alt="RAEN Digital Tools" width="180"><br/><br/>
  <sub>© 2026 RAEN Digital Tools · Todos los derechos reservados.<br/>
  Obra inscrita en el Registro de la Propiedad Intelectual de la Comunidad de Madrid.</sub>
</p>

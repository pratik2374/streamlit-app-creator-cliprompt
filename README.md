**Project**
 - **Name**: `app_gen` — Streamlit app scaffold for a specialized AI model
 - **Purpose**: Provide a clean, modular Streamlit application that follows the specifications in `streamlit_app.md`. All user inputs and settings are collected exclusively from the Streamlit sidebar.

**Goal**

 - **Short**: Build a production-ready Streamlit UI that collects API keys, model settings, chat controls, file uploads and other parameters only from the sidebar, runs model inference, and displays results in the main layout.

**Required Reference**

 - **Design & Requirements**: See `streamlit_app.md` for the full goal, mandatory sidebar and branding blocks, chatbot/agent rules, and UI requirements. This README summarizes how to get started.

**Quickstart**

 - **Prerequisites**: Install Python 3.10+ and create a virtual environment.

 - **Install dependencies**: Add dependencies to a `requirements.txt` (not included here). Example installation commands (PowerShell):

```powershell
python -m venv .venv; .\.venv\Scripts\Activate.ps1; pip install -U pip
pip install streamlit
```

 - **Run the app**: From the project root run:

```powershell
streamlit run app.py
```

**Project Layout (suggested)**

 - **`app.py`**: Main Streamlit app entrypoint. Contains the sidebar-only input collection and UI glue.
 - **`streamlit_app.md`**: Project specification and mandatory sidebar branding block (already present).
 - **`agno_info.txt`**: Reference for agent syntax and examples (used only when implementing agents).
 - **`README.md`**: This file.

**Sidebar Requirements (summary)**

 - **All inputs in sidebar**: API keys, model selection and settings, toggles, sliders, file upload controls, chat config.
 - **Branding block**: Include the exact HTML branding snippet provided in `streamlit_app.md` inside the sidebar.

**Chat & Agents (if implemented)**

 - **Chat**: Use `st.chat_input()` and maintain message history and memory for multi-turn conversations.
 - **Agents**: If you add agents, follow `agno_info.txt` for syntax and ensure specialized agents and clean input/output pipelines.

**Development notes**

 - Keep the UI minimal, modular and professional. Prefer small functions/modules for:
	 - sidebar input collection
	 - model inference wrappers
	 - UI rendering of outputs
 - Prefer configuration via environment variables for secrets in development (but the Streamlit UI must still collect keys in the sidebar per spec).

**Next steps**

 - Implement `app.py` following `streamlit_app.md` requirements. Include a `requirements.txt` capturing dependencies used (e.g., `streamlit`, any model SDKs).
 - Optionally add a simple example model stub so reviewers can run the app without external API keys.

**Contact / References**

 - Specification: `streamlit_app.md`
 - Agent framework docs: `agno_info.txt`

**License**

 - Add a license file if this project will be shared publicly.


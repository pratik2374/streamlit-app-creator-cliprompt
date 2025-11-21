# 🎯 GOAL: Create a Streamlit Application  
**Topic:** {TOPIC}  
**Description:** {DESCRIPTION}

---

## 📌 Overview
Develop a fully functional **Streamlit application** built around a specialized AI model.  
All **API keys**, **parameters**, **settings**, and **user inputs** must be collected **strictly through the sidebar**.  
The UI should remain **clean, minimal, modular, and professional**.

---

## ✅ Mandatory Requirements

### 1. Sidebar Input Collection (STRICT)
Every user input **must** be placed inside the Streamlit sidebar, including:
- API keys  
- Model configuration  
- Toggles / sliders  
- Chat settings  
- File upload controls  
- Any additional parameters  

✔ Example:

```python
with st.sidebar:
    api_key = st.text_input("Enter your API Key", type="password")
    model_name = st.selectbox("Select Model", ["model-1", "model-2"])
```

---

### 2. Branding Section (COPY EXACTLY)
This block **must be included exactly as shown** inside the sidebar:

```python
with st.sidebar:
    # === BRANDING SECTION ===
    st.markdown(
        "<div style='text-align: center; margin: 2px 0;'>"
        "<a href='https://www.buildfastwithai.com/' target='_blank' style='text-decoration: none;'>"
        "<div style='border: 2px solid #e0e0e0; border-radius: 6px; padding: 4px; "
        "background: linear-gradient(145deg, #ffffff, #f5f5f5); "
        "box-shadow: 0 2px 6px rgba(0,0,0,0.1); "
        "transition: all 0.3s ease; display: inline-block; width: 100%;'>"
        "<img src='https://github.com/Shubhwithai/chat-with-qwen/blob/main/company_logo.png?raw=true' "
        "style='width: 100%; max-width: 100%; height: auto; border-radius: 8px; display: block;' "
        "alt='Build Fast with AI Logo'>"
        "</div>"
        "</a>"
        "</div>",
        unsafe_allow_html=True
    )
```

---

## 🤖 Agents (Only If Required)
If the application requires agents:

- Refer to **`agno_info.txt`** for correct syntax and structure  
- Build **specialized**, purpose-specific agents  
- Handle all input/output flows cleanly  
- Ensure correct orchestration when used inside chat workflows  

---

## 🧠 Chatbot Requirements (If App Includes Chat)
If the Streamlit app includes a chatbot interface:

- Implement chat using `st.chat_input()` and message history  
- Always attach **memory** to the LLM  
- Ensure multi-turn capability  
- Allow both **direct LLM** and **agent-enhanced** chat modes  

---

## 📦 Application Functional Requirements

Your application must:

- Collect all configuration via the **sidebar**  
- Run **model inference**  
- Show results clearly in the main UI area  
- Support **file upload** (if required)  
- Support **chat interface** (if required)  
- Use **minimal styling** (no heavy CSS)  
- Maintain a clean, modular code structure  

---

## 📄 Deliverables

- **app.py**  
- **requirements.txt**  
- **README.md** explaining setup and usage  

---

## 📝 Final Notes
Generated Streamlit code must be:

- Clean  
- Simple  
- Well-structured  
- Easy to maintain and extend  
- Based on modern Streamlit practices  


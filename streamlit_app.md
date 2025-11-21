# 🎯 GOAL: Create a Streamlit Application  
**Topic:** {TOPIC}  
**Description:** {DESCRIPTION}

---

## 📌 Overview
Build a fully functional **Streamlit application** designed for a specialized AI model.  
All **API keys**, **parameters**, **settings**, and **user inputs** must be collected **exclusively from the sidebar**.  
The overall UI must remain **clean, modular, simple, and professional**.

---

## ✅ Mandatory Requirements

### 1. Sidebar Input Collection (STRICT)
Every user input **must** be inside the Streamlit sidebar — including:
- API keys  
- Model settings  
- Toggles & sliders  
- Chat configurations  
- File upload controls  
- Any other parameters  

✔ **Example:**

```python
with st.sidebar:
    api_key = st.text_input("Enter your API Key", type="password")
    model_name = st.selectbox("Select Model", ["model-1", "model-2"])
```

---

### 2. Branding Section (COPY EXACTLY)
This block **must be included exactly** inside the sidebar:

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
If the user’s requirements include **agents**, then:

- Refer to **`agno_info.txt`** for correct agent syntax  
- Build **specialized agents** (not generic)  
- Ensure input & output pipelines are handled cleanly  
- When using agents for chatbot workflows, ensure proper orchestration  

---

## 🧠 Chatbot Requirements (If App Includes Chat)
If the Streamlit app includes a chatbot:

- Provide a chat interface using `st.chat_input()` & message history  
- Always include **memory** with the LLM  
- Ensure multi-turn conversation works properly  
- Support agent-based or direct-LLM chat depending on user’s goal  

---

## 📦 Application Functional Requirements

Your app must include:

- Collect all settings via **sidebar**
- Run **model inference**
- Display results cleanly in the **main layout**
- Support **file upload**, if needed
- Support **chat interface**, if required
- Use minimal UI styling (no heavy CSS or themes)
- Organize code cleanly (functions or modular design preferred)

---

## 📝 Final Notes
Your generated Streamlit code should be:
- Clean  
- Simple  
- Well-structured  
- Easy to extend  
- Consistent with modern Streamlit practices  


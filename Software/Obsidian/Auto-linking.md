---
created: 2025-01-29T01:11:37-06:00
tags:
  - Obsidian
---

## **📝 Auto-Linking in Obsidian (Virtual Linker + Dataview)**

### **🔗 1. Virtual Linker (Auto-Linking While Typing)**

📌 **Purpose:** Automatically creates internal links to existing notes based on text matches.

### **🛠 Installation & Setup**

1. **Install Virtual Linker Plugin**
    
    - Go to **Settings → Community Plugins → Browse**
    - Search for **Virtual Linker / Glossary**
    - Click **Install & Enable**
2. **Configure Virtual Linker**
    
    - Go to **Settings → Virtual Linker**
    - Adjust settings:
        - **Enable Auto-Linking** ✅
        - **Enable Auto-Suggestions** ✅
        - **Match Sensitivity:** Set to **Medium**
3. **How It Works:**
    
    - When typing, **any word matching a note title** is automatically linked:
        - Example: Writing `"User Research"` → **becomes** `[[User Research]]`
    - If multiple notes match, **suggestions appear**.

---

### **📂 2. Dataview (Dynamic Reference List)**

📌 **Purpose:** Dynamically lists **related notes** at the bottom of a file.

### **🛠 Installation & Setup**

1. **Install Dataview Plugin**
    
    - Go to **Settings → Community Plugins → Browse**
    - Search for **Dataview**
    - Click **Install & Enable**
2. **Add Dynamic References to Each Note**
    
    - Open your **Templater note template**
    - Add the following **DataviewJS script** to dynamically list related notes:

---

### **📌 DataviewJS Code Block**

````markdown
## Dynamic References

```dataviewjs
const currentTitle = dv.current().file.name;
dv.list(dv.pages().where(p => p.file.outlinks.includes(dv.current().file.link)).file.link);
```
````

**What This Does:**
✅ Automatically lists **all notes that link to the current note**  
✅ Updates in **real-time** when new links are added  
✅ Works in **every new note** created with the template  

---

### **📝 Final Steps:**
- **Apply this to your note template** in **Templater**.  
- **Disable Obsidian's default template plugin** to avoid conflicts.  
- **Test:** Create a note and check if auto-linking + references work!  

---

### **🎯 Summary**
| Feature | Plugin | Functionality |
|---------|--------|--------------|
| **Auto-Linking** | Virtual Linker | Creates `[[links]]` as you type |
| **Dynamic References** | Dataview | Lists notes linking to the current note |

🚀 **Now, all your notes are auto-linked and dynamically connected!**  

---

# 🌑 Node.js Backend Snippets 

## ⚡ Supercharge Your Node/Express Development 

<p align="center">
  <img src="./images/icon.png" width="100%" />
</p>
## Full-stack ready snippets for Node/Express: CRUD controllers, auth flows, Mongoose models, MongoDB connect, JWT middleware, and Express routes. Works in VS Code, Cursor, VSCodium, Code OSS, and Zed.

<p align="center">
  <img src="https://img.shields.io/badge/VS%20Code%20Extension-Node.js%20Backend%20Snippets-3c9?style=for-the-badge&logo=visualstudiocode" />
  <img src="https://img.shields.io/badge/Version-1.0.0-blueviolet?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-gray?style=for-the-badge" />
</p>

<p align="center">
  <span style=" color: #ffffff; padding: 12px 24px; border-radius: 8px;  display: inline-block; box-shadow: 0 4px 15px rgba(102, 126, 234, 0.4);">
    🚀 Explore all my extensions and guides: <a href="https://codingyari.com" style="color: #ffd700; text-decoration: none; text-shadow: 0 2px 4px rgba(0,0,0,0.3);">codingyari.com</a> ✨
  </span>
</p>  



---

## 🖤 Why This Extension?
A dark-themed, optimized snippet pack that instantly generates:

- CRUD Controllers
- Authentication Flows
- User Model (bcrypt + JWT)
- JWT Middleware
- MongoDB Connection Helper
- Express Routes
- And much more...

⚡ **Type a shortcut → Get full backend code — instantly.**

---

##  Folder Structure 
```
nodejs-backend-snippets/
│
├── images/
│   ├── HeroDark.png
│   ├── ShortcutsDark.png
│   └── DemoDark.gif
│
├── snippets/
│   └── backend-snippets.json
│
├── package.json
├── CHANGELOG.md
└── README.md
```

---

## ⚡ Shortcuts Overview

<p align="center">
  <img src="./images/Shortcuts.png" width="80%" />
</p>

---

## 🧩 Shortcut → Snippet Map
| 🚀 Shortcut | 📝 Action |
|------------|-----------|
| `ndc` | Create Controller |
| `ndg` | Get Controller |
| `ndu` | Update Controller |
| `ndd` | Delete Controller |
| `ndcurd` | All CRUD Controllers |
| `ndm` | Mongoose Model |
| `ndcu` | Register User |
| `ndcul` | Login User |
| `ndcug` | Get Profile |
| `ndcuu` | Update Profile |
| `ndco` | Logout User |
| `ndcum` | User Model (bcrypt + JWT) |
| `ndauth` | JWT Auth Middleware |
| `nddb` | MongoDB Connection Helper |
| `ndroute` | Express CRUD Router |

> 💡 **Usage:** Type shortcut → Press `Tab` or `Enter`.

---

## 🗃 Code Structures (Dark Mode Layout)

### 📁 Controllers
```
controllers/
│
├── createData        → ndc
├── getData           → ndg
├── updateData        → ndu
├── deleteData        → ndd
└── CRUD Bundle       → ndcurd
```

---

### 👤 Authentication
```
auth/
│
├── registerUser      → ndcu
├── loginUser         → ndcul
├── getProfile        → ndcug
├── updateProfile     → ndcuu
└── logoutUser        → ndco
```

---

### 🗄 Models
```
models/
│
├── User Model (bcrypt + JWT)  → ndcum
└── Generic Model              → ndm
```

---

### 🔐 Middleware
```
middleware/
│
└── isAutherenticatedUser → ndauth
```

---

### 🌐 Database
```
database/
│
└── connectDB.js → nddb
```

---

### 🚏 Routes
```
routes/
│
└── CRUD Router → ndroute
```

---

## 📦 Installation

### **VS Code / Cursor / VSCodium**
```bash
vsce package
code --install-extension nodejs-backend-snippets-*.vsix
```

### **Zed Editor**
```bash
cp snippets/backend-snippets.json ~/.config/zed/snippets/nodejs-backend-snippets.json
```

---

## 🎨 Customization & Adding More Snippets

You can easily add more code snippets and customize existing ones to fit your workflow! All snippets are stored in `snippets/backend-snippets.json` in JSON format.

### **How to Add Custom Snippets:**

1. **Open the snippets file:**
   - Navigate to `snippets/backend-snippets.json` in your project
   - Or find it in your VS Code extension folder

2. **Add a new snippet entry:**
   ```json
   "Your Custom Snippet Name (shortcut)": {
     "prefix": "your-shortcut",
     "body": [
       "export const yourFunction = async (req, res, next) => {",
       "  // Your code here",
       "  return res?.status(200).json({ success: true });",
       "};"
     ],
     "description": "Description of what this snippet does"
   }
   ```

3. **Customize existing snippets:**
   - Edit any snippet in `backend-snippets.json`
   - Change the `prefix` to modify the shortcut
   - Modify the `body` array to change the generated code
   - Use `${1:placeholder}` for tab stops (user can fill these in)

4. **Reload your editor** to apply changes

### **Example: Adding a Custom Middleware**
```json
"Custom Validation Middleware (ndval)": {
  "prefix": "ndval",
  "body": [
    "export const validateData = async (req, res, next) => {",
    "  const { ${1:field} } = req?.body ?? {};",
    "  if (!${1:field}) {",
    "    return res?.status(400).json({",
    "      success: false,",
    "      message: '${1:field} is required'",
    "    });",
    "  }",
    "  next();",
    "};"
  ],
  "description": "Custom validation middleware"
}
```

> 💡 **Tip:** Follow the existing snippet patterns in `backend-snippets.json` for consistency. You can modify field names, add validation logic, change response formats, or create entirely new controller patterns!

--- 
 

## 👤 Author
- GitHub: https://github.com/codingyaari
- Website: https://codingyari.com
- Extensions: Full list on codingyari.com

---

## 🤝 Contributing
- PRs Welcome
- Issues Welcome
- Custom snippet suggestions welcome

---

## 📜 License
**MIT — Free for personal & commercial use**


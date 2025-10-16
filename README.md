<div align="center">

# 🛡️ CodeGuardian

### Your AI-Powered Code Review & Learning Companion

[![React](https://img.shields.io/badge/React-18.0+-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactjs.org/)
[![TailwindCSS](https://img.shields.io/badge/Tailwind-3.0+-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Groq](https://img.shields.io/badge/Groq_API-Removed-FF6B6B?style=for-the-badge&logo=ai&logoColor=white)](https://groq.com/)

**Get instant code reviews, language tips, and expert guidance - all powered by AI**


</div>

---

## 🌟 Features

### 🔍 **Intelligent Code Review**
Upload your code files and get comprehensive reviews with:
- Bug detection and security vulnerabilities
- Performance optimization suggestions
- Best practices and code quality improvements
- Line-by-line analysis with actionable feedback

### 💡 **Multi-Language Support**
Get expert guidance on:
- **JavaScript/TypeScript** - Modern ES6+ features, async patterns
- **Python** - Pythonic code, PEP8 standards
- **Java** - OOP principles, design patterns
- **C/C++** - Memory management, optimization
- **And many more languages!**

### 📁 **File Import System**
- Drag-and-drop file uploads
- Support for multiple file formats (`.js`, `.py`, `.java`, `.cpp`, etc.)
- Real-time file parsing and analysis
- Syntax highlighting and code preview

### 🎓 **Interactive Learning**
- Ask questions about any programming language
- Get detailed explanations with code examples
- Learn best practices and design patterns
- Receive personalized tips based on your skill level



## 🚀 Quick Start

### Prerequisites

Before you begin, ensure you have:
- **Node.js** (v16.0 or higher)
- **npm** or **yarn**
- **MongoDB** (local or cloud instance)

### Installation
```bash
# Clone the repository
git clone https://github.com/Keshavkumarr0/codeguardian__.git

# Navigate to project directory
cd codeguardian__

# Install dependencies
npm install

# Create environment file
cp .env.example .env
```




### Run the Application
```bash
# Start development server
npm run dev

# Build for production
npm run build

# Start production server
npm start
```

Visit `http://localhost:3000` in your browser 🎉

---

## 🛠️ Tech Stack

<div align="center">

| Technology | Purpose | Version |
|------------|---------|---------|
| ![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black) | Frontend Framework | 18.2+ |
| ![Tailwind](https://img.shields.io/badge/-TailwindCSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white) | Styling | 3.3+ |
| ![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) | Database | 6.0+ |
| ![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=node.js&logoColor=white) | Backend Runtime | 16.0+ |
| ![Express](https://img.shields.io/badge/-Express-000000?style=flat-square&logo=express&logoColor=white) | API Framework | 4.18+ |

</div>

### Architecture
```
┌─────────────────────────────────────────────────┐
│                 Frontend (React)                │
│  ┌──────────────┐  ┌──────────────┐            │
│  │ Code Editor  │  │ File Upload  │            │
│  └──────────────┘  └──────────────┘            │
│  ┌──────────────┐  ┌──────────────┐            │
│  │  Review UI   │  │   Chat Bot   │            │
│  └──────────────┘  └──────────────┘            │
└─────────────────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────┐
│              Backend (Node/Express)             │
│  ┌──────────────┐  ┌──────────────┐            │
│  │ File Parser  │  │  AI Engine   │            │
│  └──────────────┘  └──────────────┘            │
└─────────────────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────┐
│                MongoDB Database                 │
│  • Review History  • User Data  • Analytics    │
└─────────────────────────────────────────────────┘
```

---


## 💻 Usage

### 1. Code Review
```javascript
// Upload your code file
const file = document.querySelector('input[type="file"]').files[0];

// Or paste code directly
const codeReview = await fetch('/api/review', {
  method: 'POST',
  body: JSON.stringify({ code: yourCode, language: 'javascript' })
});
```

### 2. Ask Questions
```
User: "How do I optimize this Python loop?"
CodeGuardian: "Here are 3 ways to optimize your loop:
1. Use list comprehension instead of append()
2. Consider using numpy for numerical operations
3. Implement generator expressions for memory efficiency..."
```

### 3. Import Files

Supported file types:
- `.js`, `.jsx`, `.ts`, `.tsx`
- `.py`, `.java`, `.cpp`, `.c`
- `.html`, `.css`, `.json`
- `.go`, `.rs`, `.rb`, `.php`

---

## ⚠️ Important Notes

### Groq API Status
> **Note:** Previous versions of CodeGuardian used the Groq API for AI-powered code analysis. This dependency has been **removed** in the current version.

If you're upgrading from an older version:
1. Remove any Groq API keys from your `.env` file
2. Update your dependencies with `npm install`
3. The core functionality remains unchanged



## 🙏 Acknowledgments

- React Team for the amazing framework
- Tailwind CSS for beautiful styling utilities
- MongoDB for robust database solutions
- Open source community for continuous inspiration



**Made with ❤️ by Keshav Kumar**

</div>

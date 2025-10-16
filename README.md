<div align="center">

# 🛡️ CodeGuardian

### Your AI-Powered Code Review & Learning Companion

[![React](https://img.shields.io/badge/React-18.0+-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactjs.org/)
[![TailwindCSS](https://img.shields.io/badge/Tailwind-3.0+-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Groq](https://img.shields.io/badge/Groq_API-Removed-FF6B6B?style=for-the-badge&logo=ai&logoColor=white)](https://groq.com/)

**Get instant code reviews, language tips, and expert guidance - all powered by AI**

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Tech Stack](#-tech-stack) • [Contributing](#-contributing)

---

![CodeGuardian Demo](https://via.placeholder.com/800x400/1a1a2e/ffffff?text=CodeGuardian+Dashboard)

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

### 💾 **History & Analytics**
- MongoDB-powered review history
- Track your code improvements over time
- Save and revisit previous analyses
- Export reports in multiple formats

---

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

### Environment Setup

Create a `.env` file in the root directory:
```env
# MongoDB Configuration
MONGODB_URI=your_mongodb_connection_string

# Server Configuration
PORT=5000
NODE_ENV=development

# Note: Groq API has been removed from this version
# Previous versions used Groq API for AI-powered analysis
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

## 📸 Screenshots

<div align="center">

### Dashboard
![Dashboard](https://via.placeholder.com/600x350/0f0f23/00d9ff?text=Interactive+Dashboard)

### Code Review Interface
![Code Review](https://via.placeholder.com/600x350/1a1a2e/16c79a?text=Real-time+Code+Analysis)

### File Upload
![File Upload](https://via.placeholder.com/600x350/16213e/f39c12?text=Drag+%26+Drop+Files)

### Language Tips
![Tips](https://via.placeholder.com/600x350/0f0f23/e74c3c?text=Expert+Programming+Tips)

</div>

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

## 🔧 Configuration

### MongoDB Setup
```javascript
// config/database.js
const mongoose = require('mongoose');

mongoose.connect(process.env.MONGODB_URI, {
  useNewUrlParser: true,
  useUnifiedTopology: true,
});
```

### Tailwind Configuration
```javascript
// tailwind.config.js
module.exports = {
  content: ['./src/**/*.{js,jsx,ts,tsx}'],
  theme: {
    extend: {
      colors: {
        primary: '#00d9ff',
        secondary: '#16c79a',
        dark: '#0f0f23',
      },
    },
  },
};
```

---

## ⚠️ Important Notes

### Groq API Status
> **Note:** Previous versions of CodeGuardian used the Groq API for AI-powered code analysis. This dependency has been **removed** in the current version. The application now uses alternative AI analysis methods.

If you're upgrading from an older version:
1. Remove any Groq API keys from your `.env` file
2. Update your dependencies with `npm install`
3. The core functionality remains unchanged

---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**
```bash
   git checkout -b feature/AmazingFeature
```
3. **Commit your changes**
```bash
   git commit -m 'Add some AmazingFeature'
```
4. **Push to the branch**
```bash
   git push origin feature/AmazingFeature
```
5. **Open a Pull Request**

### Contribution Guidelines
- Follow existing code style
- Write meaningful commit messages
- Add tests for new features
- Update documentation as needed







## 🙏 Acknowledgments

- React Team for the amazing framework
- Tailwind CSS for beautiful styling utilities
- MongoDB for robust database solutions
- Open source community for continuous inspiration



**Made with ❤️ by Keshav Kumar**

![Footer](https://via.placeholder.com/800x100/1a1a2e/00d9ff?text=CodeGuardian+%7C+Code+Better%2C+Learn+Faster)

</div>


# 🔒 Password Strength Checker

A beautiful, interactive web application that checks password strength in real-time using regex-based criteria. Built with pure HTML, CSS, and JavaScript - no dependencies required!

![Password Strength Checker](screenshot.png)

## ✨ Features

- 🎨 **Beautiful UI** - Modern gradient design with smooth animations
- ⚡ **Real-time Validation** - Instant feedback as you type
- 📊 **Visual Strength Meter** - Color-coded progress bar (Weak/Moderate/Strong)
- 👁️ **Password Toggle** - Show/hide password visibility
- ✅ **5 Security Criteria** - Comprehensive password requirements
- 💡 **Smart Suggestions** - Helpful tips to improve password strength
- 📱 **Responsive Design** - Works perfectly on mobile and desktop
- 🚀 **Zero Dependencies** - Pure vanilla JavaScript

## 🎯 Password Criteria

The checker validates passwords based on five essential criteria:

1. ✓ At least 8 characters long
2. ✓ Contains uppercase letter (A-Z)
3. ✓ Contains lowercase letter (a-z)
4. ✓ Contains number (0-9)
5. ✓ Contains special character (!@#$%^&*)

## 🚀 Demo

**Try these passwords to see different strength levels:**

- `password` → 🔴 Weak
- `Password123` → 🟡 Moderate  
- `P@ssw0rd123!` → 🟢 Strong

## 🖥️ Screenshots

### Weak Password
![Weak Password](screenshots/weak.png)

### Moderate Password
![Moderate Password](screenshots/moderate.png)

### Strong Password
![Strong Password](screenshots/strong.png)

## 🛠️ Technologies Used

- **HTML5** - Structure
- **CSS3** - Styling with gradients and animations
- **JavaScript (ES6)** - Logic and regex validation
- **Regular Expressions** - Pattern matching for validation

## 📦 Installation & Usage

### Method 1: Direct Download

1. Download or clone this repository:
```bash
git clone https://github.com/yourusername/password-strength-checker.git
```

2. Navigate to the project folder:
```bash
cd password-strength-checker
```

3. Open `index.html` in your browser:
   - Double-click the file, OR
   - Right-click → Open with → Your Browser

### Method 2: Live Server (Recommended for Development)

1. Install [VS Code](https://code.visualstudio.com/)
2. Install the "Live Server" extension
3. Right-click on `index.html` → Open with Live Server
4. Your browser will automatically open with live reload enabled

### Method 3: GitHub Pages

1. Fork this repository
2. Go to Settings → Pages
3. Select main branch as source
4. Your site will be live at: `https://yourusername.github.io/password-strength-checker/`

## 📁 Project Structure
```
password-strength-checker/
│
├── index.html          # Main HTML file (contains CSS and JS)
├── README.md           # Project documentation
├── LICENSE             # MIT License
├── screenshot.png      # Main screenshot
│
└── screenshots/        # Additional screenshots folder
    ├── weak.png
    ├── moderate.png
    └── strong.png
```

## 💻 Code Highlights

### Regex Patterns Used
```javascript
const uppercaseCheck = /[A-Z]/.test(password);        // Uppercase letters
const lowercaseCheck = /[a-z]/.test(password);        // Lowercase letters
const digitCheck = /\d/.test(password);                // Numbers
const specialCheck = /[!@#$%^&*()_+\-=\[\]{};:'",.<>?/\\|`~]/.test(password);
```

### Strength Calculation
```javascript
const score = [lengthCheck, uppercaseCheck, lowercaseCheck, digitCheck, specialCheck]
    .filter(Boolean).length;

// Score 5/5 = Strong
// Score 3-4/5 = Moderate  
// Score 0-2/5 = Weak
```

## 🎨 Customization

### Change Color Scheme

Edit the CSS variables in `index.html`:
```css
/* Background gradient */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Strength colors */
.weak { color: #ef4444; }      /* Red */
.moderate { color: #f59e0b; }  /* Orange */
.strong { color: #10b981; }    /* Green */
```

### Modify Password Criteria

Adjust the validation rules in the JavaScript section:
```javascript
const lengthCheck = password.length >= 12;  // Change minimum length
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

## 📝 Future Enhancements

- [ ] Password strength estimation (estimated crack time)
- [ ] Common password detection (check against leaked password database)
- [ ] Password generation feature
- [ ] Copy to clipboard functionality
- [ ] Dark mode toggle
- [ ] Multiple language support
- [ ] Password history (with local storage)
- [ ] Breach check integration (Have I Been Pwned API)

## 🐛 Known Issues

- None currently! Report issues [here](https://github.com/yourusername/password-strength-checker/issues)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)
- LinkedIn: [Your Name](https://linkedin.com/in/yourprofile)
- Email: your.email@example.com

## 🌟 Acknowledgments

- Design inspired by modern web applications
- Regular expressions documentation from MDN
- Icons: Unicode emoji characters

## 📊 Stats

![GitHub stars](https://img.shields.io/github/stars/yourusername/password-strength-checker?style=social)
![GitHub forks](https://img.shields.io/github/forks/yourusername/password-strength-checker?style=social)
![GitHub issues](https://img.shields.io/github/issues/yourusername/password-strength-checker)
![GitHub license](https://img.shields.io/github/license/yourusername/password-strength-checker)

---

⭐ **If you found this project helpful, please give it a star!** ⭐

Made with ❤️ and JavaScript
```

---

## 📸 HOW TO CREATE SCREENSHOTS

### **Step 1: Take Screenshots**

1. **Open your `index.html` in browser**

2. **For Main Screenshot (screenshot.png):**
   - Type a moderate password like `Password123`
   - Press **Windows Key + Shift + S** (Windows) or **Cmd + Shift + 4** (Mac)
   - Select the application area
   - Save as `screenshot.png`

3. **For Weak Password (screenshots/weak.png):**
   - Type `password`
   - Take screenshot
   - Save as `weak.png`

4. **For Moderate Password (screenshots/moderate.png):**
   - Type `Password123`
   - Take screenshot
   - Save as `moderate.png`

5. **For Strong Password (screenshots/strong.png):**
   - Type `P@ssw0rd123!`
   - Take screenshot
   - Save as `strong.png`

---

## 📁 FINAL PROJECT STRUCTURE

Create this folder structure before uploading:
```
password-strength-checker/
│
├── index.html
├── README.md
├── LICENSE
├── screenshot.png
│
└── screenshots/
    ├── weak.png
    ├── moderate.png
    └── strong.png
```

---

## 📜 LICENSE FILE

Create a file named `LICENSE` and paste this:
```
MIT License

Copyright (c) 2024 [Your Name]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

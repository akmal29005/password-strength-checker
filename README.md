# 🔒 Password Strength Checker

A modern, real-time password strength analyzer with beautiful UI and comprehensive security feedback. Built with vanilla HTML, CSS, and JavaScript - perfect for GitHub Pages hosting.

## ✨ Features

### Real-Time Analysis
- **Instant Feedback** - See password strength as you type
- **Visual Progress Bar** - Color-coded strength indicator (Very Weak to Strong)
- **Numerical Scoring** - Get a precise strength score out of 10
- **Show/Hide Toggle** - Securely view your password while typing

### Security Validation
- ✅ **Length Check** - Ensures minimum 8 characters (recommends 12+)
- ✅ **Character Diversity** - Validates uppercase, lowercase, numbers, and symbols
- ✅ **Pattern Detection** - Identifies and penalizes common weak patterns
- ✅ **Repetition Analysis** - Flags excessive character repetition
- ✅ **Dictionary Protection** - Detects common weak passwords

### Advanced Features
- 🕒 **Crack Time Estimation** - Shows how long it would take to crack your password
- 📱 **Mobile Responsive** - Works perfectly on all devices
- 🎨 **Modern Design** - Beautiful gradient UI with smooth animations
- 💡 **Security Tips** - Built-in best practices and recommendations

## 🚀 Live Demo

[View Live Demo](https://akmal29005.github.io/password-strength-checker/)

## 🛠️ Technologies Used

- **HTML5** - Semantic markup and accessibility
- **CSS3** - Modern styling with gradients and animations
- **Vanilla JavaScript** - No dependencies, lightweight and fast
- **Responsive Design** - Mobile-first approach

## 📦 Installation & Setup

### Download
1. Download the `index.html` file
2. Open it in any modern web browser
3. No installation required!

## 🧮 How It Works

The password strength is calculated using a sophisticated algorithm that considers:

### Scoring Factors
- **Character Length** (8+ chars required, 12+ recommended)
- **Character Types** (lowercase, uppercase, numbers, symbols)
- **Uniqueness** (penalizes repeated characters)
- **Pattern Detection** (identifies common weak patterns)
- **Diversity Bonus** (rewards using all character types)

### Strength Levels
- **Very Weak (0-2/10)** - 🔴 Easily crackable
- **Weak (3-4/10)** - 🟠 Vulnerable to attacks
- **Fair (5-6/10)** - 🟡 Moderate security
- **Good (7-8/10)** - 🟢 Strong protection
- **Strong (9-10/10)** - 🟢 Excellent security

### Crack Time Calculation
Estimates time to crack based on:
- Character set size (26-94 possible characters)
- Password length
- Brute force attack assumptions (1 billion guesses/second)

## 🎨 Customization

### Color Themes
Easily customize the color scheme by modifying the CSS variables:
```css
:root {
  --primary-gradient: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  --success-color: #4caf50;
  --warning-color: #ff9800;
  --danger-color: #ff4757;
}
```

### Strength Requirements
Modify the validation rules in the `calculateStrength()` function:
```javascript
const checks = {
  length: password.length >= 8,        // Minimum length
  lowercase: /[a-z]/.test(password),   // Lowercase letters
  uppercase: /[A-Z]/.test(password),   // Uppercase letters
  number: /\d/.test(password),         // Numbers
  special: /[special_chars]/.test(password), // Symbols
  unique: !hasRepeatedChars(password)  // No repetition
};
```

## 🔒 Security & Privacy

- **No Data Collection** - Passwords are never stored or transmitted
- **Client-Side Only** - All processing happens in your browser
- **No External Dependencies** - No third-party libraries or APIs
- **Open Source** - Full transparency of all security logic

## 🌟 Use Cases

- **Personal Use** - Check your own password strength
- **Educational** - Learn about password security
- **Development** - Integrate into registration forms
- **Security Training** - Demonstrate password best practices
- **Portfolio Project** - Showcase web development skills

## 📱 Browser Support

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository

### Ideas for Contributions
- Additional language support
- New password strength algorithms
- Dark/light theme toggle
- Password generation feature
- Accessibility improvements

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by modern password security research
- UI design influenced by contemporary web trends
- Security algorithms based on NIST guidelines

**Made with ❤️ by [Your Name]**

*If you found this project helpful, please give it a ⭐ star on GitHub!*

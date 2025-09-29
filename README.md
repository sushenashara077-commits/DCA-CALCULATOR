# 📊 DCA Position Calculator

A professional **Dollar Cost Averaging (DCA) Position Calculator** designed for crypto traders. Calculate optimal position adjustments with precision and style.

![DCA Calculator](https://img.shields.io/badge/Status-Active-brightgreen) ![Responsive](https://img.shields.io/badge/Design-Responsive-blue) ![Mobile](https://img.shields.io/badge/Mobile-Optimized-orange) ![Dark Mode](https://img.shields.io/badge/Theme-Dark%2FLight-purple)

## 🚀 Features

### 💹 **Core Functionality**
- **DCA Position Adjustment Calculations** - Calculate required volume for target average price
- **Long/Short Position Support** - Handles both buying and selling scenarios
- **Leverage Integration** - Built-in leverage calculations for margin requirements
- **Real-time Validation** - Input validation with helpful error messages
- **Professional Results Display** - Clean, organized output with visual indicators

### 🎨 **User Experience**
- **Dark/Light Mode Toggle** - Automatic theme persistence with localStorage
- **Responsive Design** - Optimized for mobile, tablet, and desktop
- **Mobile-First Approach** - Touch-friendly inputs with no auto-zoom
- **Smooth Animations** - CSS animations and transitions
- **Professional UI** - Crypto trading aesthetic with modern design

### 📱 **Mobile Optimization**
- **No Auto-Zoom** - Prevents unwanted zoom on input focus
- **Touch-Friendly Buttons** - 44px+ touch targets for optimal UX
- **Responsive Typography** - Scales perfectly across all screen sizes
- **Single-Column Mobile Layout** - Optimized flow for mobile devices
- **Condensed Labels** - Smart text truncation for small screens

## 🛠 **Technical Stack**

- **HTML5** - Semantic markup with accessibility features
- **CSS3** - Modern styling with CSS Grid, Flexbox, and CSS Custom Properties
- **Vanilla JavaScript** - Lightweight, no dependencies
- **Tailwind CSS** - Utility-first CSS framework via CDN
- **Google Fonts** - Inter font family for professional typography

## 📐 **Calculation Logic**

### **Long Position (Current Price < Target Price)**
```javascript
Required Volume = (Current Volume × (Target Price - Current Average Price)) / (Current Price - Target Price)
```

### **Short Position (Current Price ≥ Target Price)**
```javascript
Required Volume = (Current Volume × (Current Average Price - Target Price)) / (Target Price - Current Price)
```

### **Margin Calculation**
```javascript
Required Margin = (Required Volume × Current Price) / Leverage
```

## 🎯 **Input Fields**

| Field | Description | Required | Example |
|-------|-------------|----------|---------|
| **Volume** | Current contracts open | Optional | 12.5 |
| **Quota** | Total cost basis allocated | Optional | 12,500 |
| **Average Price** | Current weighted average | Optional | 102.35 |
| **Leverage** | Position multiplier | **Required** | 10 |
| **Current Price** | Current market price | **Required** | 98.25 |
| **Target Price** | Desired new average | **Required** | 95.00 |

## 📊 **Result Cards**

1. **Trade Direction** - Shows LONG/SHORT based on market conditions
2. **Required Volume** - Contracts needed to reach target average
3. **New Total Value** - Updated position value after adjustment
4. **Required Margin** - Margin needed for the adjustment

## 🎨 **Theme System**

### **Dark Mode (Default)**
- Background: Deep slate tones
- Accent: Yellow/Amber highlights
- Professional crypto trading aesthetic

### **Light Mode**
- Background: Clean whites and grays
- Accent: Consistent yellow/amber branding
- Optimized for daylight usage

## 📱 **Responsive Breakpoints**

```css
/* Mobile First */
@media (max-width: 640px)  /* Mobile phones */
@media (max-width: 480px)  /* Small mobile */

/* Tablet & Desktop */
sm: 640px   /* Small tablets */
md: 768px   /* Medium tablets */
lg: 1024px  /* Laptops */
xl: 1280px  /* Desktops */
```

## 🚀 **Getting Started**

### **1. Clone Repository**
```bash
git clone https://github.com/AsharaFernando18/DCA-CALCULATOR.git
cd DCA-CALCULATOR
```

### **2. Open in Browser**
```bash
# Option 1: Direct file opening
open index.html

# Option 2: Local server (recommended)
python3 -m http.server 8080
# Navigate to http://localhost:8080
```

### **3. Usage**
1. Enter your current position details (optional fields can be left empty)
2. Input **Leverage** (required)
3. Enter **Current Market Price** (required)
4. Set your **Target Average Price** (required)
5. Click **"Calculate Adjustment"**
6. Review the results and required actions

## 🔧 **Development**

### **File Structure**
```
DCA-CALCULATOR/
├── index.html          # Main application file
├── README.md          # Documentation
└── .git/              # Git repository
```

### **Key Features in Code**
- **Mobile Zoom Prevention**: `font-size: 16px` on inputs
- **Theme Persistence**: localStorage integration
- **Input Validation**: Comprehensive error handling
- **Responsive Design**: Mobile-first CSS approach
- **Accessibility**: ARIA labels and semantic HTML

## 🎯 **Use Cases**

### **Crypto Trading Scenarios**
- **DCA Strategy Adjustment** - Modify your average entry price
- **Position Sizing** - Calculate exact volumes needed
- **Risk Management** - Understand margin requirements
- **Portfolio Rebalancing** - Optimize position allocations

### **Trading Examples**
1. **Lower Your Average**: Currently at $100, want to average down to $95
2. **Increase Exposure**: Add volume while maintaining target average
3. **Leverage Optimization**: Calculate margin requirements for different leverage levels

## 📈 **Browser Support**

- ✅ **Chrome** 90+ (Recommended)
- ✅ **Firefox** 88+
- ✅ **Safari** 14+
- ✅ **Edge** 90+
- ✅ **Mobile Browsers** (iOS Safari, Chrome Mobile)

## 🤝 **Contributing**

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 **License**

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 **Author**

**AsharaFernando18**
- GitHub: [@AsharaFernando18](https://github.com/AsharaFernando18)
- Repository: [DCA-CALCULATOR](https://github.com/AsharaFernando18/DCA-CALCULATOR)

## 🙏 **Acknowledgments**

- **Tailwind CSS** - For the utility-first CSS framework
- **Google Fonts** - For the Inter font family
- **Modern CSS** - For Grid, Flexbox, and Custom Properties support

---

### 📊 **Try it Live**

Access the calculator directly by opening `index.html` in your browser or host it on any web server for public access.

**Perfect for crypto traders who need precise DCA calculations with a professional interface!** 🚀📈

---

*Built with ❤️ for the crypto trading community*
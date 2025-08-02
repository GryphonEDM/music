# GryphonEDM Website

Personal website with obfuscated code protection.

## 🛠️ Development Workflow

### **For Development (Clean Code):**
```bash
# Use the development version with readable code
npm run dev
# Then open: http://localhost:8000/index-dev.html
```

### **For Production (Obfuscated Code):**
```bash
# Build obfuscated files
npm run build

# Deploy to GitHub Pages
npm run deploy
```

## 📁 File Structure

### **Development Files (Clean & Readable):**
- `index-dev.html` - Development version with clean code
- `index.css` - Readable CSS
- `script.js` - Readable JavaScript
- `assets/` - Images and assets

### **Production Files (Obfuscated):**
- `dist/index-minified.css` - Minified CSS
- `dist/script-obfuscated.js` - Obfuscated JavaScript

### **GitHub Pages Deployment:**
- `index.html` - Auto-generated from index-dev.html with obfuscated references

## 🔄 Workflow

1. **Develop locally** using `index-dev.html` with clean, readable code
2. **Test changes** in development environment
3. **Build for production** with `npm run build` (creates obfuscated files)
4. **Deploy** with `npm run deploy` (pushes to GitHub Pages)

## 🛡️ Code Protection

The production build includes:
- ✅ JavaScript obfuscation (variable names, string encoding)
- ✅ CSS minification
- ✅ HTML minification
- ✅ Full functionality preserved

## 📝 Commands

```bash
npm run dev          # Start development server
npm run build        # Build obfuscated production files
npm run obfuscate    # Obfuscate JavaScript only
npm run minify       # Minify CSS only
npm run deploy       # Build and deploy to GitHub Pages
```

## 🔧 File Structure

```
├── index-dev.html      # 🛠️ Development (clean, readable)
├── index.html          # 🌐 GitHub Pages (auto-generated from dev)
├── index.css           # 📝 Clean CSS
├── script.js           # 🔧 Clean JavaScript
├── dist/               # 🛡️ Auto-generated obfuscated files
├── package.json        # ⚙️ Build scripts
└── README.md           # 📖 Documentation
```

**Note:** GitHub Pages serves `index.html` which is automatically generated from `index-dev.html` with obfuscated file references. 
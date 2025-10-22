# ☕ Third Cup Coffee Shop - React SPA

A modern Single Page Application (SPA) for Third Cup Coffee Shop built with React and React Router DOM.

## 🚀 Features

- **Single Page Application** - No page reloads, smooth navigation
- **5 Main Sections**: Home, About, Menu, Contact, Order
- **Interactive Menu** - Category switching, item selection
- **Order System** - Shopping cart functionality
- **Contact Form** - Multiple contact methods
- **Responsive Design** - Works on all devices
- **Modern UI** - Professional coffee shop design

## 🛠️ Technology Stack

- **React 18** - Frontend framework
- **React Router DOM** - Client-side routing
- **CSS3** - Styling with custom properties
- **HTML5** - Semantic markup

## 📦 Installation & Setup

1. **Install Dependencies**
   ```bash
   npm install
   ```

2. **Start Development Server**
   ```bash
   npm start
   ```

3. **Open in Browser**
   ```
   http://localhost:3000
   ```

## 🎨 Adding Real Images

To replace the current styled placeholders with real coffee and bread images:

### 1. Add Images to `public/images/`

Create these image files:
```
public/images/
├── coffee/
│   ├── espresso.jpg
│   ├── cappuccino.jpg
│   ├── latte.jpg
│   ├── mocha.jpg
│   └── ...
├── pastries/
│   ├── croissant.jpg
│   ├── banana-bread.jpg
│   ├── cinnamon-roll.jpg
│   └── baguette.jpg
└── hero/
    └── coffee-shop-hero.jpg
```

### 2. Update Components

Replace the current emoji-based images in:
- `src/pages/Home.js` - Popular items section
- `src/pages/Menu.js` - Menu items
- `src/pages/Order.js` - Order items

Example update:
```jsx
// Before
<div className="item-image coffee-image">
  <span className="item-emoji">☕</span>
</div>

// After
<div className="item-image">
  <img src="/images/coffee/latte.jpg" alt="Latte" />
</div>
```

### 3. Update CSS

Add image styling in `src/styles/index.css`:
```css
.item-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: var(--radius-md);
}
```

## 🏗️ Project Structure

```
src/
├── components/
│   ├── Header.js          # Navigation header
│   └── Footer.js          # Site footer
├── pages/
│   ├── Home.js           # Landing page
│   ├── About.js          # About us page
│   ├── Menu.js           # Menu with categories
│   ├── Contact.js        # Contact form & info
│   ├── Order.js          # Order system
│   └── NotFound.js       # 404 page
├── styles/
│   └── index.css         # All styling
├── App.js                # Main app component
└── index.js              # Entry point
```

## 🎯 Key Features

### Navigation
- **React Router DOM** for seamless page transitions
- **Active link highlighting** in header
- **404 page** for invalid routes

### Menu System
- **Category switching** (Coffee/Pastries)
- **Interactive items** with hover effects
- **Click to add** functionality

### Order System
- **Shopping cart** with quantity controls
- **Customer information** form
- **Order summary** with total calculation

### Contact Page
- **Multiple contact methods** (Call, Form, Social, FAQ)
- **Interactive sidebar** navigation
- **Contact form** with validation

## 🎨 Design Features

- **Coffee shop color palette** (browns, golds, creams)
- **Responsive grid layouts**
- **Smooth animations** and transitions
- **Professional typography** (Inter + Poppins)
- **Shadow effects** and depth
- **Mobile-first** responsive design

## 🚀 Deployment

Build for production:
```bash
npm run build
```

The build folder contains the production-ready files.

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is for educational purposes as part of a React SPA lab assignment.

---

**Third Cup Coffee Shop** - Where every cup tells a story! ☕
# Lucchese Product Page Recreation

A modern recreation of the Lucchese Priscilla Suede Espresso product page, implementing an interactive e-commerce experience with dynamic product variants, size selection, and responsive design.

🔗 **Original Page**: https://www.lucchese.com/products/priscilla-suede-espresso

## 🚀 Technologies Used

- **HTML5** - Semantic markup structure
- **TailwindCSS v4** - Utility-first CSS framework with custom design system
- **TypeScript** - Type-safe JavaScript development
- **Alpine.js** - Lightweight reactive framework for UI interactions
- **Vite** - Modern build tool and development server
- **Jest** - Testing framework
- **ESLint & Prettier** - Code linting and formatting

## ✨ Features Implemented

### Core Product Page Features
- **Product Variant Selection** - Interactive color/material variants with Alpine.js
- **Dynamic Size Selection** - Overlay modal for shoe size selection
- **Pricing Module** - Real-time price updates based on selected options
- **Image Gallery** - Dynamic product images that change with variants
- **Recommended Products** - Section showcasing related items
- **Add to Cart** - Interactive button with quantity selection
- **Responsive Design** - Mobile-first approach with breakpoint optimization

### Technical Features
- **REST API Integration** - Fetch product data from mock endpoints
- **TypeScript Interfaces** - Type-safe data structures
- **Custom Design System** - Tailwind variables for consistent branding
- **Accessibility** - ARIA labels, keyboard navigation, screen reader support
- **Performance Optimization** - Code splitting, lazy loading, optimized assets

## 🎨 Design System

The project uses a custom design system with the following variables:

```css
/* Colors */
--color-gray: rgb(77, 77, 77)
--color-light-gray: rgb(250, 250, 250)
--color-dark-blue: rgb(12, 39, 82)

/* Typography */
--font-size-l: 18px
--font-size-medium: 16px
--font-family-brandon: "Brandon Grotesque", sans-serif
--font-weight-brandon: 400
```

## 🛠 Installation & Setup

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/lucchese-product-page.git
   cd lucchese-product-page
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```

4. **Open in browser**
   ```
   http://localhost:3000
   ```

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run test` - Run tests
- `npm run test:watch` - Run tests in watch mode
- `npm run lint` - Run ESLint
- `npm run format` - Format code with Prettier
- `npm run mock-api` - Start mock API server (port 3001)

## 📁 Project Structure

```
├── public/
│   ├── images/          # Product images
│   └── icons/           # UI icons
├── src/
│   ├── api/             # API integration
│   ├── components/      # Reusable components
│   ├── styles/          # CSS and Tailwind config
│   ├── types/           # TypeScript interfaces
│   └── utils/           # Utility functions
├── mock/                # Mock API data
├── tests/               # Test files
├── templates/           # Template files
└── index.html           # Main HTML file
```

## 🔧 Key Implementation Details

### Alpine.js Store
The product page uses Alpine.js reactive store pattern for state management:

```javascript
// Product state management
x-data="productStore()"
```

### TailwindCSS v4 Configuration
Custom theme configuration using CSS-first approach:

```css
@theme {
  --color-gray: rgb(77, 77, 77);
  --font-family-brandon: "Brandon Grotesque", sans-serif;
}
```

### TypeScript Interfaces
Type-safe data structures for products:

```typescript
interface Product {
  id: string;
  name: string;
  variants: ProductVariant[];
  sizes: ProductSize[];
  // ... more properties
}
```

## 🎯 Features Deep Dive

### Product Variants
- Color/material selection with visual swatches
- Dynamic price updates
- Image gallery changes based on selection
- Inventory tracking per variant

### Size Selection Overlay
- Modal overlay for size selection
- Size availability indication
- Size guide information
- Responsive grid layout

### Pricing Module
- Base price display
- Sale price handling
- Currency formatting
- Price updates with variant changes

### Image Gallery
- High-quality product images
- Thumbnail navigation
- Zoom functionality
- Responsive image loading

## 🧪 Testing

Run the test suite:

```bash
npm run test
```

Tests cover:
- Component functionality
- API integration
- User interactions
- Responsive behavior

## 🚀 Deployment

Build for production:

```bash
npm run build
```

The built files will be in the `dist/` directory.

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 🔄 Future Enhancements

- [ ] User authentication
- [ ] Shopping cart persistence
- [ ] Product reviews system
- [ ] Wishlist functionality
- [ ] Search and filtering
- [ ] Multi-language support

## 📄 License

This project is licensed under the MIT License.

## 👥 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📞 Support

For questions or issues, please create an issue in the GitHub repository.

---

**Note**: This is a recreation project for educational/demonstration purposes. All product images and content belong to their respective owners.
# PrintForge 🖨️

A Next.js platform for discovering and sharing 3D printing models, built with React, TypeScript, and Tailwind CSS.

[![Next.js](https://img.shields.io/badge/Next.js-15.2.4-black?style=flat&logo=next.js)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19.0.0-blue?style=flat&logo=react)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-blue?style=flat&logo=typescript)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.4.17-38bdf8?style=flat&logo=tailwind-css)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)

## 📋 Table of Contents

- [About](#about)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Running the Application](#running-the-application)
- [Project Structure](#project-structure)
- [Configuration](#configuration)
- [Available Scripts](#available-scripts)
- [Contributing](#contributing)
- [License](#license)

## 🎯 About

PrintForge is a community-driven platform where 3D printing enthusiasts, makers, and designers can discover, browse, and explore a vast library of 3D models. The platform features an intuitive interface with category-based navigation, search functionality, and detailed model information pages.

## ✨ Features

- **📚 Extensive Model Library**: Browse through 50+ curated 3D printing models
- **🗂️ Category Navigation**: Organized into 10 distinct categories including:
  - 3D Printer Parts & Upgrades
  - Art & Decorations
  - Educational Models
  - Fashion & Accessories
  - Tools & Utilities
  - And more...
- **🔍 Search Functionality**: Quickly find models by name or description
- **📱 Responsive Design**: Fully optimized for desktop, tablet, and mobile devices
- **♥️ Like System**: Track popular models with community engagement metrics
- **🎨 Modern UI**: Clean, professional interface built with Tailwind CSS
- **⚡ Performance**: Built on Next.js 15 with optimized rendering and routing

## 🛠️ Tech Stack

- **Framework**: [Next.js 15.2.4](https://nextjs.org/) (App Router)
- **Language**: [TypeScript 5.x](https://www.typescriptlang.org/)
- **UI Library**: [React 19.0.0](https://react.dev/)
- **Styling**: [Tailwind CSS 3.4.17](https://tailwindcss.com/)
- **Icons**: [React Icons 5.5.0](https://react-icons.github.io/react-icons/)
- **Fonts**: Google Fonts (Albert Sans, Montserrat Alternates)
- **Linting**: ESLint with Next.js configuration

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js**: Version 20.x or higher
- **npm**: Version 10.x or higher (comes with Node.js)

### Installation

1. Clone the repository:

```bash
git clone https://github.com/bakadja/print-forge.git
cd print-forge
```

2. Install dependencies:

```bash
npm install
```

### Running the Application

#### Development Mode

Start the development server with hot-reload:

```bash
npm run dev
```

The application will be available at [http://localhost:3000](http://localhost:3000)

#### Production Build

Build the application for production:

```bash
npm run build
```

Start the production server:

```bash
npm start
```

## 📁 Project Structure

```
print-forge/
├── app/
│   ├── components/         # Reusable React components
│   │   ├── CategoriesNav.tsx
│   │   ├── ModelCard.tsx
│   │   ├── ModelsGrid.tsx
│   │   ├── Navbar.tsx
│   │   ├── NavLink.tsx
│   │   └── Pill.tsx
│   ├── data/              # JSON data files
│   │   ├── categories.json
│   │   └── models.json
│   ├── lib/               # Utility functions
│   │   ├── categories.ts
│   │   └── models.ts
│   ├── types/             # TypeScript type definitions
│   │   └── index.ts
│   ├── 3d-models/         # Models pages
│   │   ├── [id]/          # Dynamic model detail page
│   │   ├── categories/    # Category pages
│   │   ├── layout.tsx
│   │   └── page.tsx
│   ├── about/             # About page
│   ├── globals.css        # Global styles
│   ├── layout.tsx         # Root layout
│   └── page.tsx           # Home page
├── public/                # Static assets
├── eslint.config.mjs      # ESLint configuration
├── next.config.ts         # Next.js configuration
├── package.json           # Dependencies and scripts
├── postcss.config.mjs     # PostCSS configuration
├── tailwind.config.js     # Tailwind CSS configuration
└── tsconfig.json          # TypeScript configuration
```

## ⚙️ Configuration

### Environment Variables

Currently, the project runs with mock data and doesn't require environment variables. For future database integration, create a `.env.local` file:

```env
# Database (example for future implementation)
DATABASE_URL="your-database-url"

# API Keys (if needed)
API_KEY="your-api-key"
```

### Tailwind Configuration

Custom colors and theme extensions can be modified in `tailwind.config.js`:

```javascript
theme: {
  extend: {
    colors: {
      "orange-accent": "#F77D36"
    }
  }
}
```

### TypeScript Configuration

Strict mode is enabled. Adjust compiler options in `tsconfig.json` as needed.

## 📜 Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm start` | Start production server |
| `npm run lint` | Run ESLint to check code quality |

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Code Style

- Follow the existing code style
- Use TypeScript for all new files
- Ensure all ESLint rules pass
- Write meaningful commit messages

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

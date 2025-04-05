# Infinite Animation Gallery

[![React Version](https://img.shields.io/badge/react-18.2.0-blue.svg)](https://reactjs.org/)
[![Redux](https://img.shields.io/badge/redux-4.2.1-purple.svg)](https://redux.js.org/)
[![Three.js](https://img.shields.io/badge/three.js-0.152.0-green.svg)](https://threejs.org/)
[![TypeScript](https://img.shields.io/badge/typescript-5.0.4-blue.svg)](https://www.typescriptlang.org/)
[![License](https://img.shields.io/badge/license-MIT-yellow.svg)](LICENSE)

## Overview

Infinite Animation Gallery is a cutting-edge web application that showcases an extensive collection of animations through a seamless infinite scrolling experience. The project combines modern web technologies to deliver high-performance 3D and 2D animations in an intuitive and responsive interface.

## Features

- **Infinite Scroll**: Seamless content loading as the user scrolls through the gallery
- **3D Animations**: Integration with Three.js for immersive 3D animation experiences
- **Responsive Design**: Optimized for all device sizes from mobile to desktop
- **Animation Filtering**: Advanced filtering system to discover animations by style, technique, and complexity
- **Performance Optimized**: Virtualized list rendering and asset lazy-loading
- **User Accounts**: Save favorite animations and create custom collections
- **Animation Details**: Comprehensive information about techniques used in each animation
- **Dark/Light Mode**: Customizable viewing experience

## Technologies

- **Frontend**:
  - React 18
  - Redux for state management
  - TypeScript for type safety
  - Three.js for 3D rendering
  - Framer Motion for UI animations
  - Tailwind CSS for styling
  - React Query for data fetching

- **Backend**:
  - Node.js with Express
  - MongoDB for database
  - GraphQL API
  - JWT authentication

- **Deployment**:
  - Docker containerization
  - CI/CD pipeline with GitHub Actions
  - AWS hosting infrastructure

## Getting Started

### Prerequisites

- Node.js (v16+)
- npm or yarn
- MongoDB (local or Atlas)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/username/infinite-animation-gallery.git
   cd infinite-animation-gallery
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file based on `.env.example` and fill in your environment variables.

4. Start the development server:
   ```bash
   npm run dev
   ```

5. Open your browser and navigate to `http://localhost:3000`

## Project Structure

```
infinite-animation-gallery/
├── public/            # Static assets
├── src/
│   ├── animations/    # Animation components and hooks
│   ├── api/           # API endpoints and services
│   ├── components/    # Reusable UI components
│   ├── hooks/         # Custom React hooks
│   ├── pages/         # Page components
│   ├── store/         # Redux store configuration
│   ├── styles/        # Global styles and theme configuration
│   ├── types/         # TypeScript type definitions
│   ├── utils/         # Utility functions
│   ├── App.tsx        # Main application component
│   └── index.tsx      # Application entry point
├── server/            # Backend code
├── .env.example       # Example environment variables
├── package.json       # Dependencies and scripts
├── tsconfig.json      # TypeScript configuration
└── README.md          # Project documentation
```

## Key Concepts

### Animation Engine

The core of the application is built around a custom animation engine that handles both 2D canvas animations and 3D scenes rendered with Three.js. The engine optimizes performance by:

- Implementing WebGL acceleration
- Using requestAnimationFrame for smooth animation
- Dynamically adjusting detail levels based on device capabilities
- Employing workers for complex calculations

### Infinite Scroll Implementation

The infinite scroll is implemented using:

- Virtualized lists to render only visible items
- Prefetching content as users approach the end of current items
- Caching previously viewed animations
- Smooth scrolling between animation transitions

### State Management

Redux is used to manage global state, with a structure that separates:

- User interface state
- Animation collection data
- Filter and search parameters
- User preferences and saved items

## Contributing

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/amazing-feature`
3. Commit your changes: `git commit -m 'Add some amazing feature'`
4. Push to the branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Developer

**João Vitor Belasque**
- Email: joaovitorpilot@outlook.com
- LinkedIn: [https://www.linkedin.com/in/joaovitorfullstack/](https://www.linkedin.com/in/joaovitorfullstack/)

## Acknowledgements

- [React](https://reactjs.org/) - UI library
- [Three.js](https://threejs.org/) - 3D library
- [Redux](https://redux.js.org/) - State management
- [Framer Motion](https://www.framer.com/motion/) - Animation library
- [Tailwind CSS](https://tailwindcss.com/) - CSS framework

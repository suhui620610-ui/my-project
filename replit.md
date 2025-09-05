# Overview

This is a modern full-stack web application built with React, TypeScript, and Express.js. The project appears to be a personal portfolio/resume website for "林柔均" (Lin Rou Jun), showcasing marketing and planning skills. The application features a comprehensive UI component library using shadcn/ui, responsive design with Tailwind CSS, smooth animations with Framer Motion, and interactive data visualizations with Chart.js.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Framework**: React 18 with TypeScript in a Single Page Application (SPA) architecture
- **Routing**: Wouter for lightweight client-side routing
- **Styling**: Tailwind CSS with custom CSS variables for theming, providing a consistent design system
- **UI Components**: shadcn/ui component library built on Radix UI primitives for accessibility and consistency
- **Animations**: Framer Motion for smooth page transitions and interactive animations
- **Data Visualization**: Chart.js for rendering interactive charts and graphs
- **State Management**: TanStack React Query for server state management and data fetching
- **Build Tool**: Vite for fast development and optimized production builds

## Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules
- **Development Server**: Custom Vite integration for development with HMR support
- **Middleware**: Custom logging middleware for API request tracking
- **Storage Interface**: Abstract storage interface with in-memory implementation for user management
- **Static Files**: Vite serves static files in development, built files served in production

## Database Architecture
- **ORM**: Drizzle ORM with PostgreSQL dialect for type-safe database operations
- **Database**: PostgreSQL (configured but not actively used in current implementation)
- **Migration System**: Drizzle Kit for database schema migrations
- **Connection**: Neon Database serverless driver for PostgreSQL connections
- **Schema**: User table with UUID primary keys and unique username constraints

## Project Structure
- **Monorepo Layout**: Client, server, and shared code in separate directories
- **Shared Types**: Common TypeScript types and schemas in `/shared` directory
- **Asset Management**: Static assets stored in `/attached_assets` with Vite alias configuration
- **Configuration**: Centralized configuration files for TypeScript, Tailwind, and build tools

## Development Features
- **Hot Module Replacement**: Vite HMR for instant development feedback
- **Error Handling**: Runtime error overlay for development debugging
- **Code Quality**: TypeScript strict mode with comprehensive type checking
- **Path Aliases**: Configured path mapping for clean imports (@/, @shared/, @assets/)

# External Dependencies

## Core Framework Dependencies
- **@neondatabase/serverless**: PostgreSQL serverless driver for database connections
- **drizzle-orm & drizzle-zod**: Type-safe ORM with Zod schema validation
- **@tanstack/react-query**: Server state management and data fetching library
- **wouter**: Lightweight routing library for React applications

## UI and Styling Dependencies
- **@radix-ui/***: Comprehensive set of accessible UI primitives for building components
- **tailwindcss**: Utility-first CSS framework for responsive design
- **framer-motion**: Animation library for React components
- **class-variance-authority & clsx**: Utility libraries for conditional CSS class management
- **lucide-react**: Modern icon library with React components

## Development and Build Dependencies
- **vite**: Fast build tool and development server
- **@vitejs/plugin-react**: React support for Vite
- **tsx**: TypeScript execution environment for Node.js
- **esbuild**: JavaScript bundler for production builds

## Data Visualization
- **chart.js**: Flexible charting library for interactive data visualization
- **react-chartjs-2**: React wrapper for Chart.js (likely used but not explicitly listed)

## Additional Utilities
- **date-fns**: Modern date utility library for JavaScript
- **zod**: TypeScript-first schema validation library
- **nanoid**: URL-safe unique string ID generator
- **connect-pg-simple**: PostgreSQL session store for Express.js (prepared for future session management)
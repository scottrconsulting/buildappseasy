# BuildAppsEasy - TikTok-Driven App Development Platform

## Overview

BuildAppsEasy is a modern full-stack web application that serves as a TikTok-driven app development platform. The application showcases app development services, integrates with TikTok content, and provides lead generation capabilities for potential clients. It's built as a marketing and lead capture platform for a developer who builds apps live on TikTok.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Routing**: Wouter for client-side routing
- **Styling**: Tailwind CSS with custom design system
- **UI Components**: Radix UI primitives with shadcn/ui component library
- **State Management**: React Query (TanStack Query) for server state
- **Form Handling**: React Hook Form with Zod validation
- **Build Tool**: Vite for fast development and optimized builds

### Backend Architecture
- **Runtime**: Node.js with Express.js
- **Language**: TypeScript with ES modules
- **API Design**: RESTful API endpoints
- **Validation**: Zod schemas for type-safe data validation
- **Database**: PostgreSQL with Drizzle ORM
- **Session Management**: Express sessions with PostgreSQL store

### Development Setup
- **Full-stack Development**: Single repository with client/server separation
- **Development Server**: Vite dev server with Express backend proxy
- **Hot Module Replacement**: Enabled for fast development cycles
- **TypeScript**: Strict configuration with path mapping

## Key Components

### Database Schema (PostgreSQL + Drizzle)
- **Users Table**: Authentication and user management
- **Leads Table**: Contact form submissions for quotes/services
- **Consultations Table**: Consultation booking requests
- **Schema Validation**: Drizzle-Zod integration for type-safe database operations

### API Endpoints
- `POST /api/leads` - Create new lead from contact form
- `GET /api/leads` - Retrieve all leads (admin functionality)
- `POST /api/consultations` - Book consultation appointments
- `GET /api/consultations` - Retrieve consultation bookings

### Frontend Features
- **Responsive Design**: Mobile-first approach with Tailwind CSS
- **Interactive Sections**: Hero, Services, Portfolio, TikTok content, Contact
- **Form Handling**: Quote requests and consultation bookings
- **Toast Notifications**: User feedback for form submissions
- **Smooth Scrolling**: Navigation between page sections

### UI/UX Design System
- **Color Palette**: Electric purple, hot pink, electric blue, bright green
- **Typography**: Modern, clean font hierarchy
- **Components**: Comprehensive shadcn/ui component library
- **Animations**: Smooth transitions and hover effects
- **Accessibility**: ARIA-compliant components from Radix UI

## Data Flow

1. **User Interaction**: Users navigate the landing page and interact with forms
2. **Form Submission**: Contact forms validate data using Zod schemas
3. **API Processing**: Express endpoints handle form submissions
4. **Database Storage**: Drizzle ORM persists data to PostgreSQL
5. **Response Handling**: React Query manages API responses and UI updates
6. **User Feedback**: Toast notifications confirm successful submissions

## External Dependencies

### Core Technologies
- **React Ecosystem**: React, React DOM, React Hook Form
- **Styling**: Tailwind CSS, Radix UI, class-variance-authority
- **Backend**: Express.js, Drizzle ORM, Zod validation
- **Database**: PostgreSQL via Neon Database (@neondatabase/serverless)
- **Development**: Vite, TypeScript, ESBuild

### UI Component Libraries
- **Radix UI**: Comprehensive set of accessible UI primitives
- **shadcn/ui**: Pre-built component system based on Radix UI
- **Lucide React**: Icon library for consistent iconography

### Development Tools
- **Type Safety**: TypeScript with strict configuration
- **Code Quality**: ESLint, Prettier (implied by project structure)
- **Build Optimization**: Vite for development, ESBuild for production

## Deployment Strategy

### Build Process
- **Frontend**: Vite builds optimized React bundle to `dist/public`
- **Backend**: ESBuild compiles TypeScript server to `dist/index.js`
- **Static Assets**: Served from Express in production

### Environment Configuration
- **Development**: `npm run dev` - runs both frontend and backend concurrently
- **Production**: `npm run build` && `npm start` - builds and serves optimized app
- **Database**: Requires `DATABASE_URL` environment variable for PostgreSQL connection

### Replit Integration
- **Auto-deployment**: Configured for Replit autoscale deployment
- **Port Configuration**: Runs on port 5000 internally, exposed on port 80
- **Module Dependencies**: nodejs-20, web, postgresql-16

## Changelog

```
Changelog:
- June 23, 2025. Initial setup
```

## User Preferences

```
Preferred communication style: Simple, everyday language.
```
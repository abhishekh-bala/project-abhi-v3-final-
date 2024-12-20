GoDaddy Contest Dashboard Documentation
=======================================

Project Overview
---------------
A React-based web application for managing GoDaddy's guide contest and prize drawings. The application features two main dashboards: Contest Dashboard for live prize drawings and Admin Dashboard for guide management.

Tech Stack
----------
1. Frontend Framework:
   - React 18.3.1 with TypeScript
   - Vite 5.4.2 for build tooling
   - TypeScript 5.5.3 for type safety

2. UI/Styling:
   - Tailwind CSS 3.4.1 for styling
   - Framer Motion for animations
   - Lucide React for icons
   - React Confetti for celebration effects
   - React Hot Toast for notifications

3. Development Tools:
   - ESLint for code linting
   - PostCSS and Autoprefixer for CSS processing
   - Custom ESLint configuration for React and TypeScript

Project Structure
----------------
1. Core Components:
   - App.tsx: Main application component
   - Navigation.tsx: Tab-based navigation
   - ContestDashboard.tsx: Prize drawing interface
   - AdminDashboard.tsx: Guide management interface

2. Feature Components:
   - WinnerModal.tsx: Displays winner information
   - CountdownOverlay.tsx: Animated countdown
   - TicketReveal.tsx: Ticket number animation
   - LoadingSpinner.tsx: Loading states
   - PageLoader.tsx: Page transition loader

3. Utility Components:
   - Logo.tsx: GoDaddy logo display
   - TicketNumber.tsx: Ticket display
   - VehicleImage.tsx: Prize vehicle images
   - WinnerCard.tsx: Winner information card

4. Custom Hooks:
   - useCountdown.ts: Countdown timer logic

5. Types and Utilities:
   - types/index.ts: TypeScript interfaces
   - utils/fetchData.ts: Data fetching logic

Key Features
-----------
1. Contest Dashboard:
   - Live prize drawing system
   - Animated winner selection
   - Confetti celebration effects
   - Prize-specific animations
   - Ticket number reveal sequence

2. Admin Dashboard:
   - Guide information display
   - Ticket allocation tracking
   - Search functionality
   - Pagination system
   - Real-time filtering

3. Shared Features:
   - Responsive design
   - Smooth animations
   - Error handling
   - Loading states
   - Toast notifications

Data Structure
-------------
1. Guide Interface:
   {
     jomax_id: string;
     name: string;
     tickets: number[];
   }

2. Winner Interface:
   {
     guide: Guide;
     ticket: number;
     prize: 'Pulsar Bike' | 'Jupiter Scooty';
   }

User Workflow
------------
1. Contest Flow:
   - Access Contest Dashboard
   - Click "Reveal Winner" button
   - Watch countdown animation
   - View ticket reveal sequence
   - See winner celebration
   - Confirm and continue

2. Admin Flow:
   - Access Admin Dashboard
   - View all guides and tickets
   - Search/filter guides
   - Monitor ticket distribution
   - Track winner selection

Animation System
--------------
1. Framer Motion Animations:
   - Page transitions
   - Component mounting
   - Winner reveals
   - Countdown sequence
   - Hover effects

2. CSS Animations:
   - Gradient backgrounds
   - Loading spinners
   - Shimmer effects
   - Text gradients

Styling Architecture
------------------
1. Tailwind CSS:
   - Custom color scheme
   - Responsive design
   - Custom gradients
   - Animation utilities

2. Custom CSS:
   - Gradient animations
   - Font configurations
   - Custom keyframes
   - Utility classes

Error Handling
-------------
1. Data Fetching:
   - Try-catch blocks
   - Error state management
   - Toast notifications
   - Fallback UI

2. User Interactions:
   - Input validation
   - State verification
   - Loading indicators
   - Error boundaries

Performance Optimizations
-----------------------
1. Code Splitting:
   - Component-level splitting
   - Dynamic imports
   - Lazy loading
   - Bundle optimization

2. State Management:
   - Local state usage
   - Custom hooks
   - Memoization
   - Effect cleanup

Development Guidelines
--------------------
1. Component Creation:
   - Single responsibility
   - TypeScript interfaces
   - Proper prop types
   - JSDoc documentation

2. Code Style:
   - ESLint rules
   - Consistent formatting
   - Clear naming
   - Type safety

3. Testing:
   - Component testing
   - Hook testing
   - Integration tests
   - Error scenarios

Deployment
---------
1. Build Process:
   - Vite production build
   - Asset optimization
   - Environment variables
   - Performance checks

2. Requirements:
   - Node.js 18+
   - npm/yarn
   - Modern browser
   - Internet connection

This documentation provides a comprehensive overview of the GoDaddy Contest Dashboard, covering its architecture, features, and implementation details.

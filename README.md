# GoodMe LMS

> **LBYE** - Learn Before You Earn

A modern Learning Management System (LMS) platform built with Next.js, enabling teachers to create and manage courses, and students to enroll, learn, and track their progress.

## 🌐 Live Demo

**Live Site:** [https://lms-poc-eta.vercel.app](https://lms-poc-eta.vercel.app)

## ✨ Features

### For Students
- 📚 Browse and discover courses
- 🎓 Enroll in courses
- 📹 Watch course videos
- 📊 Track learning progress
- 📱 Responsive design for mobile and desktop
- 🌓 Dark/Light theme support

### For Teachers
- ➕ Create and manage courses
- 📝 Add course content (videos, images)
- 👥 View enrolled students
- 📈 Monitor course performance
- 🎨 Rich course editing interface

### General Features
- 🔐 Secure authentication with NextAuth
- 👤 Role-based access control (Teacher/Student)
- 🎨 Modern UI with Material-UI
- 📱 Fully responsive design
- 🌓 Theme switching (Dark/Light mode)
- 🔒 Protected routes with middleware
- 📤 File uploads with ImageKit integration
- ⚡ Server-side rendering with Next.js App Router

## 🛠️ Tech Stack

- **Framework:** [Next.js 15](https://nextjs.org/) (App Router)
- **Language:** [TypeScript](https://www.typescriptlang.org/)
- **UI Library:** [Material-UI (MUI)](https://mui.com/)
- **Authentication:** [NextAuth.js](https://next-auth.js.org/)
- **Form Handling:** [React Hook Form](https://react-hook-form.com/) + [Yup](https://github.com/jquense/yup)
- **Styling:** [Emotion](https://emotion.sh/) (CSS-in-JS)
- **Media Storage:** [ImageKit](https://imagekit.io/)
- **Font:** [Geist](https://vercel.com/font)

## 📋 Prerequisites

- Node.js 18+ 
- npm, yarn, pnpm, or bun
- Environment variables configured (see below)

## 🚀 Getting Started

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/goodme-lms.git
cd goodme-lms
```

2. Install dependencies:
```bash
npm install
# or
yarn install
# or
pnpm install
# or
bun install
```

### Environment Variables

Create a `.env.local` file in the root directory with the following variables:

```env
# NextAuth Configuration
CLERK_SECRET_KEY=your-secret-key-here

# API Configuration
NEXT_PUBLIC_API_URL=http://localhost:3000

# ImageKit Configuration (if using ImageKit for file uploads)
IMAGEKIT_PUBLIC_KEY=your-imagekit-public-key
IMAGEKIT_PRIVATE_KEY=your-imagekit-private-key
IMAGEKIT_URL_ENDPOINT=your-imagekit-url-endpoint
```

### Running the Development Server

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the application.

## 📁 Project Structure

```
src/
├── app/                    # Next.js App Router pages
│   ├── (public)/          # Public routes (home, course preview, auth)
│   ├── (protected)/       # Protected routes (dashboard, courses)
│   │   └── (teacher)/    # Teacher-specific routes
│   └── api/               # API routes
├── components/            # React components
│   ├── atom/             # Atomic components (Switch)
│   ├── molecule/         # Molecular components (Cards, Drawer, Video Player)
│   └── organism/         # Complex components (Forms, Layout, Top Bar)
├── libs/                 # Utilities and services
│   ├── services/         # API service functions
│   ├── session/          # Session management
│   ├── types/            # TypeScript type definitions
│   ├── utils/            # Helper functions
│   └── validations/      # Form validation schemas
├── hooks/                # Custom React hooks
├── constants/            # Application constants
├── context/              # React context providers
└── theme/                # Theme configuration
```

## 🔐 Authentication & Authorization

The application uses NextAuth.js for authentication with:
- JWT-based sessions
- Credentials provider
- Role-based access control (Teacher/Student)
- Protected route middleware
- Automatic redirects for authenticated/unauthenticated users

## 🎨 Theming

The application supports both dark and light themes:
- Theme preference is stored in localStorage
- Toggle available in the top navigation bar
- Material-UI theme system with custom configurations

## 📦 Building for Production

```bash
npm run build
npm start
```

## 🚢 Deployment

The easiest way to deploy this Next.js application is using [Vercel](https://vercel.com):

1. Push your code to GitHub
2. Import your repository in Vercel
3. Configure environment variables
4. Deploy!

For more details, see the [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying).

## 📝 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm start` - Start production server
- `npm run lint` - Run ESLint

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is private and proprietary.

## 👥 Authors

- Abhijeet Kumar Gupta



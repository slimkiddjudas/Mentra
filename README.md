# Mentra: Real-time AI Teaching Platform

![Mentra Logo](/public/images/logo.svg)

## 📚 Overview

Mentra is an advanced SaaS platform that revolutionizes personalized learning through AI-powered companions. Build custom learning companions tailored to specific subjects, teaching styles, and personalities for an interactive educational experience through natural voice conversations.

## ✨ Features

- **Custom Learning Companions**: Create personalized teaching companions for various subjects including Mathematics, Science, Coding, Language, History, and Economics.
- **Voice-Enabled Conversations**: Engage in natural voice conversations with AI companions using cutting-edge voice recognition and synthesis.
- **Customizable Teaching Styles**: Choose between casual or formal teaching approaches to match your learning preferences.
- **Session Tracking**: Monitor your learning journey with detailed tracking of completed lessons and created companions.
- **Bookmark System**: Save and organize your favorite companions for quick access.
- **Responsive Design**: Fully optimized experience across desktop and mobile devices.

## 🛠️ Tech Stack

- **Frontend**: Next.js 15, React 19, TailwindCSS 4
- **Authentication**: Clerk
- **Database**: Supabase
- **Voice AI**: VAPI.ai
- **Error Monitoring**: Sentry
- **UI Components**: Radix UI
- **Styling**: TailwindCSS with custom animations (tw-animate-css)
- **Form Handling**: React Hook Form with Zod validation

## 🚀 Getting Started

### Prerequisites

- Node.js 18.0 or later
- npm, yarn, pnpm, or bun

### Environment Variables

Create a `.env.local` file in the root directory with the following variables:

```env
# Clerk Authentication
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

# Supabase
NEXT_PUBLIC_SUPABASE_URL=
NEXT_PUBLIC_SUPABASE_ANON_KEY=

# VAPI.ai
NEXT_PUBLIC_VAPI_API_KEY=

# Sentry
NEXT_PUBLIC_SENTRY_DSN=
```

### Installation

```bash
# Clone the repository
git clone https://github.com/slimkiddjudas/Mentra.git
cd mentra

# Install dependencies
npm install
# or
yarn install
# or
pnpm install
# or
bun install

# Start development server
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the application.

## 📖 Project Structure

```
├── app/                 # Next.js App Router
│   ├── api/             # API Routes
│   ├── companions/      # Companion creation & management
│   ├── my-journey/      # User learning history
│   ├── sign-in/         # Authentication
│   └── subscription/    # Subscription management
├── components/          # React components
│   └── ui/              # UI component library
├── constants/           # Application constants
├── lib/                 # Utility functions & services
│   ├── actions/         # Server actions
│   ├── supabase.ts      # Supabase client
│   └── vapi.sdk.ts      # VAPI integration
├── public/              # Static assets
└── types/               # TypeScript type definitions
```

## 🔒 Authentication

Mentra uses Clerk for authentication, providing:

- Email/password login
- Google OAuth
- User profile management
- Session handling

## 💾 Database Schema

The application uses Supabase with the following main tables:

- `companions`: Stores companion configurations
- `users`: User information linked with Clerk authentication
- `sessions`: Records of learning sessions

## 🎯 Roadmap

- [ ] Enhanced analytics dashboard
- [ ] Collaborative learning sessions
- [ ] Mobile application
- [ ] Offline mode support
- [ ] Integration with educational content providers

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👥 Contributors

- [Your Name](https://github.com/yourusername) - Lead Developer
- [Contributor Name](https://github.com/username) - Frontend Developer
- [Contributor Name](https://github.com/username) - Backend Developer

## 🙏 Acknowledgements

- [Next.js](https://nextjs.org) - The React Framework
- [Supabase](https://supabase.io) - Open Source Firebase Alternative
- [Clerk](https://clerk.dev) - Authentication & User Management
- [VAPI.ai](https://vapi.ai) - Voice AI Platform
- [Sentry](https://sentry.io) - Error Monitoring

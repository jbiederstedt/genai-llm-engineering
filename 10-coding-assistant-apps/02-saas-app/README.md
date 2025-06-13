# SaaS Application

A full-stack SaaS application built with Next.js, TypeScript, and Drizzle ORM. This application features a UI using Tailwind CSS and Radix UI components, with secure authentication and database integration.

## 🚀 Features

- ⚡️ Next.js 15 with App Router
- 🔒 Authentication and Authorization
- 💾 PostgreSQL Database with Drizzle ORM
- 🎨 Modern UI with Tailwind CSS and Radix UI
- 💳 Stripe Integration for Payments
- 🔐 Secure Password Hashing with bcrypt
- 📱 Responsive Design
- 🎯 TypeScript for Type Safety

## 🛠️ Tech Stack

- **Framework:** Next.js 15
- **Language:** TypeScript
- **Styling:** Tailwind CSS
- **UI Components:** Radix UI
- **Database:** PostgreSQL
- **ORM:** Drizzle
- **Authentication:** Custom JWT-based auth
- **Payment Processing:** Stripe
- **Package Manager:** pnpm

## 📦 Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   pnpm install
   ```
3. Copy the environment variables:
   ```bash
   cp .env.example .env
   ```
4. Set up your environment variables in `.env`

## 🗄️ Database Setup

1. Set up the database:
   ```bash
   pnpm db:setup
   ```
2. Run migrations:
   ```bash
   pnpm db:migrate
   ```
3. (Optional) Seed the database:
   ```bash
   pnpm db:seed
   ```

## 🚀 Development

Start the development server:

```bash
pnpm dev
```

The application will be available at `http://localhost:3000`.

## 📝 Available Scripts

- `pnpm dev` - Start development server
- `pnpm build` - Build for production
- `pnpm start` - Start production server
- `pnpm db:setup` - Set up database
- `pnpm db:seed` - Seed database with sample data
- `pnpm db:generate` - Generate database migrations
- `pnpm db:migrate` - Run database migrations
- `pnpm db:studio` - Open Drizzle Studio

## 🔧 Environment Variables

Required environment variables:

- `POSTGRES_URL` - PostgreSQL connection string
- `STRIPE_SECRET_KEY` - Stripe secret key
- `STRIPE_WEBHOOK_SECRET` - Stripe webhook secret
- `BASE_URL` - Base URL of your application (e.g., http://localhost:3000)
- `AUTH_SECRET` - Secret key for authentication

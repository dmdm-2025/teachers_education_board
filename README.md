# Teacher's Education Platform

A modern web platform for teacher education, professional development, and career growth. This application provides a comprehensive solution for educators to enhance their skills, connect with opportunities, and access valuable resources.

## 🚀 Features

- **AI-Powered Counselor**: Get personalized career guidance and teaching advice
- **Interactive Lead Capture**: Multi-step form to collect teacher information and preferences
- **Membership Plans**: Subscription-based access to premium content and resources
- **Responsive Design**: Fully responsive interface that works on all devices
- **Dark Mode**: Beautiful dark theme for comfortable viewing
- **Secure Authentication**: NextAuth.js integration for user authentication
- **Database Integration**: PostgreSQL database with Prisma ORM
- **Email Notifications**: Automated email communication with Resend
- **Payment Processing**: Secure payment integration with Razorpay

## 🛠️ Tech Stack

- **Frontend**: Next.js 14, TypeScript, Tailwind CSS
- **UI Components**: Headless UI, Hero Icons, Framer Motion
- **Backend**: Next.js API Routes
- **Database**: PostgreSQL with Prisma ORM
- **Authentication**: NextAuth.js
- **Payments**: Razorpay
- **Email**: Resend
- **AI**: OpenAI GPT-4 (with GPT-3.5 fallback)
- **Deployment**: Vercel

## 🚀 Getting Started

### Prerequisites

- Node.js 18.0.0 or later
- PostgreSQL database
- npm or yarn

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/dmdm-2025/teachers_education_board.git
   cd teachers_education_board
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Set up environment variables:
   - Copy `.env.example` to `.env.local`
   - Update the variables with your configuration

4. Set up the database:
   ```bash
   npx prisma generate
   npx prisma db push
   ```

5. Run the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```

6. Open [http://localhost:3000](http://localhost:3000) in your browser

## 📦 Project Structure

```
.
├── prisma/           # Database schema and migrations
├── public/           # Static files
├── src/
│   ├── app/          # Next.js app directory
│   ├── components/   # Reusable UI components
│   ├── lib/          # Utility functions and configurations
│   └── styles/       # Global styles
├── .env.example      # Example environment variables
└── package.json      # Project dependencies and scripts
```

## 🔧 Configuration

### Environment Variables

Create a `.env.local` file in the root directory and add the following variables:

```env
# Database
DATABASE_URL="postgresql://user:password@localhost:5432/your_database_name"

# Next Auth
NEXTAUTH_URL="http://localhost:3000"
NEXTAUTH_SECRET="your_nextauth_secret_here"

# OpenAI
OPENAI_API_KEY="your_openai_api_key_here"

# Resend
RESEND_API_KEY="your_resend_api_key_here"
RESEND_FROM_EMAIL="noreply@yourdomain.com"
ADMIN_EMAIL="admin@yourdomain.com"

# Razorpay
NEXT_PUBLIC_RAZORPAY_KEY_ID="your_razorpay_key_id"
RAZORPAY_KEY_SECRET="your_razorpay_key_secret"
```

## 🛠️ Scripts

- `dev`: Start the development server
- `build`: Build the application for production
- `start`: Start the production server
- `lint`: Run ESLint
- `type-check`: Check TypeScript types
- `prisma:generate`: Generate Prisma client
- `prisma:push`: Push schema to database

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Next.js](https://nextjs.org/) - The React Framework
- [Tailwind CSS](https://tailwindcss.com/) - A utility-first CSS framework
- [Prisma](https://www.prisma.io/) - Next-generation ORM for Node.js & TypeScript

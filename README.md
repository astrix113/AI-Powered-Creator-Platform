# Creatr

A modern, AI-powered platform for content creators to write, publish, and grow their audience. Built with Next.js, Convex, and cutting-edge AI tools.

![Creatr Logo](https://via.placeholder.com/800x400/000000/FFFFFF?text=Creatr)

## ✨ Features

- **AI Writing Assistant**: Get smart suggestions for titles, content, and SEO optimization using Google Gemini
- **Community Building**: Grow your audience with followers, comments, likes, and engagement tools
- **Analytics & Insights**: Track performance with detailed view counts, engagement metrics, and charts
- **Content Scheduling**: Plan and schedule your content with real-time updates
- **AI Image Transformations**: Transform images with background removal, smart crop, and text overlays using ImageKit
- **Content Discovery**: Explore trending content and discover new creators in your personalized feed
- **Rich Text Editor**: Create beautiful content with React Quill editor
- **Dark/Light Theme**: Seamless theme switching with next-themes
- **Responsive Design**: Optimized for all devices with Tailwind CSS and shadcn/ui components

## 🚀 Tech Stack

- **Frontend**: Next.js 16, React 18, TypeScript
- **Backend**: Convex (real-time database)
- **Authentication**: Clerk
- **AI**: Google Generative AI (Gemini)
- **Image Processing**: ImageKit
- **Styling**: Tailwind CSS, shadcn/ui, Radix UI
- **Charts**: Chart.js, React Chart.js 2
- **Forms**: React Hook Form, Zod validation
- **Icons**: Lucide React

## 📋 Prerequisites

- Node.js 18+
- npm, yarn, pnpm, or bun
- Convex account
- Clerk account
- ImageKit account

## 🛠️ Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/creatr.git
   cd creatr
   ```

2. **Install dependencies**

   ```bash
   npm install
   # or
   yarn install
   # or
   pnpm install
   # or
   bun install
   ```

3. **Set up Convex**

   ```bash
   npx convex dev --once
   ```

   This will create a `.env.local` file with your Convex URL.

4. **Configure environment variables**

   Create a `.env.local` file in the root directory and add:

   ```env
   # Convex
   NEXT_PUBLIC_CONVEX_URL=your_convex_url

   # Clerk
   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
   CLERK_SECRET_KEY=your_clerk_secret_key
   NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
   NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
   NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/dashboard
   NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/dashboard

   # Google Gemini AI
   GOOGLE_GENERATIVE_AI_API_KEY=your_gemini_api_key

   # ImageKit
   NEXT_PUBLIC_IMAGEKIT_URL_ENDPOINT=your_imagekit_url
   IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
   IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
   ```

5. **Set up Clerk authentication**
   - Go to [Clerk Dashboard](https://dashboard.clerk.com/)
   - Create a new application
   - Copy the publishable key and secret key to your `.env.local`

6. **Set up ImageKit**
   - Go to [ImageKit Dashboard](https://imagekit.io/dashboard)
   - Create a new account/project
   - Copy the URL endpoint, public key, and private key to your `.env.local`

7. **Set up Google Gemini AI**
   - Go to [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Create an API key
   - Add it to your `.env.local`

## 🚀 Running the Application

1. **Start the development server**

   ```bash
   npm run dev
   # or
   yarn dev
   # or
   pnpm dev
   # or
   bun dev
   ```

2. **Open your browser**

   Navigate to [http://localhost:3000](http://localhost:3000)

## 📁 Project Structure

```
creatr/
├── app/                    # Next.js app router pages
│   ├── (auth)/            # Authentication pages
│   ├── (public)/          # Public-facing pages
│   ├── dashboard/         # User dashboard
│   ├── api/               # API routes
│   └── globals.css        # Global styles
├── components/            # Reusable React components
│   ├── ui/               # shadcn/ui components
│   └── ...               # Custom components
├── convex/               # Convex backend functions
│   ├── schema.js         # Database schema
│   └── ...               # Query/mutation functions
├── hooks/                # Custom React hooks
├── lib/                  # Utility functions and data
├── public/               # Static assets
└── ...                   # Config files
```

## 🎯 Usage

### Creating Content

1. Sign up or sign in to your account
2. Navigate to the dashboard
3. Click "Create Post" to open the editor
4. Use the AI writing assistant for suggestions
5. Add images and format your content
6. Publish or save as draft

### Managing Your Profile

- Update your profile information in Settings
- View your posts and analytics in the Dashboard
- Manage followers and engagement

### Exploring Content

- Browse the public feed for trending content
- Visit creator profiles to follow and engage
- Use search to discover specific topics

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Next.js](https://nextjs.org/) - The React framework
- [Convex](https://www.convex.dev/) - Real-time database
- [Clerk](https://clerk.com/) - Authentication
- [ImageKit](https://imagekit.io/) - Image processing
- [Google Gemini](https://ai.google.dev/) - AI assistance
- [shadcn/ui](https://ui.shadcn.com/) - UI components

## 📞 Support

If you have any questions or need help, please open an issue on GitHub or contact the maintainers.

---

Built with ❤️ for content creators everywhere.

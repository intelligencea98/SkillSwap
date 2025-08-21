# SkillSwap - Trade Skills, Build Community

A modern web application that enables neighbors to exchange skills without money, powered by blockchain technology for secure transactions.

## 🚀 Features

- **Skill Trading**: Connect with neighbors to exchange skills and services
- **AI-Powered Matching**: Smart algorithm matches users based on skills and location
- **Blockchain Security**: Secure transactions using Algorand blockchain
- **Points System**: Earn and spend points for fair skill exchanges
- **Real-time Communication**: Contact system for task coordination
- **Mobile Responsive**: Optimized for all devices

## 🛠️ Tech Stack

- **Frontend**: React 18, TypeScript, Tailwind CSS
- **Backend**: Supabase (PostgreSQL, Auth, Real-time)
- **Blockchain**: Algorand SDK
- **Build Tool**: Vite
- **Deployment**: Netlify
- **Icons**: Lucide React

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/your-username/skillswap.git
cd skillswap
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
```bash
cp .env.example .env
```

Fill in your Supabase credentials:
```env
VITE_SUPABASE_URL=your_supabase_project_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

4. Start the development server:
```bash
npm run dev
```

## 🗄️ Database Setup

The application uses Supabase for data storage. Migration files are included in the `supabase/migrations/` directory.

### Tables:
- `users` - User profiles and authentication
- `tasks` - Skill exchange tasks
- `task_applications` - Task applications and assignments
- `contact_requests` - Contact information sharing

## 🚀 Deployment

### Netlify Deployment

1. Build the project:
```bash
npm run build
```

2. Deploy to Netlify:
   - Connect your GitHub repository to Netlify
   - Set build command: `npm run build`
   - Set publish directory: `dist`
   - Add environment variables in Netlify dashboard

### Environment Variables for Production

```env
VITE_SUPABASE_URL=your_production_supabase_url
VITE_SUPABASE_ANON_KEY=your_production_supabase_anon_key
```

## 🔧 Development

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint
- `npm run lint:fix` - Fix ESLint errors
- `npm run type-check` - Run TypeScript type checking

### Code Structure

```
src/
├── components/          # Reusable UI components
│   ├── auth/           # Authentication components
│   ├── blockchain/     # Blockchain-related components
│   ├── common/         # Common components (ErrorBoundary, SEO)
│   ├── layout/         # Layout components (Navbar, Footer)
│   ├── tasks/          # Task-related components
│   └── ui/             # Basic UI components
├── context/            # React context providers
├── hooks/              # Custom React hooks
├── lib/                # External library configurations
├── pages/              # Page components
├── services/           # API and external services
├── types/              # TypeScript type definitions
└── utils/              # Utility functions
```

## 🔐 Security Features

- Row Level Security (RLS) on all database tables
- Input validation and sanitization
- CSRF protection
- Secure headers configuration
- Environment variable protection

## 📱 Progressive Web App

The application includes PWA features:
- Web App Manifest
- Service Worker (can be added)
- Offline functionality (can be enhanced)
- Install prompts

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/new-feature`
3. Commit changes: `git commit -am 'Add new feature'`
4. Push to branch: `git push origin feature/new-feature`
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

For support, email support@skillswap.com or create an issue in the GitHub repository.

## 🙏 Acknowledgments

- Built with [Bolt.new](https://bolt.new)
- Icons by [Lucide](https://lucide.dev)
- Images from [Pexels](https://pexels.com)
- Blockchain powered by [Algorand](https://algorand.com)
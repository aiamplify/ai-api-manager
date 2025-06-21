# AI API Manager

A comprehensive web application for managing and monitoring AI API usage across multiple providers. Track costs, set budgets, analyze usage patterns, and optimize your AI spending with detailed analytics and insights.

## 🚀 Features

### Core Functionality
- **Multi-Provider Support**: Manage API keys and track usage for OpenAI, Anthropic, Google AI, Perplexity, and more
- **Real-time Usage Tracking**: Monitor token consumption, request counts, and costs across all your AI services
- **Cost Analytics**: Detailed breakdowns of spending by provider, model, and time period
- **Budget Management**: Set spending limits with customizable alerts and notifications
- **Usage Insights**: AI-powered recommendations for cost optimization and usage patterns

### Dashboard & Analytics
- **Interactive Charts**: Visualize usage trends, cost breakdowns, and performance metrics
- **Custom Date Ranges**: Analyze data across different time periods
- **Export Capabilities**: Download usage reports and analytics data
- **Real-time Alerts**: Get notified when approaching budget limits or unusual usage patterns

### Security & Privacy
- **Encrypted API Keys**: All API keys are securely encrypted and stored
- **User Authentication**: Secure login with NextAuth.js
- **Data Privacy**: Your usage data stays private and secure

## 🛠 Tech Stack

- **Frontend**: Next.js 14, React 18, TypeScript
- **Styling**: Tailwind CSS, Radix UI components
- **Database**: PostgreSQL with Prisma ORM
- **Authentication**: NextAuth.js
- **Charts**: Chart.js, Recharts, Plotly.js
- **State Management**: Zustand, React Query

## 📋 Prerequisites

- Node.js 18+ 
- PostgreSQL database
- npm or yarn package manager

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/aiamplify/ai-api-manager.git
cd ai-api-manager
```

### 2. Install Dependencies
```bash
cd app
npm install
# or
yarn install
```

### 3. Environment Setup
Create a `.env.local` file in the `app` directory:

```env
# Database
DATABASE_URL="postgresql://username:password@localhost:5432/ai_api_manager"

# NextAuth
NEXTAUTH_URL="http://localhost:3000"
NEXTAUTH_SECRET="your-secret-key-here"

# Optional: OAuth providers
GOOGLE_CLIENT_ID="your-google-client-id"
GOOGLE_CLIENT_SECRET="your-google-client-secret"
```

### 4. Database Setup
```bash
# Generate Prisma client
npx prisma generate

# Run database migrations
npx prisma db push

# Seed the database with initial data
npm run seed
```

### 5. Start Development Server
```bash
npm run dev
```

Visit `http://localhost:3000` to access the application.

## 📊 Database Schema

The application uses a comprehensive database schema with the following main entities:

- **Users**: User accounts and authentication
- **Providers**: AI service providers (OpenAI, Anthropic, etc.)
- **Models**: Available AI models with pricing information
- **ApiKeys**: Encrypted storage of user API keys
- **UsageData**: Detailed usage tracking and cost calculations
- **Budgets**: Spending limits and budget management
- **Alerts**: Notifications and warnings
- **Insights**: AI-powered usage recommendations

## 🔧 Configuration

### Adding New Providers
1. Add provider information to the database via the admin interface
2. Configure pricing models for each provider's offerings
3. Set up API integration for automatic usage tracking (if supported)

### Setting Up Budgets
1. Navigate to the Budgets section
2. Create budgets for specific providers, models, or global spending
3. Configure alert thresholds and notification preferences

## 📈 Usage Analytics

The application provides comprehensive analytics including:

- **Cost Trends**: Track spending over time
- **Usage Patterns**: Identify peak usage periods and optimization opportunities
- **Model Comparison**: Compare costs and performance across different AI models
- **Provider Analysis**: Evaluate spending distribution across providers

## 🔒 Security

- API keys are encrypted using industry-standard encryption
- All database connections use secure protocols
- User sessions are managed securely with NextAuth.js
- Regular security updates and dependency management

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/aiamplify/ai-api-manager/issues) page
2. Create a new issue with detailed information
3. Join our community discussions

## 🗺 Roadmap

- [ ] Additional AI provider integrations
- [ ] Advanced cost optimization algorithms
- [ ] Team collaboration features
- [ ] API for third-party integrations
- [ ] Mobile application
- [ ] Advanced reporting and export options

---

Built with ❤️ for the AI community

# reddit-clone-project


A modern, full-stack Reddit clone built with Next.js, React, TypeScript, Prisma, and PostgreSQL.

## 🌟 Features

- ✨ **Beautiful, Modern UI** - Reddit-inspired design with light and dark mode support
- 🔐 **User Authentication** - Register and login with secure password hashing
- 📝 **Posts & Communities** - Create posts in different communities
- 💬 **Comments** - Add comments to posts and engage with community
- ⬆️⬇️ **Voting System** - Upvote and downvote posts
- 📱 **Responsive Design** - Works seamlessly on desktop and mobile
- 🗄️ **PostgreSQL Database** - Robust data persistence
- ⚡ **Server-Side & Client-Side Rendering** - Optimal performance

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- PostgreSQL database
- npm or yarn

### Installation

1. **Clone and Install**
```bash
npm install
```

2. **Configure Database**
   - Edit `.env` file with your PostgreSQL connection string
   - Example: `DATABASE_URL="postgresql://postgres:root123@localhost:5432/reddit_clone"`

3. **Setup Database**
```bash
npm run db:push
npm run db:seed
```

4. **Start Development Server**
```bash
npm run dev
```

5. **Open in Browser**
   - Navigate to [http://localhost:3000](http://localhost:3000)
   - Login with: `dev@example.com` / `password123`

## 📚 Database Schema

- **Users** - User accounts with authentication
- **Communities** - Topic-based communities
- **Posts** - User-created content in communities
- **Comments** - Discussion threads on posts
- **Votes** - User interactions (upvotes/downvotes)

## 🔗 API Endpoints

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/auth/login` | POST | User login |
| `/api/register` | POST | User registration |
| `/api/post` | GET, POST | Posts management |
| `/api/community` | GET, POST | Communities management |
| `/api/comment` | GET, POST | Comments management |
| `/api/vote` | POST | Voting |

## 📦 Tech Stack

- **Frontend**: React 19, Next.js 16, TypeScript, Tailwind CSS
- **Backend**: Next.js API Routes
- **Database**: PostgreSQL with Prisma ORM
- **Authentication**: bcrypt for password hashing
- **UI Components**: Custom React components with Tailwind CSS
- **Notifications**: React Hot Toast

## 🛠️ Available Scripts

```bash
npm run dev           # Start development server
npm run build         # Build for production
npm run start         # Start production server
npm run db:push       # Sync Prisma schema to database
npm run db:seed       # Populate database with sample data
npm run db:reset      # Reset database (caution!)
npm run lint          # Run ESLint
```

## 📖 Detailed Setup Guide

For step-by-step instructions, see [SETUP.md](./SETUP.md)

## 🎨 Design Features

- Modern gradient-based color scheme
- Smooth transitions and hover effects
- Dark mode support with system preference detection
- Mobile-responsive grid layout
- Professional typography

## 🔒 Security

- Passwords hashed with bcrypt
- SQL injection prevention via Prisma ORM
- Environment variables for sensitive data
- Secure session handling

## 🚧 Future Enhancements

- [ ] Direct messaging between users
- [ ] User profiles and customization
- [ ] Search functionality
- [ ] Image upload support
- [ ] Real-time notifications
- [ ] User karma and reputation system
- [ ] Community moderation tools

## 📝 Sample Credentials

After running `npm run db:seed`:

| Email | Password |
|-------|----------|
| dev@example.com | password123 |
| designer@example.com | password123 |
| fullstack@example.com | password123 |

## 🤝 Contributing

Contributions are welcome! Feel free to open issues and submit pull requests.

## 📄 License

This project is open source and available under the MIT License.

## 🆘 Troubleshooting

**Database Connection Error**
- Ensure PostgreSQL is running
- Check DATABASE_URL in .env file
- Run `npm run db:push`

**Port Already in Use**
- Run on different port: `npm run dev -- -p 3001`

**Prisma Issues**
- Clear cache: `rm -rf node_modules/.prisma`
- Regenerate: `npx prisma generate`

For more help, see [SETUP.md](./SETUP.md#troubleshooting)

---

Built with ❤️ using Next.js and Prisma

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.

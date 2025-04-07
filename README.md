# Graphy - Tattoo Artist Social Network

A social network platform for tattoo artists to showcase their work, connect with clients, and manage their business.

## Features

- User authentication and profiles
- Tattoo portfolio management
- Direct messaging between users
- User blocking functionality
- Message read status tracking
- Search functionality
- Responsive design

## Tech Stack

- Next.js 14
- TypeScript
- Prisma
- PostgreSQL
- NextAuth.js
- Tailwind CSS
- Playwright (E2E testing)
- Jest (Unit & Integration testing)

## Getting Started

### Prerequisites

- Node.js 18+
- PostgreSQL
- npm or yarn

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Kayler1303/graphy.git
   cd graphy
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   ```bash
   cp .env.example .env.local
   ```
   Fill in the required environment variables in `.env.local`

4. Set up the database:
   ```bash
   npx prisma generate
   npx prisma migrate dev
   ```

5. Start the development server:
   ```bash
   npm run dev
   ```

## Testing

The project includes comprehensive test coverage:

### Unit Tests
```bash
npm test
```

### Integration Tests
```bash
npm test -- --testPathPattern=integration
```

### E2E Tests
```bash
npm run test:e2e
```

### Test Coverage
```bash
npm run test:coverage
```

## CI/CD Pipeline

The project uses GitHub Actions for continuous integration and deployment:

- Runs on every push to main and pull requests
- Executes unit, integration, and E2E tests
- Generates and uploads test reports
- Uploads coverage reports to Codecov

## Project Structure

```
src/
├── app/              # Next.js app router
├── components/       # React components
├── lib/             # Utility functions
├── prisma/          # Database schema
└── tests/           # Test files
    ├── e2e/         # End-to-end tests
    └── integration/ # Integration tests
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Next.js team for the amazing framework
- Prisma team for the excellent ORM
- All contributors and supporters 
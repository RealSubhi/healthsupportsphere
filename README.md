# Support Sphere - Healthcare Community Platform

A comprehensive healthcare support platform that enables users to connect, share experiences, and access trusted medical resources. Built with React, TypeScript, and Express.js.

## Features

### 🏥 Healthcare Communities
- Condition-specific support groups (Diabetes, PCOS, Cancer, Mental Health)
- Anonymous posting for privacy
- Expert-verified content
- Community membership tracking

### 📅 Events & Workshops
- Virtual and in-person healthcare events
- Educational workshops with certified professionals
- Event registration and attendance tracking
- Featured events for better discovery

### 👥 Local Support Groups
- Location-based group discovery
- In-person meetup coordination
- Verified organizers and contact information
- Meeting schedules and location details

### 🆘 Support System
- 24/7 support ticket system
- Medical and community assistance
- Priority-based ticket handling
- Expert response tracking

### 📚 Resource Library
- Expert-reviewed health information
- Categorized medical resources
- Treatment guides and educational materials
- Downloadable content

## Tech Stack

### Frontend
- **React 18** with TypeScript
- **Tailwind CSS** for styling
- **Radix UI** components
- **TanStack Query** for state management
- **Wouter** for routing
- **Vite** for development and building

### Backend
- **Node.js** with Express.js
- **TypeScript** for type safety
- **PostgreSQL** with Drizzle ORM
- **Neon Database** for serverless PostgreSQL
- **Zod** for validation

## Getting Started

### Prerequisites
- Node.js 18 or higher
- PostgreSQL database (Neon recommended)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/support-sphere.git
cd support-sphere
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
```bash
# Copy the example environment file
cp .env.example .env

# Add your database URL
DATABASE_URL=your_postgresql_connection_string
```

4. Run database migrations:
```bash
npm run db:push
```

5. Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:5000`

## Development

### Project Structure
```
├── client/          # React frontend
├── server/          # Express backend
├── shared/          # Shared types and schemas
└── migrations/      # Database migrations
```

### Available Scripts
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run db:push` - Push schema changes to database
- `npm run db:studio` - Open database studio

## API Endpoints

### Communities
- `GET /api/communities` - List all communities
- `POST /api/communities/:id/join` - Join a community
- `POST /api/communities/:id/leave` - Leave a community

### Posts
- `GET /api/posts` - Get community posts
- `POST /api/posts` - Create new post
- `POST /api/posts/:id/like` - Like a post

### Events
- `GET /api/events` - List healthcare events
- `POST /api/events` - Create new event
- `POST /api/events/:id/register` - Register for event

### Local Groups
- `GET /api/local-groups` - Find local support groups
- `POST /api/local-groups` - Create new group
- `POST /api/local-groups/:id/join` - Join group

### Support
- `GET /api/support/tickets` - Get support tickets
- `POST /api/support/tickets` - Create support ticket

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Privacy & Security

This platform is designed with healthcare privacy in mind:
- Anonymous posting capabilities
- Secure user authentication
- HIPAA-compliant data handling
- Encrypted sensitive information

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For support, please create a ticket through the platform's support system or contact the development team.

## Acknowledgments

- Built for the healthcare community
- Designed with accessibility and privacy as priorities
- Inspired by the need for safe, supportive healthcare discussions
# testcompo

test

## Tech Stack

- Node.js 18+
- Express.js
- TypeScript
- Jest (testing)

## Getting Started

### Prerequisites

- Node.js 18 or higher
- npm or yarn

### Installation
```bash
# Install dependencies
npm install

# Copy environment variables
cp .env.example .env

# Start development server
npm run dev
```

The API will be available at `http://localhost:3000`

## API Endpoints

### Service Information
```
GET /
```

Returns service information and available endpoints.

### Health Check
```
GET /health
```

Returns service health status.

### Get Items
```
GET /api/items
```

Returns a list of items.

### Create Item
```
POST /api/items
Content-Type: application/json

{
  "name": "Item name",
  "description": "Item description"
}
```

Creates a new item.

## Development
```bash
# Run in development mode with hot reload
npm run dev

# Build for production
npm run build

# Run tests
npm test

# Lint code
npm run lint

# Format code
npm run format
```

## Docker
```bash
# Build image
docker build -t testcompo .

# Run container
docker run -p 3000:3000 testcompo
```

## Environment Variables

- `PORT` - Server port (default: 3000)
- `NODE_ENV` - Environment (development/production)

## Project Structure
```
├── src/
│   ├── index.ts       # Main application file
│   └── routes.ts      # API routes
├── dist/              # Compiled JavaScript (generated)
├── Dockerfile         # Docker configuration
├── package.json       # Dependencies
└── tsconfig.json      # TypeScript configuration
```

## Owner

group:default/devops

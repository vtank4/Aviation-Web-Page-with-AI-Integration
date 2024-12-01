# FULL-STACK WEB APPLICATION - Civil Aviation Project

## Project Overview
A comprehensive full-stack web application that provides real-time flight price predictions using machine learning capabilities. The application integrates a user-friendly frontend with FastAPI backend and employs Random Forest algorithms for accurate pricing predictions.

## Features
- Real-time flight price prediction
- Price categorization (budget, moderate, expensive)
- Interactive data visualizations using Plotly.js
- Auto-suggestion input for destinations
- JWT authentication for secure access
- Rate limiting for DDOS protection
- Server-side rendering for optimal performance

## Tech Stack
### Frontend
- Next.js 14
- React
- TailwindCSS
- shadcn/ui, aceternity-ui, magic-ui
- Plotly.js for data visualization
- Zod for input validation

### Backend
- FastAPI
- JWT authentication
- PostgreSQL with Prisma ORM
- SerpAPI integration for real-time flight data

### Machine Learning
- Random Forest model with 84.10% accuracy
- pandas for data processing
- scikit-learn for model implementation

## Architecture
- Client Layer (Frontend):
  - Server-side rendering (SSR)
  - Responsive design
  - Type-safe server actions
  - Form validation with Zod

- Server Layer (Backend):
  - RESTful API endpoints
  - JWT middleware
  - Connection pooling
  - Rate limiting protection

## Performance
- First Contentful Paint (FCP): < 500ms
- API response time: Optimized with caching
- Data processing: Efficient with connection pooling
- Model prediction accuracy: 84.10%

## Security Features
- JWT authentication required for protected routes
- Rate limiting middleware for DDOS protection
- Input validation on both client and server side
- Secure API endpoints with proper error handling

## Installation

```bash
# Clone repository
git clone [repository-url]

# Install dependencies
npm install

# Environment setup
cp .env.example .env

# Run development server
npm run dev
```

## API Documentation
Essential endpoints:
- `POST /api/v1/auth/signUp`: User registration
- `POST /api/v1/auth/signIn`: User authentication
- `GET /api/v1/flight-prices/destinations`: Get available destinations
- `POST /api/v1/prediction`: Generate flight price predictions

Full API documentation available at `localhost:8000/docs`

## Authors
- Xuan Tuan Minh Nguyen
- Ba Viet Anh (Henry) Nguyen
- Trong Dat Hoang

## License
- Please follow license in LICENSE.md file

## Acknowledgments
- FastAPI documentation and community
- Next.js documentation
- Zeppelin Universität for the dataset


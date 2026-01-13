# product-admin-web-app

## Technologies Used

### Frontend

- ReactJS (Vite)
- TypeScript
- Tailwind CSS
- Shadcn
- Axios
- Tanstack Query
- Sonner (Toast notifications)

### Backend

- Node.js
- Express.js
- PostgreSQL
- Drizzle ORM

## Local Development Setup

### Prerequisites

- Node.js (v18 or higher)
- PostgreSQL
- npm (v9 or higher)

### Installation

1. Clone the repository and cd product-admin-web-app
2. Install dependencies:
   ```bash
   navigate to frontend folder then open cmd then npm install (to install dependencies)
   navigate to backend folder then open cmd then npm install (to install dependencies)
   ```

### Database Setup

1. Create a PostgreSQL database
2. Add / Update the `.env` file in the backend directory with your database credentials (view env.example for reference). The website uses [Neon tech](https://neon.tech) for the database connection.
3. Run database migrations:
   ```bash
   'root folder'
   npm run generate
   npm run migrate
   ```

### Environment Variables

Create `.env` files in both frontend and backend directories:

**Frontend (.env)**
exactly like this to run locally

replace the url where your backend is running

```bash
VITE_API_URL=http://localhost:5001/
```

**Backend (.env)**

update the url where you database is located

should be your own Database url
```bash
DATABASE_URL=postgresql://user:password@localhost:5432/database_name
```

## Backend setup

in the index.js for backend add the Frontend url (in allowedOrigins) where your client is running to allow cors origin

## Running the Application

by default it should be running this localhost ports

- **Backend**: http://localhost:5001 
- **Frontend**: http://localhost:5173

1.  run them separately:
   - Frontend:
     ```bash
     npm run dev
     ```
     
   - Backend:
     ```bash
     npm run start
     ```

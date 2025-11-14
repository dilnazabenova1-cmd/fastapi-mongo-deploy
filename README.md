[README.md](https://github.com/user-attachments/files/23547321/README.md)

# HotelEase Microservice

## Setup & Deployment

1. Create MongoDB Atlas cluster and get MONGO_URI.
2. Set environment variables in Render:
   - MONGO_URI
   - DB_NAME
   - JWT_SECRET
3. Build Docker image locally:
   docker build -t hoteleaze .
4. Run locally:
   docker run -p 8000:8000 --env-file .env hoteleaze
5. Deploy to Render using Docker & env variables.
6. Test endpoints:
   - /health
   - /health/db
   - /api/rooms (CRUD)
   - /api/guests (CRUD)
   - /api/bookings (CRUD)

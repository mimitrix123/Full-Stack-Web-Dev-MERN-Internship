# E-Commerce Capstone

MERN capstone implementing product listing, authentication, cart, order creation and admin product endpoints.

## Local setup
1. Start MongoDB or create a MongoDB Atlas database.
2. In `server`, copy `.env.example` to `.env` and set `MONGO_URI` and `JWT_SECRET`.
3. `npm install && npm start`.
4. In `client`, set `VITE_API_URL` if the server is not on `http://localhost:5005/api`.
5. `npm install && npm run dev`.

## Deployment
- Frontend: Vercel or Netlify; set `VITE_API_URL` to the deployed API.
- Backend: Render/other Node host; set `MONGO_URI`, `JWT_SECRET`, `CLIENT_URL`, and `PORT`.
- Database: MongoDB Atlas.

## Production checklist
- Add an admin bootstrap route or seed script with controlled credentials.
- Validate/sanitize all request bodies.
- Add rate limiting, Helmet, structured logging, tests, image storage, payment provider, and order inventory transactions before production use.

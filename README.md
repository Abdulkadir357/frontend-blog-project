# Build Journey Notes

I built this project from scratch as a full stack blog. These are the notes I keep for my future self so I remember the main steps and fixes.

1. **Choosing React + Vite** – I scaffolded the frontend with Vite + React, set up the entry files, and wrote components for the form and post list.
2. **Talking to the API** – I created a custom hook (`usePosts`) and a `services/api.js` module to handle fetching and creating posts with proper loading and error states.
3. **Coding the backend** – I built an Express server that reads environment variables, uses a Mongoose schema for validation, and returns JSON responses with clear status codes.
4. **Protecting secrets** – I stored MongoDB credentials in `.env` files and exposed a `CORS_ORIGIN` setting so I control which frontends can call the API.
5. **Connecting to MongoDB Atlas** – I set up an Atlas cluster, created the user (`db-user123`), plugged the connection string into the backend, and verified the “Connected to MongoDB” log.
6. **Fixing npm conflicts** – I resolved an `eslint` peer dependency issue by pinning `eslint` to `^8.57.1` so it matches `eslint-config-react-app`.
7. **Handling runtime errors** – I kept the backend running with the correct `.env` values so the frontend fetch calls succeed; when something failed, I checked the server logs first.

These notes capture the full build so I can repeat it or troubleshoot quickly later.


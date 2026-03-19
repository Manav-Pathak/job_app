# CareerSphere - Job Portal Web App

CareerSphere is a full-stack job portal where candidates can discover and apply for jobs, and recruiters/admins can manage companies, post openings, and review applicants.

## Key Features

- User authentication (signup/login) with JWT and cookies
- Job browsing and job detail pages for candidates
- Apply-to-job workflow and applied jobs tracking
- Admin dashboard for company and job management
- Applicant management for posted jobs
- Profile update flow with image upload support

## Tech Stack

### Frontend

- React + Vite
- Redux Toolkit (+ redux-persist)
- React Router
- Tailwind CSS + Radix UI

### Backend

- Node.js + Express
- MongoDB + Mongoose
- JWT authentication
- Multer + Cloudinary (file upload)

## Basic Project Structure

```text
job_app/
|-- backend/                # Express API + MongoDB models/routes/controllers
|-- frontend/               # React client app
|-- readme.md
```

## Run Locally

### 1) Clone and install dependencies

```bash
git clone <your-repo-url>
cd job_app

cd backend
npm install

cd ../frontend
npm install
```

### 2) Configure environment variables

Create `backend/.env`:

```env
PORT=8000
MONGO_URI=your_mongodb_connection_string
SECRET_KEY=your_jwt_secret

# Optional (needed for image upload features)
CLOUD_NAME=your_cloudinary_cloud_name
API_KEY=your_cloudinary_api_key
API_SECRET=your_cloudinary_api_secret
```

### 3) Start backend

```bash
cd backend
npm run dev
```

### 4) Start frontend

```bash
cd frontend
npm run dev
```

Frontend runs on `http://localhost:5173` and connects to backend on `http://localhost:8000`.

## UI Screenshots

Add your screenshots below:



Tip: create a `screenshots/` folder in the project root and place image files there.

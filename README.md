# JobLane – Job Portal  

JobLane is a **full-stack job portal** built with the MERN stack. It connects **job seekers** with **employers** and provides an **admin panel** for managing the platform. Users can register, log in, upload resumes, and apply for jobs, while employers can post and manage job listings.  

🌐 **Live Demo**:  
- **Frontend (Vercel)** → [https://joblaneapp.vercel.app/](https://joblaneapp.vercel.app/)  
- **Backend (Render)** → [https://joblane-g8id.onrender.com/](https://joblane-g8id.onrender.com/)  

---

## 🚀 Features
- 🔑 User authentication with JWT  
- 👨‍💼 Role-based access (**Applicant**, **Employer**, **Admin**)  
- 📝 Employers can post and manage jobs  
- 📂 Applicants can apply for jobs with resumes  
- 🖼️ Cloudinary integration for file uploads (avatars & resumes)  
- 📊 Admin can manage all jobs and users  
- 🌍 Deployed with **Vercel** (frontend) and **Render** (backend)  

---

## 🛠️ Tech Stack
**Frontend**
- React (Vite)  
- TailwindCSS  

**Backend**
- Node.js  
- Express.js  
- MongoDB Atlas (Mongoose)  
- Cloudinary  
- JWT + bcrypt  

---

## ⚙️ Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/joblane.git
cd joblane
```
## ⚙️ Setup Instructions

### 2. Backend Setup
```bash
cd server
npm install
```
#### Create a file server/config/config.env:

```ini
PORT=5000
DB=mongodb+srv://<username>:<password>@cluster.mongodb.net/joblane
CLOUDINARY_NAME=<your_cloudinary_name>
CLOUDINARY_API_KEY=<your_cloudinary_api_key>
CLOUDINARY_API_SECRET=<your_cloudinary_api_secret>
JWT_SECRET=<your_secret>
```
#### Run backend:

```bash
npm run dev
```
### 3. Frontend Setup
```bash
cd ../client
npm install
```
#### Create a .env in client/:

```ini
VITE_API_URL=http://localhost:5000
```
#### Run frontend:

```bash
npm run dev
```
## 🌐 Deployment

### Backend (Render)

1. Push repo to GitHub.
2. Create a Web Service on Render.
3. Select the server/ folder and set environment variables from config.env.
4. Deploy → get backend URL.

👉 Current deployment: [ https://joblane-g8id.onrender.com/](https://joblane-g8id.onrender.com/)

### Frontend (Vercel)

1. Push repo to GitHub.
2. Import the repo into Vercel.
3. Select the client/ folder.
4. Build settings:
```ini
Build Command → npm run build

Publish Directory → dist
```
5. Add environment variable:

```ini
VITE_API_URL=https://joblane-g8id.onrender.com/
```
Deploy → get frontend URL.

👉 Current deployment: [https://joblaneapp.vercel.app/](https://joblaneapp.vercel.app/)

👤 Author
Developed from scratch by Mrigank Mouli Singh
🔗 [LinkedIn](https://www.linkedin.com/in/mrigank-mouli-singh/)

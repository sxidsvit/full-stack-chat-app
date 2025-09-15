# Full-Stack Chat Application

A modern, real-time chat application built with a **Node.js** and **Express** backend, a **React** frontend, and **MongoDB** for data persistence. This project features custom JWT authentication, real-time messaging with **Socket.io**, image uploads via **Cloudinary**, and a sleek UI styled with **Tailwind CSS** and **DaisyUI**. It includes API rate-limiting with **Arcjet**, welcome emails via **Resend**, and supports easy deployment on free-tier platforms like **Sevalla**.

[Site](https://full-stack-chat-app-c3jmp.sevalla.app/)

## Features

- 🔐 **Custom JWT Authentication**: Secure user authentication without third-party services.
- ⚡ **Real-Time Messaging**: Powered by Socket.io for instant chat updates.
- 🟢 **Online/Offline Indicators**: Real-time user presence tracking.
- 🔔 **Notification & Typing Sounds**: Toggleable audio feedback for messages and typing events.
- 📨 **Welcome Emails**: Automated emails sent on signup using Resend.
- 🗂️ **Image Uploads**: Store and share images via Cloudinary.
- 🧰 **REST API**: Built with Node.js and Express.
- 🧱 **MongoDB Integration**: Persistent data storage with MongoDB.
- 🚦 **API Rate-Limiting**: Secure endpoints with Arcjet.
- 🎨 **Modern UI**: Built with React, Tailwind CSS, and DaisyUI.
- 🧠 **State Management**: Lightweight and efficient with Zustand.
- 🧑‍💻 **Git Workflow**: Organized with branches, pull requests, and merges.
- 🚀 **Easy Deployment**: Optimized for free-tier platforms like Sevalla.

## Prerequisites

- [Node.js](https://nodejs.org/en/docs/) (v20.0.0 or higher)
- [npm](https://docs.npmjs.com/) (included with Node.js)
- [MongoDB Atlas](https://www.mongodb.com/docs/atlas/) account for database hosting
- [Cloudinary](https://cloudinary.com/documentation) account for image uploads
- [Resend](https://resend.com/docs) account for email services
- [Arcjet](https://docs.arcjet.com/) account for API rate-limiting
- [Git](https://git-scm.com/doc) for version control
- [Socket.io](https://socket.io/docs/v4/) for real-time messaging
- [React](https://react.dev/reference) for frontend development
- [Tailwind CSS](https://tailwindcss.com/docs) and [DaisyUI](https://daisyui.com/docs/) for styling
- [Zustand](https://docs.pmnd.rs/zustand/) for state management
- [Sevalla](https://sevalla.com/docs/) for deployment

---

![]()<img src="demo.gif" alt="demo gif" width="620" height="485" style="display: block; margin-left:100px ;">

---

## Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/sxidsvit/full-stack-chat-app.git
   cd full-stack-chat-app
   ```

2. **Install Dependencies**:

   - Backend:
     ```bash
     cd backend
     npm install
     ```
   - Frontend:
     ```bash
     cd frontend
     npm install
     ```

3. **Set Up Environment Variables**:
   - Create a `.env` file in the `backend` directory with the following:
     ```env
     PORT=3000
     MONGO_URI=your_mongo_uri}^{+
     NODE_ENV=development
     JWT_SECRET=your_jwt_secret
     RESEND_API_KEY=your_resend_api_key
     EMAIL_FROM=your_email_from_address
     EMAIL_FROM_NAME=your_email_from_name
     CLIENT_URL=http://localhost:5173
     CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
     CLOUDINARY_API_KEY=your_cloudinary_api_key
     CLOUDINARY_API_SECRET=your_cloudinary_api_secret
     ARCJET_KEY=your_arcjet_key
     ARCJET_ENV=development
     ```
   - Replace placeholders with credentials from MongoDB Atlas, Cloudinary, Resend, and Arcjet.

## Running the Application

1. **Start the Backend**:

   ```bash
   cd backend
   npm run dev
   ```

   The backend runs on `http://localhost:3000` (or the port specified in `.env`).

2. **Start the Frontend**:

   ```bash
   cd frontend
   npm run dev
   ```

   The frontend runs on `http://localhost:517
3` (default for Vite).

3. **Access the App**:
   Open `http://localhost:5173` in your browser to use the chat application.

## Testing Locally

- Verify MongoDB connectivity using the `MONGO_URI`.
- Ensure Cloudinary and Resend services are configured correctly.
- Test real-time features (messaging, typing indicators) by opening multiple browser tabs or devices.

## Deployment

The app is optimized for deployment on Sevalla or similar platforms.

1. **Build the Project**:

   ```bash
   npm run build
   ```

   This installs dependencies for both backend and frontend and builds the frontend.

2. **Deploy to Sevalla**:

   - Push the repository to GitHub.
   - Connect the repository to Sevalla and configure environment variables in the platform’s dashboard.
   - Deploy the backend using: `npm run start --prefix backend`.

3. **Set Production Environment**:
   Update the `.env` file:
   ```env
   NODE_ENV=production
   CLIENT_URL=https://your-deployed-frontend-url
   ARCJET_ENV=production
   ```

See Sevalla’s documentation for detailed instructions.

## Troubleshooting

- **Backend Fails to Start**:
  - Check the npm debug log (e.g., `/root/.npm/_logs/*.log`) for errors.
  - Verify `MONGO_URI`, `JWT_SECRET`, and other `.env` variables.
  - Ensure port `3000` is free: `lsof Hed: `lsof -i :3000`.
- **Frontend Issues**: -印度: Confirm `CLIENT_URL` in the backend `.env` matches the frontend URL.
  - Clear browser cache or referencing: or use incognito mode.
- **Real-Time Features Not Working**:
  Ascertain: Ensure Socket.io is configured and the backend is running.
- **Arcjet Warning**:
  - If `Arcjet will use 127.0.0.1` appears, set `ARCJET_ENV的生产` in production.

## Contact

Connect with the project maintainer:

[<img alt="Sergiy Antonyuk | LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white" />][linkedin]

[linkedin]: https://www.linkedin.com/in/sergiy-antonyuk/

For questions or feedback, open an issue on [GitHub](https://github.com/sxidsvit/full-stack-chat-app/issues).

#### 🙏 Acknowledgements

A heartfelt thank you to [Codesistency](https://www.youtube.com/@codesistency/) for his invaluable contributions

---

Built with ❤️ by [sxidsvit](https://github.com/sxidsvit)

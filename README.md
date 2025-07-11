# Truck Border Clearance System

This project consists of a Node.js/Express backend and a modern HTML frontend for managing truck border clearance, user accounts, and admin capabilities.

---

## 🚀 Hosting Guide

### 1. **Frontend: Host on GitHub Pages**

- Place your `index.html` (from this repo, version 11) and any static files in the root of your repository.
- In your repository, go to **Settings > Pages** and set the source to the `main` branch and root (`/`).
- Your static site will be available at:  
  `https://<your-username>.github.io/<repo-name>/`

**Important:**  
You must update `index.html` so all API URLs (e.g. `API_URL`, `USER_API_URL`) point to your deployed backend server, NOT `localhost`.

Example:
```js
const API_URL = 'https://your-backend-service.onrender.com/api/records';
const USER_API_URL = 'https://your-backend-service.onrender.com/api/users';
```

---

### 2. **Backend: Host on a Node.js Platform**

You cannot host the server on GitHub Pages.
Use a service like [Render](https://render.com), [Railway](https://railway.app), [Heroku](https://heroku.com), or [Vercel](https://vercel.com).

#### **Deploy steps (Render example):**

1. Push your `server.js` (from version 6 below) to a public GitHub repo.
2. Go to [Render.com](https://render.com) and select "Web Service" -> "Connect a Repository".
3. Select your repo and set the root file to `server.js`.
4. Set the environment to Node.js, and the start command to `node server.js`.
5. Deploy.

Your backend will be available at e.g. `https://truck-border-clearance.onrender.com`.

---

## 🛠️ Files

### `server.js` (Node backend - version 6)
Paste the following into your server project:

```javascript
// (see below for full server.js code)
```

### `index.html` (Frontend - version 11)
Paste the following as `index.html` in your repo:

```html
// (see below for full index.html code)
```

---

## 🔑 Admin Account

- Username: `admin`
- Password: `admin 1`

---

## 📢 Notes

- **GitHub Pages cannot run Node.js/Express servers.**
- **Frontend and backend must be deployed separately.**
- **Update API URLs in `index.html` to point to your backend.**
- **For file backup features, your backend must have write permissions to the backup path.**
- **For production, you should use a database instead of in-memory stores.**

---

## 💬 Questions?

Open an issue in this repo!

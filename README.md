# 🔗 URL Shortener

A modern full-stack URL Shortener application built with React, Node.js, Express, and MongoDB. Users can transform long URLs into short, shareable links, generate QR codes, and quickly access links through QR scanning.

---

## ✨ Features

* 🔗 Shorten long URLs into unique short links
* 🚀 Instant redirection to the original URL
* 📱 Generate QR codes for every shortened URL
* ⬇️ Download QR codes as PNG images
* 📊 Track click counts for shortened links
* 🎨 Responsive UI built with Tailwind CSS & DaisyUI
* ⚡ Fast frontend powered by Vite

---

## 🛠️ Tech Stack

### Frontend

* React
* Vite
* Axios
* Tailwind CSS
* DaisyUI
* react-qr-code
* qrcode

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* NanoID
* dotenv
* CORS

---

## 📁 Project Structure

```text
url-shortener/
├── backend
│   ├── models
│   │   └── Url.js
│   ├── routes
│   │   └── url.js
│   ├── package.json
│   └── server.js
│
└── frontend
    ├── public
    │   ├── favicon.svg
    │   └── icons.svg
    ├── src
    │   ├── App.jsx
    │   ├── index.css
    │   └── main.jsx
    ├── index.html
    ├── package.json
    └── vite.config.js
```

---

## ⚙️ Environment Variables

### Backend (.env)

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
BASE_URL=http://localhost:5000
FRONTEND_URL=http://localhost:5173
```

### Frontend (.env)

```env
VITE_BACKEND_URL=http://localhost:5000
```

---

## 🚀 Installation & Setup

### 1. Clone Repository

```bash
git clone https://github.com/your-username/url-shortener.git
cd url-shortener
```

### 2. Setup Backend

```bash
cd backend
npm install
npm run dev
```

### 3. Setup Frontend

```bash
cd frontend
npm install
npm run dev
```

---

## 📡 API Endpoints

### Create Short URL

```http
POST /shorten
```

Request Body:

```json
{
  "originalUrl": "https://example.com"
}
```

Response:

```json
{
  "shortId": "abc1234",
  "shortUrl": "http://localhost:5000/abc1234",
  "originalUrl": "https://example.com",
  "clicks": 0
}
```

### Redirect to Original URL

```http
GET /:shortId
```

Redirects the user to the original URL and updates the click count.

---

## 📸 Screenshots

Add screenshots here after completing the UI.

```md
![Homepage](./screenshots/homepage.png)
```

---

## 🌐 Deployment

Deployment links will be added after hosting the project.

Planned Services:

* Frontend → Vercel
* Backend → Render
* Database → MongoDB Atlas

---

## 🔮 Future Improvements

* User Authentication
* Custom Short URLs
* Analytics Dashboard
* URL Expiration Support
* User URL History
* Copy Link Statistics

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome.

Feel free to fork the repository and submit a pull request.

---

## 📄 License

This project is licensed under the MIT License.

---

⭐ If you found this project helpful, consider giving it a star on GitHub.

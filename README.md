
# 🖼️ Imagify - AI Image Generator from Text Prompts

**Imagify** is a full-stack application that lets users generate stunning images from text prompts using the powerful Clipdrop API. Built with a React frontend and Node.js backend, it provides a clean and user-friendly interface to transform imagination into visuals.

---


## 🚀 Features

- ✨ Generate high-quality images from text prompts using Clipdrop API
- ⚛️ React-based frontend for a smooth user experience
- 🔧 Node.js/Express backend to handle API requests securely
- 📁 History of generated images (optional feature)
- 🌐 Responsive design for mobile and desktop
- 💰 (Optional) Credit-based system or API usage limit

---

## 📊 Sequence Diagram - Imagify

```mermaid
sequenceDiagram
    participant U as User
    participant F as Frontend (React)
    participant B as Backend (Node.js)
    participant C as Clipdrop API

    U->>F: Enter text prompt
    F->>B: POST /api/generate { prompt }
    B->>C: Send prompt to Clipdrop API
    C-->>B: Return generated image URL
    B-->>F: Send image URL
    F-->>U: Display generated image
```

---

## 🧰 Tech Stack

| Frontend     | Backend      | API/Services    |
|--------------|--------------|-----------------|
| React.js     | Node.js      | Clipdrop API    |
| Axios        | Express.js   | dotenv          |
| Tailwind CSS | CORS         | Vercel / Render |

---

## 📸 Demo

[Watch the demo](https://drive.google.com/file/d/19D3t-t6xzSqgMHG-1iv9WeZ7zSNI1HDL/view)

---

## ⚙️ Installation

### 1. Clone the Repository
```bash
git clone https://github.com/nandhan7/imagify.git
cd imagify
```

### 2. Set Up Backend
```bash
cd backend
npm install
# Create a .env file and add your Clipdrop API key
echo "CLIPDROP_API_KEY=your_api_key_here" > .env
npm start
```

### 3. Set Up Frontend
```bash
cd ../frontend
npm install
npm start
```

---

## 🌐 API Usage (Backend)

The backend exposes a single POST route:

```
POST /api/generate
Body: {
  prompt: "a futuristic cityscape at night"
}
```

The server sends the prompt to the Clipdrop API and returns the generated image URL.

---

## 📁 Project Structure

```
imagify/
│
├── frontend/          # React app
│   ├── src/
│   ├── public/
│   └── ...
│
├── backend/           # Node.js server
│   ├── routes/
│   ├── controllers/
│   └── ...
```

---

## 🛡️ Environment Variables

Create a `.env` file in the `backend/` directory:

```env
CLIPDROP_API_KEY=your_clipdrop_api_key
```

---

## 💡 Future Enhancements

- User authentication and image history
- Download/share generated images
- Multiple image styles (e.g., anime, photorealistic)
- API usage tracking

---

## 🙌 Acknowledgements

- [Clipdrop API](https://clipdrop.co/apis) for image generation
- [React.js](https://react.dev/)
- [Express.js](https://expressjs.com/)
- [Tailwind CSS](https://tailwindcss.com/)

---

## 📄 License

MIT License. Feel free to use and modify!

---

## 🤝 Connect

Built with ❤️ by [B V Nandhan](https://github.com/nandhan7)

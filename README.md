# 🧠 Hand-Drawn Symbol Recognition Tool (React + Node.js + HuggingFace)

This is a simple web-based image recognition tool that allows users to upload or draw hand-drawn shapes (like **circle**, **triangle**, **star**) and identifies them using a free image classification model from **Hugging Face**.

---

## 🚀 Features

- Upload hand-drawn symbols like circle, triangle, star.
- Recognize symbols using a public deep learning model (`microsoft/resnet-50`) via HuggingFace Inference API.
- Built with:
  - 🖼️ React (frontend)
  - 🌐 Node.js + Express (backend)
  - 🤖 HuggingFace ResNet model (image classification)

---

## 🖥️ Demo

Upload a hand-drawn image, and the app will return a prediction of what shape it recognizes.

![demo-gif](demo.gif) <!-- Optional: Add a demo GIF here -->

---

## 📁 Project Structure

symbol-recognition-app/
├── client/ # React frontend
│ └── src/App.js # Image uploader UI
├── server/ # Node.js backend
│ └── index.js # Express server with HuggingFace proxy
├── uploads/ # Temporary image uploads
├── README.md

yaml
Copy
Edit

---

## 🛠️ Installation & Usage

### Prerequisites

- Node.js >= 14
- npm or yarn

---

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/symbol-recognition-app.git
cd symbol-recognition-app
2. Start the backend server
bash
Copy
Edit
cd server
npm install
node index.js
Server will start on: http://localhost:5000

3. Start the frontend (React app)
Open another terminal:

bash
Copy
Edit
cd client
npm install
npm start
App will run on: http://localhost:3000

###
🔗 API Usage
The backend proxies requests to:

ruby
Copy
Edit
https://api-inference.huggingface.co/models/microsoft/resnet-50
No authentication is needed for small usage, but you can use a free Hugging Face token if rate-limited.

✏️ Future Improvements
Add drawing canvas (instead of upload)

Train custom model using Roboflow or Teachable Machine

Add confidence thresholds

Host on Vercel + Render/Heroku for live demo

📄 License
MIT License

🤝 Contributing
Pull requests are welcome! Feel free to open an issue if you want to suggest a feature or report a bug.

🧑‍💻 Author
Swastik Ranjan

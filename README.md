Here’s an updated `README.md` file that includes the **Flask backend (`app.py`)** along with the **React CAD Viewer** setup.

---

```markdown
# CAD Viewer

A full-stack **CAD Viewer** that allows users to upload and visualize **3D CAD models** in a web browser.  
Built using **React Three Fiber** for 3D rendering and **Flask** as the backend for file uploads.

## 🚀 Features
- **Upload CAD models** (STL, OBJ, etc.)
- **View & interact** with models in 3D
- **Orbit, zoom, and pan controls**
- **Fast & responsive UI** using Tailwind CSS
- **Backend for file storage** with Flask

---

## 📦 Installation & Setup

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/your-username/cad-viewer.git
cd cad-viewer
```

### 2️⃣ Setup & Run the **Backend** (Flask)
#### 📌 Install dependencies
```sh
cd backend
pip install -r requirements.txt
```
#### 📌 Start the Flask server
```sh
python app.py
```
The server will run at `http://127.0.0.1:5000/`.

---

### 3️⃣ Setup & Run the **Frontend** (React)
#### 📌 Install dependencies
```sh
cd ../cad-viewer
npm install
```
#### 📌 Start the React development server
```sh
npm start
```
The React app runs on `http://localhost:3000/`.

---

## 📂 Project Structure
```
cad-viewer/
│            # Flask API
│├── uploads/           # Uploaded CAD models
│├── app.py             # Flask server
│├── requirements.txt   # Python dependencies
│── cad-viewer/              # React App
│   ├── src/
│   │   ├── components/    # 3D components
│   │   ├── styles/        # Tailwind CSS styles
│   │   ├── App.js         # Main component
│   │   ├── index.js       # React entry point
│── README.md              # Documentation
```

---

## 🛠 Tech Stack
### **Frontend**
- **React** + **Three.js** + **@react-three/fiber**
- **@react-three/drei** (for camera controls, loaders)
- **Axios** (for API communication)
- **Tailwind CSS** (for styling)

### **Backend**
- **Flask** (Python)
- **Flask-CORS** (for cross-origin requests)
- **File storage** for CAD models

---

## 🎨 Usage
1. **Upload a CAD model** (`.glb`, `.obj`).
2. **View & interact** with the 3D model.
3. **Pan, zoom, and rotate** the model in the scene.

---

## 🎯 API Endpoints
### 🔹 **Upload File**
**Endpoint:** `POST /upload`  
**Description:** Uploads a CAD model.  
**Request:** FormData with `file` field  
**Response:**
```json
{
  "message": "File uploaded successfully",
  "filename": "model.glb"
}
```

### 🔹 **Retrieve File**
**Endpoint:** `GET /models/<filename>`  
**Description:** Fetches the uploaded model file.  
**Response:** Returns the file if it exists.

---

## 🤝 Contributing
1. **Fork the repo**
2. **Create a new branch**
3. **Make changes & commit**
4. **Submit a pull request**

---


---



---

### ✅ **Next Steps**
- **Add file type validation** (only allow `.glb`, `.obj`)
- **Improve UI** for uploading & model selection
- **Deploy Flask & React app**

Let me know if you need modifications! 🚀

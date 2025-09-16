# 🎓 PresenZ – AI-Powered Face Recognition Attendance System  

PresenZ is an advanced **deep learning-based attendance system** that uses real-time **facial recognition** to automatically mark attendance.  
It eliminates manual roll calls by detecting, identifying, and logging individuals with high accuracy.  

✨ Built with **YOLOv8**, **DeepFace**, **OpenCV**, and **Flask**, PresenZ provides both **backend intelligence** and a **web-based UI**.  

---

## 🚀 Features  

- 📷 **Real-time Detection** – Tracks faces live from CCTV / webcam / video feed  
- 🤖 **Face Recognition** – Identifies individuals using **DeepFace embeddings**  
- 🗂️ **Attendance Logs** – Exports clean CSV files with name + timestamp  
- ⚡ **Optimized Pipeline** – YOLOv8 detection + DeepFace caching for speed  
- 🌐 **Web UI (Flask + HTML/CSS/JS)** – Simple dashboard to start/stop tracking and view attendance  
- 🔒 **Duplicate Prevention** – Each person is marked *Present* only once  

---

## 🛠️ Tech Stack  

| Module       | Purpose                              |  
|--------------|--------------------------------------|  
| YOLOv8       | High-speed face detection            |  
| DeepFace     | Face embeddings + identity matching  |  
| OpenCV       | Video I/O, bounding boxes, overlays  |  
| Flask        | Web backend + API for UI             |  
| HTML/CSS/JS  | Frontend dashboard for users         |  
| Pandas/Numpy | Data handling + CSV generation       |  

---

## 📂 Project Structure  

```bash
PresenZ/
│── core1.py                # YOLO + DeepFace pipeline  
│── core1_improved.py       # Optimized pipeline (faster, frame skipping)  
│── deep_track_prototype.py # Webcam-based demo  
│── templates/              # HTML files for Flask UI  
│── static/                 # CSS/JS assets for UI  
│── known_faces/            # Database of registered faces  
│── attendance/             # Output attendance CSVs  
│── output/                 # Annotated videos  
│── yolov11l-face.pt        # YOLOv8 large model  
│── yolov11n-face.pt        # YOLOv8 nano model  
│── requirements.txt        # Dependencies  
│── README.md               # Project documentation  

```

## ⚡ Setup Instructions  

### 1️⃣ Clone the repo  
```bash
git clone https://github.com/<your-username>/PresenZ.git
cd PresenZ
```

### 2️⃣ Create virtual environment (Windows)
``` bash
python -m venv venv
venv\Scripts\activate
```

### 3️⃣ Install dependencies
``` bash
pip install -r requirements.txt
pip install flask opencv-python-headless deepface
```

### 4️⃣ Download YOLO weights
Place yolov11l-face.pt and yolov11n-face.pt inside the project root folder.

### 5️⃣ Run Flask UI
``` bash
python app.py
```

👉 Visit http://127.0.0.1:5000
 in your browser.

📊 Sample Attendance Log

final_attendance.csv
Name,Time
Shankar Singh,2025-07-12 09:43:21
Anurag Singh,2025-07-12 09:44:12

🔮 Future Scope

🌍 Multi-camera support for large classrooms

🖥️ Admin dashboard for attendance analytics

🛡️ Liveness detection to prevent spoofing

📱 Mobile-friendly interface

👨‍💻 Team PresenZ

🧑‍💻 [Your Name] – Full Stack & UI

🧑‍💻 [Teammate] – Deep Learning & Model Integration

🧑‍💻 [Teammate] – Backend & Database

📧 Contact us: team.presenz@gmail.com

⚡ PresenZ – Making attendance smart, fast, and effortless!


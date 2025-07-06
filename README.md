# Endangered Species Detection and Prevention

A full-stack web application that detects and analyzes endangered species using **YOLO object detection**. The app provides detailed information about detected animals including their habitat, conservation status, threats, and protection measures.

🚀 **Live Demo:** [endangerdspecies.netlify.app](https://endangerdspecies.netlify.app/)

---

## 🌟 Features

- ✅ Real-time object detection using YOLO
- 📊 Detailed information for detected animals:
  - Class, population, physical attributes
  - Habitat details
  - Conservation status
  - Threats and protection strategies
- 🖼️ Visual detection results with bounding boxes
- 📱 Responsive, modern UI built with React

---

## 🗂️ Project Structure

```
yolo-detection-app/
├── backend-api/
│   ├── app.py              # Flask backend server
│   ├── animal_data.py      # Animal information database
│   ├── requirements.txt    # Python dependencies
│   └── best_model.pt       # YOLO model weights
└── src/
    ├── App.js              # Main React component
    └── App.css             # Frontend styling
```

---

## 📦 Dataset Used

This project uses a Pascal VOC-style annotated dataset converted to **YOLOv4 Darknet** format, hosted on [Roboflow](https://roboflow.com).

- 📁 **Dataset Name:** Pascal to YOLOv4 Darknet  
- 🔗 **Access Link:** [Roboflow Dataset – Pascal to YOLOv4 Darknet (v3)](https://universe.roboflow.com/patrick-aaiqr/pascal-to-yolov4-darknet/dataset/3)
- 🧾 **Annotations Format:** YOLOv4 (Darknet TXT files)
- 🐾 **Use Case:** Object detection of animals for endangered species classification
- 📊 Includes classes, bounding boxes, and image preprocessing tools

To use this dataset:
1. Download the ZIP from the Roboflow dataset page (linked above)
2. Unzip it into your working directory
3. Train or test using the `best_model.pt` after proper training

---

## ⚙️ Setup & Installation

### 🔧 Backend Setup (Flask)

1. **Create a virtual environment**
   ```bash
   python -m venv venv
   ```

2. **Activate the virtual environment**
   - **Windows**
     ```bash
     venv\Scripts\activate
     ```
   - **macOS/Linux**
     ```bash
     source venv/bin/activate
     ```

3. **Install dependencies**
   ```bash
   cd backend-api
   pip install -r requirements.txt
   ```

4. **Add YOLO model weights**
   Place your trained YOLO model file (`best_model.pt`) inside the `backend-api/` directory.

5. **Run the Flask server**
   ```bash
   python app.py
   ```

---

### 🎨 Frontend Setup (React)

1. **Install dependencies**
   ```bash
   npm install
   ```

2. **Start development server**
   ```bash
   npm start
   ```

> 🖥️ The app will be running at:
> - Frontend: [http://localhost:3000](http://localhost:3000)
> - Backend API: [http://localhost:5000](http://localhost:5000)

---

## 📡 API Endpoints

| Endpoint         | Method | Description                           |
|------------------|--------|---------------------------------------|
| `/process`       | POST   | Processes uploaded image for detection |
| `/get_image`     | GET    | Returns the processed image with detections |

---

## 🛠️ Technologies Used

### Backend:
- Python
- Flask
- OpenCV
- PyTorch
- YOLO (Ultralytics)

### Frontend:
- React.js
- Modern CSS

---

## 🤝 Contributing

We welcome contributions! Here's how:

1. **Fork** this repository
2. **Create** a new feature branch:
   ```bash
   git checkout -b feature/YourFeatureName
   ```
3. **Commit** your changes:
   ```bash
   git commit -m "Add your message here"
   ```
4. **Push** to your branch:
   ```bash
   git push origin feature/YourFeatureName
   ```
5. **Open** a Pull Request

---

## 📷 Screenshot

![example](https://github.com/user-attachments/assets/4e383d67-bf2c-434f-983c-16eab1e5b7ab)



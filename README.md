

# Face Recognition Attendance System

## Project Overview
This is an automated attendance management system using face recognition technology. The project leverages computer vision and machine learning to streamline the attendance tracking process for educational institutions or workplaces.


## Features
- Real-time face detection
- Face recognition and identification
- Automated attendance logging
- Easy-to-use interface
- Secure and accurate attendance tracking

## Prerequisites
- Python 3.8+
- OpenCV
- face_recognition library
- NumPy
- Pandas

## Installation

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/face-recognition-attendance.git
cd face-recognition-attendance
```

### 2. Create Virtual Environment
```bash
python -m venv attendanceenv
# Activate the virtual environment
# Windows
attendanceenv\Scripts\activate
# macOS/Linux
source attendanceenv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

## Project Structure
```
face-recognition-attendance/
│
├── main.py               # Main application script
├── face_recognition.py   # Face detection and recognition logic
├── database.py           # Database management
├── attendance_log.csv    # Attendance records
│
├── known_faces/          # Directory for storing known face encodings
│   ├── employee1.jpg
│   ├── employee2.jpg
│   └── ...
│
└── requirements.txt      # Project dependencies
```

## Configuration

### Known Faces
1. Add clear, front-facing images of individuals to the `known_faces/` directory
2. Ensure images are named appropriately (e.g., `john_doe.jpg`)

### Attendance Log
- Attendance is automatically logged in `attendance_log.csv`
- Format includes:
  - Timestamp
  - Name
  - Employee/Student ID
  - Status

## Usage

### Running the Application
```bash
python main.py
```

### Command Line Options
```
python main.py --mode [train/recognize]
  --mode train    : Prepare face encodings
  --mode recognize: Start attendance recognition
```

## Technical Details

### Face Recognition Process
1. Load known face encodings
2. Capture live video feed
3. Detect faces in each frame
4. Compare detected faces with known encodings
5. Log attendance for matched individuals

### Accuracy Considerations
- Recommended lighting: Well-lit environments
- Camera quality: HD webcam (720p+)
- Face angle: Preferably front-facing

## Troubleshooting

### Common Issues
- **No faces detected**: 
  - Ensure proper lighting
  - Check camera positioning
  - Verify image quality in `known_faces/`

- **Installation Problems**:
  ```bash
  # Reinstall dependencies
  pip install --upgrade pip
  pip install -r requirements.txt
  ```

## Security Notes
- Store face encoding files securely
- Implement access controls
- Comply with data protection regulations

## Future Improvements
- Machine learning model for improved recognition
- Multi-camera support
- Cloud-based attendance tracking
- Advanced analytics

## Contributing
1. Fork the repository
2. Create your feature branch
3. Commit changes
4. Push to the branch
5. Create a Pull Request



## Contact
Himani Chunduru
himani3366@gmail.com

---


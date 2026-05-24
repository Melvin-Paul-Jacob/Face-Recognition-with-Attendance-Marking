# Face Recognition with Attendance Marking

An automated attendance management system powered by Computer Vision and Face Recognition. The system detects and recognizes registered individuals in real time using a webcam and automatically records attendance, eliminating the need for manual attendance tracking.

## Features

- Real-time face detection using OpenCV
- Face recognition of registered users
- Automatic attendance marking
- CSV-based attendance logging
- Duplicate attendance prevention
- Fast and lightweight implementation
- Easy enrollment of new users
- Simple and intuitive workflow

## Project Workflow

1. **Register Faces**
   - Capture images of individuals.
   - Store and organize training data.

2. **Encode Face Features**
   - Generate facial embeddings from registered images.
   - Save encodings for future recognition.

3. **Real-Time Recognition**
   - Capture video stream from webcam.
   - Detect faces in each frame.
   - Compare detected faces against stored encodings.

4. **Attendance Marking**
   - Identify recognized individuals.
   - Record name, date, and timestamp.
   - Prevent multiple entries for the same person on the same day.

## Tech Stack

- Python
- OpenCV
- NumPy
- Face Recognition Library
- Pandas
- CSV File Handling

## Directory Structure

```text
Face-Recognition-with-Attendance-Marking/
│
├── ImagesAttendance/        # Registered face images
├── Attendance.csv           # Attendance records
├── main.py                  # Main application
├── requirements.txt         # Dependencies
└── README.md
```

## Usage

### Add New Users

1. Place images of individuals inside the `ImagesAttendance` folder.
2. Use the person's name as the image filename.

Example:

```text
ImagesAttendance/
├── John_Doe.jpg
├── Alice_Smith.jpg
└── Bob_Jones.jpg
```

### Run the Application

```bash
python main.py
```

### Attendance Recording

When a registered face is detected:

- Name is identified
- Current date is recorded
- Timestamp is stored
- Attendance is appended to `Attendance.csv`

Example:

```csv
Name,Time
John Doe,09:02:15
Alice Smith,09:05:31
```

## Applications

- Educational Institutions
- Corporate Attendance Systems
- Research Laboratories
- Training Centers
- Access Monitoring Systems
- Smart Office Solutions

## Future Improvements

- Database integration (MySQL/PostgreSQL)
- Web dashboard for attendance analytics
- Anti-spoofing and liveness detection
- Multi-camera support
- Cloud synchronization
- Face mask recognition support
- Employee/student management portal

## Performance

- Real-time face detection and recognition
- Low computational overhead
- Scalable for small to medium-sized deployments
- High recognition accuracy under proper lighting conditions

---

If you found this project useful, consider giving it a ⭐ on GitHub.

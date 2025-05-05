# FaceMark Attendance

A Python-based attendance system that uses face recognition to automatically mark attendance of students/employees. The system captures images through a webcam, recognizes faces, and marks attendance in a CSV file.

## Features

- Face detection and recognition
- Real-time attendance marking
- Student/Employee profile management
- Password protection for admin functions
- CSV export of attendance records
- Simple and intuitive GUI interface

## Prerequisites

- Python 3.7 or higher
- Webcam
- Required Python packages (listed in requirements.txt)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/face-recognition-attendance-system.git
cd face-recognition-attendance-system
```

2. Create and activate a virtual environment:
```bash
# Windows
python -m venv .venv
.venv\Scripts\activate

# Linux/Mac
python3 -m venv .venv
source .venv/bin/activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

## Project Structure

```
face-recognition-attendance-system/
├── main.py                 # Main application file
├── test.py                # Test file
├── haarcascade_frontalface_default.xml  # Face detection model
├── TrainingImage/         # Directory for storing face images
├── TrainingImageLabel/    # Directory for storing training data
├── StudentDetails/        # Directory for student information
└── Attendance/           # Directory for attendance records
```

## Setup Instructions

1. Run the main application:
```bash
python main.py
```

2. First-time setup:
   - Set up an admin password when prompted
   - The system will create necessary directories automatically

3. Adding new students/employees:
   - Click on "Take Images" button
   - Enter ID and Name
   - Look at the camera to capture face images
   - Click "Save Profile" to train the system

4. Taking attendance:
   - Click on "Take Attendance" button
   - The system will automatically detect faces and mark attendance
   - Attendance records are saved in the Attendance directory

## Directory Structure Setup

The following directories will be created automatically when you run the application:

- `TrainingImage/`: Stores captured face images
- `TrainingImageLabel/`: Stores training data and password file
- `StudentDetails/`: Stores student information in CSV format
- `Attendance/`: Stores attendance records in CSV format

## Security Notes

- The system uses password protection for administrative functions
- Face images and personal information are stored locally
- Regular backups of the data are recommended

## Troubleshooting

1. If the webcam is not detected:
   - Check if the webcam is properly connected
   - Ensure no other application is using the webcam
   - Try restarting the application

2. If face detection is not working:
   - Ensure proper lighting conditions
   - Check if the face is clearly visible
   - Verify that the haarcascade file is present

3. If the application crashes:
   - Check if all required directories exist
   - Verify that all dependencies are installed
   - Check the console for error messages

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the GNU L3 License - see the LICENSE file for details.

## Contact

For support or queries, please open an issue in the GitHub repository.


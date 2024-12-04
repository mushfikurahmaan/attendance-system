attendance_system/
├── images/                          # Folder to store training images of known faces
│   ├── friend_name/                 # Folder for each person
│   │   ├── image_1.jpg              # Multiple images of the same person
│   │   ├── image_2.jpg
│   │   └── ...
│   ├── other_friend_name/
│   │   ├── image_1.jpg
│   │   ├── image_2.jpg
│   │   └── ...
│   └── ...
├── logs/                            # Centralized logs for debugging and tracking
│   ├── app.log                      # Logs for application activity (Flask, etc.)
│   ├── model.log                    # Logs for model training and recognition
│   ├── errors.log                   # Logs for errors and exceptions
│   ├── attendance_updates.log       # Logs attendance updates (timestamps, IDs)
│   └── webcam.log                   # Logs webcam activity (start, stop, detections)
├── app/                             # Main application folder for Flask
│   ├── __init__.py                  # Initialize Flask app
│   ├── routes.py                    # Web app routes (e.g., for attendance display)
│   ├── static/                      # Static files (CSS, JS, Images)
│   └── templates/                   # HTML templates for the web interface
│       ├── index.html               # Home page template
│       └── attendance.html          # Attendance display template
├── model/                           # Model-related scripts and files
│   ├── train_model.py               # Script to train and save face encodings
│   ├── recognize_face.py            # Script for real-time face recognition
│   ├── test_recognition.py          # NEW: Script to test the model
│   └── face_encodings.pkl           # Pickled file storing known face encodings
├── database/                        # Database folder
│   ├── attendance.db                # SQLite database storing attendance records
│   ├── create_db.py                 # Script to initialize database and tables
│   └── db_manager.py                # NEW: Utility for managing database operations
├── utils/                           # Utility scripts
│   ├── capture_images.py            # Script to capture and save images
│   ├── save_encodings.py            # Script to generate and save encodings
│   ├── logger.py                    # Logging utility for log management
│   └── config.py                    # NEW: Configuration settings
├── requirements.txt                 # List of required Python dependencies
├── setup.sh                         # NEW: Automated environment setup script
├── run.py                           # Main entry point for running the application
└── README.md                        # Project documentation

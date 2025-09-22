# Face-Based Employee Attendance System 🎯

An AI-powered employee attendance system using advanced face recognition technology. Built with Django, OpenCV, PyTorch, and facenet-pytorch for accurate and efficient attendance tracking.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Django](https://img.shields.io/badge/Django-5.0+-green.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-4.0+-red.svg)
![PyTorch](https://img.shields.io/badge/PyTorch-Latest-orange.svg)

## 🚀 Features

- **Smart Employee Registration**: Register employees with photo capture and facial data encoding
- **Real-time Face Recognition**: Live camera feed for instant attendance marking
- **Comprehensive Reporting**: Attendance history with CSV export functionality
- **Flexible Camera Support**: Works with webcams and IP cameras
- **Admin Dashboard**: Complete employee and attendance management system
- **Modern UI**: Responsive design with dark/light theme support
- **Security Features**: Employee authorization system with active/inactive status

## 🛠️ Technologies Used

- **Backend**: Python, Django 5.0+
- **Computer Vision**: OpenCV, PyTorch, facenet-pytorch
- **Database**: SQLite (development) / PostgreSQL (production)
- **Frontend**: HTML5, CSS3, JavaScript, Lucide Icons
- **Deployment**: Gunicorn, Whitenoise, Docker-ready

## 📋 Prerequisites

- Python 3.8 or higher
- pip (Python package manager)
- Git
- Camera (webcam or IP camera)

## ⚡ Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/face-attendance-system.git
cd face-attendance-system
```

### 2. Create Virtual Environment
```bash
python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Database Setup
```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Create Admin User
```bash
python manage.py createsuperuser
```

### 6. Run Development Server
```bash
python manage.py runserver
```

### 7. Access the Application
- **Main Application**: http://127.0.0.1:8000/
- **Admin Panel**: http://127.0.0.1:8000/admin/

## 🎯 Usage Guide

### Employee Registration
1. Navigate to "Student Registration"
2. Fill in employee details
3. Capture or upload a clear photo
4. System automatically extracts facial features

### Marking Attendance
1. Go to "Mark Attendance"
2. Allow camera access
3. Face will be automatically detected and recognized
4. Attendance is marked with timestamp

### Viewing Reports
1. Access "Attendance Log"
2. Filter by date, employee, or department
3. Export data as CSV for external analysis

### Camera Configuration
1. Go to "Camera Config"
2. Set up webcam or IP camera
3. Test camera feed before use

## 🚀 Deployment

### Heroku Deployment
```bash
# Install Heroku CLI
heroku create your-app-name
heroku config:set DEBUG=False
heroku config:set SECRET_KEY=your-secret-key
git push heroku main
heroku run python manage.py migrate
heroku run python manage.py createsuperuser
```

### Docker Deployment
```bash
docker build -t face-attendance .
docker run -p 8000:8000 face-attendance
```

## 🔧 Configuration

### Environment Variables
Create a `.env` file in the root directory:
```env
SECRET_KEY=your-secret-key-here
DEBUG=False
DB_NAME=your_db_name
DB_USER=your_db_user
DB_PASSWORD=your_db_password
```

### Camera Settings
- **Webcam**: Use index 0 for default camera
- **IP Camera**: Configure with camera URL in admin panel
- **Resolution**: Adjustable in camera configuration

## 🎨 Screenshots

| Home Dashboard | Employee Registration | Face Recognition |
|---|---|---|
| ![Dashboard](screenshots/dashboard.png) | ![Registration](screenshots/registration.png) | ![Recognition](screenshots/recognition.png) |

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **facenet-pytorch** for the excellent face recognition model
- **Django** for the robust web framework
- **OpenCV** for computer vision capabilities
- **Lucide** for beautiful icons

## 📞 Support

If you encounter any issues or have questions:
- Open an issue on GitHub
- Contact: [your-email@example.com]
- LinkedIn: [Your LinkedIn Profile]

## 🎯 Roadmap

- [ ] Mobile app integration
- [ ] Advanced analytics dashboard
- [ ] Multi-location support
- [ ] Integration with HR systems
- [ ] REST API development
- [ ] Real-time notifications

---

⭐ **Star this repository if you found it helpful!**

**Built with ❤️ by [Your Name]**

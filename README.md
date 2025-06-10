# Present Android - Machine Learning Deployment

Dự án triển khai các mô hình Machine Learning trên nền tảng Android, bao gồm 3 module chính:

## 📱 Modules

### 1. ImageGeneration
- **Mô tả**: Ứng dụng Android tích hợp mô hình sinh ảnh bằng AI
- **Công nghệ**: TensorFlow Lite, Android SDK
- **Tính năng**: Tạo ảnh từ văn bản hoặc từ input của người dùng

### 2. YOLO_Mobile  
- **Mô tả**: Ứng dụng nhận diện đối tượng real-time sử dụng YOLO
- **Công nghệ**: YOLO model, TensorFlow Lite, Camera2 API
- **Tính năng**: Phát hiện và nhận diện đối tượng trong thời gian thực

### 3. TransferLearningMobile
- **Mô tả**: Ứng dụng phân loại ảnh sử dụng Transfer Learning
- **Công nghệ**: Pre-trained models, TensorFlow Lite
- **Tính năng**: Phân loại ảnh dựa trên mô hình đã được train trước

## 🚀 Yêu cầu hệ thống

- **Android SDK**: API level 21+ (Android 5.0)
- **Android Studio**: 4.0 trở lên
- **Gradle**: 7.0+
- **Java**: JDK 11+
- **RAM**: Tối thiểu 4GB khuyến nghị 8GB

## 📋 Cài đặt và chạy dự án

### Bước 1: Clone repository
```bash
git clone <repository-url>
cd Present_Android
```

### Bước 2: Mở project trong Android Studio
1. Mở Android Studio
2. Chọn "Open an Existing Project"
3. Chọn thư mục của module bạn muốn chạy:
   - `ImageGeneration/`
   - `YOLO_Mobile/`
   - `TransferLearningMobile/`

### Bước 3: Sync project
- Android Studio sẽ tự động sync Gradle
- Đợi quá trình download dependencies hoàn tất

### Bước 4: Chạy ứng dụng
1. Kết nối thiết bị Android hoặc khởi động emulator
2. Chọn module muốn chạy
3. Nhấn "Run" hoặc Shift+F10

## 🔧 Cấu hình

### Dependencies chính
- TensorFlow Lite
- Camera2 API
- OpenCV (cho xử lý ảnh)
- Material Design Components

### Models
- Các mô hình ML được lưu trong thư mục `assets/` của mỗi module
- Format: `.tflite` để tối ưu cho mobile

## 📚 Cấu trúc dự án

```
Present_Android/
├── ImageGeneration/          # Module sinh ảnh AI
├── YOLO_Mobile/             # Module nhận diện đối tượng
├── TransferLearningMobile/  # Module phân loại ảnh
├── .gitignore              # Loại trừ file không cần thiết
└── README.md               # File này
```

## 🎯 Tính năng chính

### ImageGeneration
- [x] Sinh ảnh từ text prompt
- [x] Giao diện người dùng thân thiện
- [x] Lưu ảnh đã tạo
- [x] Share ảnh lên social media

### YOLO_Mobile
- [x] Real-time object detection
- [x] Hiển thị bounding box và confidence score
- [x] Hỗ trợ nhiều class đối tượng
- [x] Chụp ảnh với detection results

### TransferLearningMobile
- [x] Phân loại ảnh từ camera
- [x] Phân loại ảnh từ gallery
- [x] Hiển thị confidence score
- [x] Top-5 predictions

## 🛠️ Phát triển

### Thêm model mới
1. Convert model sang format `.tflite`
2. Đặt file trong `assets/`
3. Cập nhật code load model trong MainActivity

### Custom training
- Sử dụng transfer learning với TensorFlow
- Export model sang TensorFlow Lite
- Test trên mobile device

## 📱 Screenshots

(Thêm screenshots của các ứng dụng ở đây)

## 🤝 Đóng góp

1. Fork repository
2. Tạo feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Mở Pull Request

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

## 📞 Liên hệ

- **Email**: dattq.b21cn222@stu.ptit.edu.vn
- **GitHub**: [quydatsadboy](https://github.com/quydatsadboy)

## 🙏 Acknowledgments

- TensorFlow team cho TensorFlow Lite
- Google cho Android ML Kit
- OpenCV community
- YOLO authors

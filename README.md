# FACE DECTECTION WITH DNN
## Đề tài sáng tạo khởi nghiệp Naver - Ptit
Tên đề tài: "Xây dựng hệ thống đo thân nhiệt tự động ứng dụng AI"

Thực hiện bởi: Information Network Lab (PTIT)

## Tổng quan
### Phần cứng
- Raspberry Pi 4
- Camera nhiệt MX...
- Cam thường
### Thuận toán
- Sử dụng các thuật toán nhẹ, nhận diện tốt như Haar Cascade, DNN,.. Để nhận diện khuôn mặt
### Kịch bản
- Các ảnh, video đầu vào cam thường được ứng dụng thuật toán DNN để nhận diện khuôn mặt, đóng khung khuôn mặt và đưa ra vị trí của khung
- Từ tọa độ đầu ra, áp dụng vào cam nhiệt để nhận diện vùng cần đo nhiệt
- Sau khi có được vùng cần đo thì nhiệt độ trung bình của mỗi người sẽ bằng trung bình cộng của tất cả các điểm nhiệt trên khuôn mặt

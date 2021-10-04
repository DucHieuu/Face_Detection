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
- Sử dụng các thuật toán nhẹ, phản hồi nhanh, phù hợp với phần cứng như Haar Cascade, DNN,.. để nhận diện khuôn mặt
### Kịch bản
- Các ảnh, video đầu vào cam thường được ứng dụng thuật toán DNN để nhận diện khuôn mặt, đóng khung khuôn mặt và đưa ra vị trí của khung
- Từ tọa độ đầu ra, áp dụng vào cam nhiệt để nhận diện vùng cần đo nhiệt
- Sau khi có được vùng cần đo thì nhiệt độ trung bình của mỗi người sẽ bằng trung bình cộng của tất cả các điểm nhiệt trên khuôn mặt
### Hình ảnh minh họa
![image](https://user-images.githubusercontent.com/71936544/135860458-7372b95b-cf63-403a-9f05-9f176f321a9d.png)
![image](https://user-images.githubusercontent.com/71936544/135860308-5e055221-1657-4dc6-9bb4-8f60140bf474.png)

## Chú thích
- `detect_face.py` `detect_face_video.py` : Phát hiện khuôn mặt dựa trên thuật toán DNN
- `deploy.prototxt.txt` `res10_300x300_ssd_iter_140000.caffemodel` : Model cần có khi sử dụng thuật toán DNN
- `haar_face_detector.py`: Phát hiện khuôn mặt sử dụng thuật toán Haar Cascade
- `haarcascade_frontalface_default.xml`: Model cần có khi sử dụng Haar Cascade
## Tài liệu tham khảo:
- [pyimagesearch](https://www.pyimagesearch.com/2018/02/26/face-detection-with-opencv-and-deep-learning/)

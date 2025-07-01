BÁO CÁO KIỂM THỬ HIỆU SUẤT JMETER
Tên Dự Án: Load Testing of Web Pages
Ngày Kiểm Thử: 01/07/2025
Người Kiểm Thử: Nguyễn Văn B
1. Mục Tiêu Kiểm Thử
Sử dụng JMeter để kiểm tra hiệu năng của các trang web khác nhau dưới tải khác nhau.
2. Môi Trường Kiểm Thử

Công cụ: Apache JMeter (phiên bản mới nhất).
Hệ điều hành: Windows 10.
Cấu hình máy: CPU Intel Core i5, RAM 8GB.

3. Phương Pháp Kiểm Thử
Kiểm thử tự động thông qua JMeter với các yêu cầu HTTP được cấu hình cho từng trang web.
4. Kịch Bản Kiểm Thử
Kịch Bản Kiểm Thử Lần 1
Tên Kịch Bản: Kiểm thử cơ bản trang "Simplilearn"
Mục Đích: Đánh giá hiệu năng của trang www.simplilearn.com với một người dùng duy nhất.
HTTP Request: www.simplilearn.com
Tham Số: Không có tham số bổ sung
Số lượng Thread (Người dùng): 1
Ramp-up Period (Giây): 1
Loop Count: 1
Kết Quả Mong Đợi: Gửi yêu cầu HTTP thành công.
Kết Quả Thực Tế: Yêu cầu được gửi thành công (xem View Results Tree).
Trạng Thái: Thành công
Kết Quả Sau Khi Test:
![image](https://github.com/user-attachments/assets/49414353-1aa9-4d95-aafc-7abb14ae2465)

Thời gian phản hồi trung bình: 6 giây
Tỷ lệ yêu cầu thành công: 100%
Kết quả chi tiết: Tất cả yêu cầu được xử lý thành công, không có lỗi.

Kịch Bản Kiểm Thử Lần 2
Tên Kịch Bản: Kiểm thử trang "Resources"
Mục Đích: Đánh giá hiệu năng của trang /resources/ trên www.simplilearn.com.
HTTP Request: www.simplilearn.com/resources/
Tham Số: Không có tham số bổ sung
Số lượng Thread (Người dùng): 5
Ramp-up Period (Giây): 2
Loop Count: 5
Kết Quả Mong Đợi: Gửi yêu cầu HTTP thành công.
Kết Quả Thực Tế: Yêu cầu được gửi thành công (xem View Results Tree).
Trạng Thái: Thành công
Kết Quả Sau Khi Test:
![image](https://github.com/user-attachments/assets/35dec0af-4f19-4d57-9a8f-c5338dfdcc34)

Thời gian phản hồi trung bình: 9 giây
Tỷ lệ yêu cầu thành công: 100%
Kết quả chi tiết: Tất cả yêu cầu được xử lý thành công, không có lỗi.

Kịch Bản Kiểm Thử Lần 3
Tên Kịch Bản: Kiểm thử trang "Corporate"
Mục Đích: Đánh giá hiệu năng của trang /corporate-training/ trên www.simplilearn.com.
HTTP Request: www.simplilearn.com/corporate-training/
Tham Số: Không có tham số bổ sung
Số lượng Thread (Người dùng): 10
Ramp-up Period (Giây): 3
Loop Count: 10
Kết Quả Mong Đợi: Gửi yêu cầu HTTP thành công.
Kết Quả Thực Tế: Yêu cầu được gửi thành công (xem View Results Tree).
Trạng Thái: Thành công
Kết Quả Sau Khi Test:
![image](https://github.com/user-attachments/assets/d7127948-42cb-4e12-a032-9f9f3928c95e)

Thời gian phản hồi trung bình: 12 giây
Tỷ lệ yêu cầu thành công: 98%
Kết quả chi tiết: Một số yêu cầu có độ trễ nhẹ, nhưng không có lỗi nghiêm trọng.
![image](https://github.com/user-attachments/assets/0b009696-d7e9-44c2-b5f0-3efbb6a88de6)

5. Kết Luận
Các trang web www.simplilearn.com, /resources/, và /corporate-training/ hoạt động ổn định dưới các kịch bản kiểm thử. Thời gian phản hồi tăng nhẹ khi số lượng người dùng đồng thời tăng, nhưng tỷ lệ thành công vẫn cao (98-100%). Đề xuất tối ưu hóa thêm để cải thiện hiệu suất khi tải cao.

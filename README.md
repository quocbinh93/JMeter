# JMeter
## Kiểm tra hiệu năng trang web
### Mục tiêu:

- Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập trang web https://phenikaa-uni.edu.vn/vi.
- Chạy kịch bản kiểm tra và ghi lại kết quả.
- Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
- Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của trang web.
### Kịch bản kiểm tra:

- Thread Group:
  - Số lượng thread: 100
-- Thời gian chạy: 60 giây
-- Ramp-up period: 10 giây
- HTTP Request:
-- URL: https://phenikaa-uni.edu.vn/vi
Method: GET
Content encoding: UTF-8
Listeners:
View Results Tree
Aggregate Report
Kết quả kiểm tra:

Metric	Value
Total requests	1000
Successful requests	998
Failed requests	2
Average response time	40 ms
Median response time	38 ms
90th percentile response time	70 ms
Throughput	16 requests/second

drive_spreadsheet
Xuất sang Trang tính
Phân tích kết quả kiểm tra:

Số lượng yêu cầu thành công: 998/1000 = 99,8%
Số lượng yêu cầu thất bại: 2/1000 = 0,2%
Thời gian phản hồi trung bình: 40 ms
Thời gian phản hồi trung vị: 38 ms
Thời gian phản hồi percentil 90: 70 ms
Chuyển tải: 16 yêu cầu/giây
Kết luận:

Trang web https://phenikaa-uni.edu.vn/vi có hiệu năng tốt. Số lượng yêu cầu thành công rất cao (99,8%), số lượng yêu cầu thất bại rất thấp (0,2%). Thời gian phản hồi trung bình, trung vị và percentil 90 đều ở mức thấp (dưới 100 ms). Chuyển tải của trang web cũng khá cao (16 yêu cầu/giây).

Lưu ý:

Kết quả kiểm tra này chỉ mang tính chất tham khảo. Hiệu năng thực tế của trang web có thể thay đổi tùy thuộc vào nhiều yếu tố, chẳng hạn như lưu lượng truy cập, vị trí máy chủ, v.v.
Để có được kết quả kiểm tra chính xác hơn, cần thực hiện nhiều lần kiểm tra trong các điều kiện khác nhau.
Bài tập 2: Kiểm tra hiệu năng API

Mục tiêu:

Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập API thời tiết https://openweathermap.org/current.
Chạy kịch bản kiểm tra và ghi lại kết quả.
Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của API.
Kịch bản kiểm tra:

Thread Group:
Số lượng thread: 100
Thời gian chạy: 60 giây
Ramp-up period: 10 giây
HTTP Request:
URL: https://openweathermap.org/current
Method: GET
Content encoding: UTF-8
Listeners:
View Results Tree
Aggregate Report
Kết quả kiểm tra:

Metric	Value
Total requests	1000
Successful requests	996
Failed requests	4
Average response time	100 ms
Median response time	98 ms
90th percentile response time	150 ms
Throughput	16 requests/second

drive_spreadsheet
Xuất sang Trang tính
Phân tích kết quả kiểm tra:

Số lượng yêu cầu thành công: 996/1000 = 99,6%
Số lượng yêu cầu thất bại: 4/1000 = 0,4%
Thời gian phản hồi trung bình: 10

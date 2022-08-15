# Linear-Regression
Data fitting using linear regression
Trong đồ án này, sinh viên được yêu cầu thực hiện:

1. Xây dựng mô hình *dự đoán tuổi thọ trung bình* **sử dụng hồi quy tuyến tính** (7 điểm)

- Yêu cầu 1a: Sử dụng toàn bộ 10 đặc trưng đề bài cung cấp (2 điểm)
	- Huấn luyện 1 lần duy nhất cho 10 đặc trưng trên toàn bộ tập huấn luyện (`train.csv`)
	- Thể hiện công thức cho mô hình hồi quy (tính $y$ theo 10 đặc trưng trong $X$)
	- Báo cáo **1 kết quả trên tập kiểm tra (`test.csv`)** cho mô hình vừa huấn luyện được
    
- Yêu cầu 1b: Xây dựng mô hình sử dụng duy nhất 1 đặc trưng, tìm mô hình cho kết quả tốt nhất (2 điểm)
	- Thử nghiệm trên toàn bộ (10) đặc trưng đề bài cung cấp
	- Yêu cầu **sử dụng phương pháp 5-fold Cross Validation** để tìm ra đặc trưng tốt nhất
	- Báo cáo **10 kết quả tương ứng cho 10 mô hình** từ 5-fold Cross Validation (lấy trung bình)
	
	<center>

	| STT | Mô hình với 1 đặc trưng | RMSE |
	|:---:|:-----------------------:|:----:|
	|  1  | Adult Mortality         |      |
	|  2  | BMI                     |      |
	|     | ...                     |      |
	|  10 | Schooling               |      |

	</center>

	- Thể hiện công thức cho mô hình hồi quy theo đặc trưng tốt nhất (tính $y$ theo đặc trưng tốt nhất tìm được)
    - Báo cáo **1 kết quả trên tập kiểm tra (`test.csv`)** cho mô hình tốt nhất tìm được
	
- Yêu cầu 1c: Sinh viên tự xây dựng mô hình, tìm mô hình cho kết quả tốt nhất (3 điểm)
	- Xây dựng `m` mô hình khác nhau (tối thiểu 3), đồng thời khác mô hình ở 1a và 1b
		- Mô hình có thể là sự kết hợp của 2 hoặc nhiều đặc trưng
		- Mô hình có thể sử dụng đặc trưng đã được chuẩn hóa hoặc biến đổi (bình phương, lập phương...)
		- Mô hình có thể sử dụng đặc trưng được tạo ra từ 2 hoặc nhiều đặc trưng khác nhau (cộng 2 đặc trưng, nhân 2 đặc trưng...)
		- ...
	- Yêu cầu **sử dụng phương pháp 5-fold Cross Validation** để tìm ra mô hình tốt nhất
	- Báo cáo **`m` kết quả tương ứng cho `m` mô hình** từ 5-fold Cross Validation (lấy trung bình)

	<center>

	| STT |           Mô hình          | RMSE |
	|:---:|:--------------------------:|:----:|
	|  1  | Sử dụng 2 đặc trưng (a, b) |      |
	| ... | ...                        |      |
	|  m  | ...                        |      |

	</center>

	- Thể hiện công thức cho mô hình hồi quy tốt nhất mà sinh viên tìm được
	- Báo cáo **1 kết quả trên tập kiểm tra (`test.csv`)** cho mô hình tốt nhất tìm được

- <ins>Lưu ý:</ins>
    - Tập `test.csv` chỉ được sử dụng 3 lần như được đề cập bên trên
    - Kết quả báo cáo là độ đo [RMSE](https://www.sciencedirect.com/topics/engineering/root-mean-squared-error)
    

2. Báo cáo về kết quả, đánh giá và nhận xét các mô hình đã xây dựng (3 điểm)
    - Báo cáo cần có thông tin cá nhân (họ và tên, MSSV), số trang và tài liệu tham khảo (cần chỉ định cụ thể tài liệu được sử dụng cho phần nào trong bài làm)
    - Liệt kê TẤT CẢ thư viện đã sử dụng và lý do sử dụng chúng
	- Liệt kê TẤT CẢ hàm đã sử dụng và mô tả các hàm đó
    - Báo cáo và nhận xét kết quả từ TOÀN BỘ các mô hình xây dựng được (có $1 + (10 + 1) + (m + 1)$ kết quả)
    - Với yêu cầu 1b và 1c: giải thích hoặc nêu giả thuyết cho mô hình đạt kết quả tốt nhất
	- Với yêu cầu 1c: giải thích lý do vì sao lại trích chọn/thiết kế các đặc trưng cho `m` mô hình

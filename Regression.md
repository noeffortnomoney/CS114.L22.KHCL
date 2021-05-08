## Một số bài toán regression trong thực tế

### 1. Dự đoán tuổi thọ trung bình của từng nước

- Input:
    + Tỉ lệ sinh sản
    + New Environmental Performance Index (EPI)
    + GDP(gross domestic product)
    + Tỉ lệ bệnh tim
    + Dân số
    + Mật độ dân số
    + Tỉ lệ đột quỵ
- Output:
    Tuổi thọ trung bình của từng nước
- Cách thu nhập data:
    Có thể thu nhập thông tin qua internet (vì thực sự thông tin không quá khó kiếm) như wikipedia,etc.. hoặc đơn giản hơn có thể lấy bộ dataset của WHO trên Kaggle
- Cách xử lý data:
    +Tìm xem các feature nào có bị multicollinear và xử lý.
    +Tìm xem các feature là outliner và xử lý

### 2. Dự đoán kết quả tổng kết môn học từ số giờ học ở nhà trong 1 tuần của 1 sinh viên

- Input:
	  Số giờ (giờ). (Kiểu số thực)
- Output:
	  Kết quả tổng kết môn học. (Kiểu số thực)
- Cách thu thập data:
	  Bộ dữ liệu khảo sát giờ học và điểm tổng kết môn học tương ứng của mỗi sinh viên do nhà trường thu thập.
- Cách xử lý data:
    + Gom nhóm các dữ liệu về số giờ học và kết quả tổng kết vào cùng 1 file CSV.
    + Xóa các dữ liệu không hợp lí (NULL hoặc giá trị âm).

### 3. Dự đoán giá nhà ở

- Input: (kiểu số nguyên)
    + Diện tích $(m^2)$
    + Số phòng
    + Tuổi căn nhà
 - Output: (kiểu số nguyên)
     Giá nhà (triệu đồng)
 - Cách thu thập data:
    + Thu thập bộ dữ liệu về giá nhà ở (từ các trang web rao bán nhà ở, bất động sản)
    + Xin dữ liệu từ nhà ở trong thực tế (tìm kiếm khách hàng rao bán nhà ở)
    + Ngoài ra, cần tìm hiểu rõ thị trường bất động sản (nhà ở) ở thời điểm trong quá khứ gần nhất đến tương lai
- Cách xử lý data:
    + Gom nhóm các dữ liệu về diện tích, số phòng, tuổi căn nhà và giá nhà vào cùng 1 file CSV
    + Xóa các dòng mà thuộc tính không có giá trị (NULL)
    + Xóa các dồng mà thuộc tính có giá trị âm
 
 ### 4. Dự đoán cân nặng của 1 người từ chiều cao của họ
 
 - Input: (kiểu số thực)
     Chiều cao (cm)
 - Output: (kiểu số nguyên)
     Cân nặng (kg)
 - Cách thu thập data:
    + Thu thập bộ dữ liệu về chiều cao của người (từ các trang web số liệu về chiều cao)
    + Xin dữ liệu từ chiều cao của mọi người trong thực tế (có thể dùng cách khảo sát để tìm kiếm dữ liệu)
    + Ngoài ra, cần tìm hiểu rõ số liệu chiều cao của người ở thời điểm trong quá khứ gần nhất đến tương lai
- Cách xử lý data:
    + Gom nhóm các dữ liệu về chiều cao và cân nặng vào cùng 1 file CSV
    + Xóa các dòng mà thuộc tính không có giá trị (NULL)
    + Xóa các dồng mà thuộc tính có giá trị âm

# MÔ TẢ ĐỒ ÁN CUỐI KÌ

## Lý do chọn đề tài này
Nhận dạng là lĩnh vực được các nhà khoa học rất quan tâm để giải quyết các yêu cầu 
trong cuộc sống hiện nay, có nhiều lĩnh vực nhận dạng như nhận dạng tín hiệu, nhận dạng 
tiếng nói hay nhận dạng ảnh. Vấn đề nhận dạng chữ viết tay thực sự là một thách thức đối với 
những nhà nghiên cứu.

Chữ viết tay xuất hiện ở hầu hết trong các công việc cảu các cơ quan, nhà máy, xí 
nghiệp, trường học. Việc nhập một văn bản viết tay trên giấy vào máy tính hầu như chỉ có 
một cách giải quyết đó là gõ lại từng ký tự, việc này luôn chiếm nhiều thời gian và đôi khi 
không đảm bảo tiến độ hoạt động của công việc. Việc nhận dạng chữ viết tay hầu như đã có 
nhiều nhà nghiên cứu thử sức, nhưng phần lớn họ chỉ nhận diện chữ viết tiếng Anh, vậy 
những ngôn ngữ của các quốc gia khác thì sao? Với những lý do trên nhóm em đã chọn 
nghiên cứu đề tài: “Nhận dạng chữ viết tay tiếng Việt”.

## Mô tả bài toán
Bài toán thuộc dạng bài phân loại.

INPUT: Một tấm ảnh trong đó có chứa đúng một chữ cái tiếng Việt. 

OUTPUT: Chữ cái tương ứng với tấm ảnh đó.

VD: 

Input:            

   ![image](https://user-images.githubusercontent.com/79963001/126604150-d7520a5f-f4b4-4558-886c-3beeef64de2e.png)

Output: a



## Mô tả về bộ dữ liệu
### Cách thức xây dựng bộ dữ liệu
Bộ dữ liệu tự xây dựng.

Ngôn ngữ sử dụng: tiếng Việt.

Bảng chữ cái Việt Nam bao gồm 29 chữ cái. Trong đó 22 chữ cái là thuộc chữ cái 
latin. Có 7 chữ cái biến thể bằng cách thêm dấu. Không những thế chữ cái còn có thêm 6 ngữ 
âm là ngang, sắc , huyền , hỏi, ngã, nặng. Kết hợp với các nguyên âm sẽ tạo nên các biến thể 
khác. Tổng cộng chúng ta sẽ có 89 loại chữ cần thu thập. 

Nhóm em đã làm các tờ giấy thu nhập chữ viết phân phát cho người thân và người 
quen. Một bộ sẽ có hai tờ giấy, bao gồm 89 chữ cái, mỗi chữ cái sẽ được điền 10 lần. Sau đó 
các tờ giấy sẽ được thu nhập và chụp hình lại. Hình sau đó sẽ được phân tách ra thành từng 
chữ cái và dán nhãn. Đây là phương thức vô cùng mất thời gian nhưng đảm bảo tính đa dạng 
của dataset.

Nhóm em đã share dataset với nhóm của bạn Nguyễn Dương Hải.

### Số lượng, độ đa dạng dữ liệu
Bộ dataset chữ cái viết tay tiếng Việt sau khi thu thập có tổng cộng 50114 hình ảnh đã 
được phân loại.

Tham khảo tại: [Dataset Chữ cái Tiếng Việt](https://github.com/noeffortnomoney/CS114.L22.KHCL/blob/main/Final%20Project/Dataset%20ch%E1%BB%AF%20c%C3%A1i%20thu%20th%E1%BA%ADp.md)

Dataset được chia làm ba set: 30068 ảnh cho Training set, 10023 ảnh cho Val set và 
10023 ảnh cho Test set.

### Các thao tác, tiền xử lí dữ liệu:
Tiền xử lý ảnh là một bước vô cùng quan trọng để chuẩn bị dữ liệu cho các model. Có 
rất nhiều bước quan trọng trong xử lý tiền dữ liệu như data cleaning, data transformation và 
feature selection. Một tập dữ liệu sẽ chứa rất nhiều biến số, một biến số sẽ chứa rất nhiều 
thông tin. Vì vậy để đơn giản hóa các chiều không gian của model, chúng ta sẽ chỉ chọn 
những biến số độc đáo và chứa thông tin quan trọng.



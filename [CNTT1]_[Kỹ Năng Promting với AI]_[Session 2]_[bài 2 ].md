
# **Phần 1: Phân tích vấn đề**

Dựa vào số lượng ví dụ mẫu trong từng câu lệnh, em xác định các dòng bị phân loại sai theo bảng sau :
| STT | Phân loại bị sai  hiện tại | Phân loại đúng | Lý do |
|---|---|---|---|
| 1 | Few-shot | Zero-shot | Không có ví dụ mẫu. |
| 2 | One-shot | Zero-shot | Không có ví dụ mẫu. |
| 4 | Zero-shot | Few-shot | Có 3 ví dụ mẫu. |
| 5 | Few-shot | Zero-shot | Không có ví dụ mẫu.

- Các dòng 1, 2, 4, 5 là  bị phân loại sai đã đc phân lại trong bảng trên . Còn  dòng 3 và 6 đã được phân loại đúng rồi .
# **Phần 2: Hoàn thiện bảng**
| STT | Nội dung câu lệnh (Prompt) | Phân loại đúng | Số lượng ví dụ mẫu nhận diện được |
|---|---|---|---|
| 1 | Phân loại đánh giá: 'Pin dùng được nửa ngày là hết'. | Zero-shot | 0 |
| 2 | Viết hoa tiêu đề theo phong cách công nghệ. | Zero-shot | 0 |
| 3 | RAM 8GB → Đa nhiệm mượt mà mở 20 tab. | One-shot | 1 |
| 4 | Hàng tốt → Pos; Giao trễ → Neg; Bình thường → Neu. | Few-shot | 3 |
| 5 | Viết lại email thông báo bảo hành xong cho khách. | Zero-shot | 0 |
| 6 | Err_404 → Không tìm thấy trang. | One-shot | 1 |

# **Bước 1: Thiết kế 2 phương án Prompt là :

### **1. Phương án 1: Zero-shot**

**Prompt:**


Hãy phân loại phản hồi khách hàng thành 3 nhóm sau :

- TÍCH CỰC: 
- TIÊU CỰC: 
- HỖ TRỢ: 
câu mỉa mai sau :"Nhân viên nhiệt tình quá, gọi mãi 30 phút mới thấy xuất hiện!" 
hãy đọc và xác định nhóm cần phân loại 


### **2. Phương án 2: Few-shot**

**Prompt:**


Hãy phân loại phản hồi khách hàng thành 3 nhóm:
TÍCH CỰC, TIÊU CỰC, CẦN HỖ TRỢ.

Ví dụ:
- "Đồ ăn ngon, giá rẻ." → TÍCH CỰC
- "Giao hàng chậm, nhân viên thái độ tệ." → TIÊU CỰC
- "Cửa hàng ở đâu? Giá món này bao nhiêu?" → CHỖ TRỢ
câu mỉa mai sau :"Nhân viên nhiệt tình quá, gọi mãi 30 phút mới thấy xuất hiện!"

Hãy dựa vào các ví dụ trên để xếp loại và phân loại khách hàng 


# **Bước 2: Bảng so sánh Trade-off**
| Tiêu chí | Giải pháp 1 (Zero-shot) | Giải pháp 2 (Few-shot) |
|---|---|---|
| Độ dễ hiểu | Cao, dễ viết nhanh | Trung bình, cần viết dài |
| Tốn token | Ít tốn token | Tốn nhiều token hơn |
| Xử lý câu mỉa mai | Kém, dễ bị nhầm | Tốt, có ví dụ mẫu để làm theo |
| Độ chính xác | Có thể chưa chính xác | Chính xác hơn trong trường hợp có ví dụ |



# **Bước 3: Thử nghiệm thực tế**


### bảng thử nghiệm kết quả thực tế

| Phương án | Kết quả phân loại |
|---|---|
| Zero-shot | TÍCH CỰC (Ai bị dễ nhầm do có từ " nhiệt tình ") |
| Few-shot | Nhận dạng đúng đây là phản hồi TIÊU CỰC |

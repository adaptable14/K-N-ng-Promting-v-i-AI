

# Phần 1. Phân tích BPE

1.  **Cơ chế cắt từ của BPE đối với ký tự tiếng Việt có dấu là**

BPE là thuật toán chia văn bản thành các đơn vị nhỏ gọi là Token. Và Đối với tiếng Việt các từ có dấu  có thể bị chia thành nhiều Token nhỏ hơn do nguyên lí vận hành của BPE
Vì vậy, một từ có thể chứa nhiều Token, không phải lúc nào  1 từ luôn bằng 1 Token.

2. **Nguyên nhân Mẫu B tốn Token hơn Mẫu A  vì**

-   **Mẫu A (Tiếng Anh):** vì  các từ tiếng Anh thường được nhận diện thành những cụm lớn nên số Token ít hơn.
    
-   **Mẫu B (Tiếng Việt):** Các từ Tiếng việt có dấu và cụm ký tự phức tạp hơn  có thể bị chia thành nhiều phần nhỏ nên số Token tăng lên.
    

# **Phần 2. Tối ưu Prompt tiếng Việt để giúp tiết kiệm khoảng 30–40% Token:

** Đề xuất 1: Viết Prompt ngắn gọn, loại bỏ từ dư thừa**

-   Bỏ những câu chào hỏi, từ ngữ không cần thiết.
    
-   Không lặp lại yêu cầu nhiều lần.
    
-  Chỉ  giữ lại những thông tin quan trọng.
    

** Đề xuất  2: Dùng gạch đầu dòng và gộp các yêu cầu**

-   Trình bày yêu cầu bằng gạch đầu dòng.
    
-   Gộp các ý có nội dung liên quan vào với nhau 
    
-   Hạn chế diễn đạt  ý muốn bằng những câu khác nhau gọn .
    



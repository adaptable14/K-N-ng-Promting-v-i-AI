
# **Phần 1. Giải thích hình tượng Chiếc cốc nước là :**

Context Window  có thể hiểu giống như một chiếc cốc nước có dung tích nước  giới hạn. Mỗi tin nhắn của khách hàng và câu trả lời của AI đều chiếm một lượng nước nhỏ  hay dc hiểu là  Token trong chiếc cốc.  Và Khi cuộc hội thoại kéo dài, lượng nước hay lượng  Token ngày càng tăng. Khi cốc đầy, hệ thống có thể cắt bỏ những thông tin cũ để nhường chỗ cho thông tin mới đị đây như là lúc dót nước chàn cốc lượng nước cũ xe bi chàn da ngoài để thay thế cho lượng nước mới 

 và để  giải thích cho nhân viên lý do AI quên thông tin ở Lượt 1 qua hình ảnh chiếc cốc thì là do AI quên tên và mã đơn hàng của khách vì thông tin ở lượt 1  vì lượng token đã đầy khiến cho dữ liệu cũ có thể  đẩy ra khỏi cốc . Vì thế khiến cho  AI không còn đủ thông tin để nhận diện đúng khách hàng và xảy ra nhầm lẫn và xai sót 

## **Phần 2. Phương án quản lý RAM bộ nhớ**

  **phương án 1 :**

-   Yêu cầu AI trả lời ngắn gọn, tránh giải thích dài dòng.
    
-   Thường xuyên tóm tắt những thông tin quan trọng trong cuộc hội thoại.
    
-   Nhắc lại tên khách hàng và mã đơn hàng khi cần thiết chánh trường hợp AI bị quên .
    

**phương án 2**

-   Khi bắt đầu phiên hoạt động mới, tự động chuyển các thông tin quan trọng từ phiên trước hoặc tóm tắt nội dung  ngắn gọn của thông tin ấy sang phiên hoạt động mới
    
- Giới hạn độ dài câu trả lời của AI để tránh lãng phí dung lượng Context Window.
    
-    Chia cuộc hội thoại thành nhiều phiên nhỏ theo từng chủ đề để tránh tích lũy quá nhiều Token.


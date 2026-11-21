**Phép tích chập và Max Pooling:** Tính toán thủ công ma trận đầu ra và xác định kích thước qua các bước trượt cửa sổ tích chập (Convolution) và gộp cực đại (Max Pooling).

**Luồng dữ liệu qua các tầng:** Xác định kích thước bản đồ đặc trưng (Feature Map) qua nhiều tầng tích chập liên tiếp và số chiều của vector sau bước duỗi phẳng (Flatten).

**Xử lý đầu vào có độ dài thay đổi:** Trình bày hai phương pháp chuẩn hóa đầu vào cho dữ liệu chuỗi: Padding/cắt bớt về độ dài cố định và sử dụng Global Max Pooling.

**Biểu diễn văn bản (Text CNN):** Chuyển đổi câu văn sang dạng số thông qua nhân ma trận One-Hot Encoding với ma trận Embedding, sau đó áp dụng các bộ lọc n-gram (2-gram, 3-gram) kết hợp Max Pooling để trích xuất vector đặc trưng.

**Lưu trữ và nạp mô hình (Chương 13):** Quản lý trọng số và trạng thái mô hình qua `state_dict()`, lưu và khôi phục mô hình bằng `torch.save` và `pickle`.

**Khảo sát hàm kích hoạt (Chương 14):** So sánh trực quan Sigmoid, Tanh, ReLU, ReLU6 và LeakyReLU trên bài toán phân loại phi tuyến (`make_circles`), theo dõi độ lớn gradient qua từng tầng để phân tích hiện tượng triệt tiêu gradient (vanishing gradient).

**Hàm mất mát (Chương 15):** Triển khai các hàm mất mát cho bài toán hồi quy (MSE, MAE), phân loại (Cross-Entropy, NLLLoss, BCELoss) và tự định nghĩa hàm mất mát tùy chỉnh (MAPE).

**Điều chuẩn và Lịch trình học (Chương 16 - 17):** Áp dụng kỹ thuật Dropout để giảm overfitting và điều chỉnh tốc độ học động bằng `lr_scheduler` (LinearLR, ExponentialLR, LambdaLR).

**Quản lý dữ liệu và Tinh chỉnh siêu tham số (Chương 18 - 20):** Xây dựng luồng nạp dữ liệu theo lô với `Dataset` và `DataLoader`, tích hợp mô hình PyTorch vào `scikit-learn` (thông qua `skorch`) để đánh giá chéo (k-fold) và tìm kiếm siêu tham số tối ưu (Grid Search).

**Kiểm soát và Trực quan hóa quá trình huấn luyện (Chương 21 - 23):** Tạo điểm lưu (Checkpointing), dừng sớm (Early Stopping)[cite: 120, 128], xuất kiến trúc mạng sang định dạng ONNX để trực quan hóa bằng Netron và vẽ biểu đồ theo dõi các chỉ số đánh giá qua từng epoch.

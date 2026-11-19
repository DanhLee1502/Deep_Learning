**Thiết kế kiến trúc MLP:** Xây dựng cấu trúc mạng, lựa chọn hàm kích hoạt đầu ra và hàm mất mát phù hợp cho ba bài toán điển hình: hồi quy tuyến tính (Linear + MSE), phân loại nhị phân (Sigmoid + BCE) và phân loại đa lớp (Softmax + CCE), đồng thời tính toán số lượng tham số cần học.

**MLP cho bài toán hồi quy:** Thực hiện thủ công một chu kỳ huấn luyện hoàn chỉnh gồm lan truyền xuôi (Feedforward) với hàm kích hoạt ReLU, lan truyền ngược (Backpropagation) bằng quy tắc dây chuyền, cập nhật trọng số và đánh giá mức độ giảm của hàm mất mát.

**MLP cho bài toán phân loại đa lớp:** Tính toán vector logits, chuyển đổi sang phân bố xác suất bằng hàm Softmax, tính hàm mất mát Categorical Cross-Entropy và xác định kích thước ma trận gradient ở tầng đầu ra.

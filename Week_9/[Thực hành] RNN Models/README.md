**Dự đoán chuỗi thời gian (Chương 27):** Tìm hiểu cấu trúc tế bào LSTM (các cổng điều khiển và trạng thái bộ nhớ). Tiền xử lý dữ liệu chuỗi thời gian (`airline-passengers.csv`) theo phương pháp cửa sổ trượt (sliding window), huấn luyện mô hình hồi quy với `nn.LSTM`, đánh giá bằng chỉ số RMSE và trực quan hóa kết quả dự đoán qua các độ dài cửa sổ khác nhau (`lookback = 1` và `lookback = 4`).

**Mô hình sinh văn bản (Chương 28):** Xây dựng mô hình sinh văn bản ở mức ký tự (character-level) trên tập dữ liệu *Alice's Adventures in Wonderland*. Thực hiện ánh xạ ký tự sang số, huấn luyện mạng LSTM đơn tầng và đa tầng (stacked LSTM) để tự động sinh chuỗi văn bản mới từ một đoạn gợi ý (prompt).

**Tối ưu hóa huấn luyện trên GPU:** Kiểm tra thiết bị phần cứng (`torch.cuda`) và chuyển dịch dữ liệu cùng tham số mô hình sang GPU (`.to(device)`) để tăng tốc độ huấn luyện cho các mô hình chuỗi.

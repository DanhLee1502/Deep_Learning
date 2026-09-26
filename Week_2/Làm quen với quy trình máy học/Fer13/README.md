Bài toán nhận diện cảm xúc khuôn mặt (7 lớp: angry, disgust, fear, happy, neutral, sad, surprise) từ ảnh grayscale 48×48 (Kaggle FER2013), dùng CNN thay vì thuật toán ML cổ điển vì là dữ liệu ảnh.

  - Dữ liệu: 28,709 ảnh train / 7,178 ảnh test, mất cân bằng nghiêm trọng (disgust chỉ ~1.5% dữ liệu)
  - Xử lý dữ liệu: chuẩn hóa pixel, data augmentation (flip/rotate/zoom), tính class weights để xử lý mất cân bằng
  - Spot-check kiến trúc: so sánh CNN cơ bản (2 khối Conv-MaxPool) và CNN cải tiến (3 khối Conv-BatchNorm-Dropout + augmentation)
  - Tối ưu: huấn luyện với EarlyStopping, ReduceLROnPlateau, ModelCheckpoint; minh họa ý tưởng ensemble
  - Kết quả: ~47% accuracy trên tập test (giới hạn do huấn luyện trên CPU 1 nhân, không GPU) — lưu model .keras + nhãn lớp, kèm hướng cải thiện (transfer learning, thêm epoch, oversampling)

Bài toán phân loại đa lớp (3 loài hoa: setosa, versicolor, virginica) trên bộ dữ liệu Iris kinh điển (UCI).

  - Dữ liệu: 150 mẫu, 4 thuộc tính số (sepal/petal length & width), sạch, không missing, 3 lớp cân bằng
  - Khám phá dữ liệu: box plot, histogram, scatter matrix — nhận thấy petal-length/petal-width phân tách 3 loài rất rõ
  - Mô hình: so sánh 6 thuật toán (LR, LDA, KNN, CART, NB, SVM) bằng 10-fold cross-validation
  - Tối ưu: GridSearchCV tuning KNN & SVM, thử nghiệm thêm Random Forest và Voting Classifier
  - Kết quả: SVM sau tuning đạt 100% accuracy trên tập validation; lưu model + minh họa dự đoán trên mẫu mới

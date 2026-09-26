Bài toán phân loại nhị phân — dự đoán khả năng sống sót của hành khách trên tàu Titanic (dữ liệu Kaggle).

  - Dữ liệu: 891 mẫu train, 12 thuộc tính (tuổi, giới tính, hạng vé, giá vé, số người thân đi cùng...), có missing ở Age/Cabin/Embarked
  - Xử lý dữ liệu: điền missing Age (median theo Pclass+Sex), Embarked (mode), Fare (median theo Pclass)
  - Feature engineering: trích xuất Title từ tên, tạo FamilySize, IsAlone, HasCabin, mã hóa Sex/Embarked
  - Mô hình: so sánh 6 thuật toán (Logistic Regression, KNN, Decision Tree, Naive Bayes, SVM, Random Forest) bằng 10-fold cross-validation
  - Tối ưu: GridSearchCV tuning Random Forest & SVM, thử nghiệm Voting Classifier  
  - Kết quả: đánh giá trên tập validation (accuracy, confusion matrix), xuất submission.csv sẵn sàng nộp Kaggle

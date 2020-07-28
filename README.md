# BBC-text-categorization

Tập dữ liệu này chứa 2225 bài báo trên BBC và gồm 2 trường. Trường thứ nhất là chủ đề của bài báo, trường thứ 2 là nội dung và tiêu đề của bài báo. Trong bài này m sẽ sử dụng machine learning cũng như convolutional neural network để phân loại bài báo vào 1 trong 5 chủ đề. Nội dung của notebook bao gồm các phần sau:

1. Understanding data

2. Preprocessing data

Trong phần này mình sẽ loại bỏ các stop words, các từ và kí hiều đặc biệt cũng như thực hiện stemming và Lemmantization

3. Feature extraction and traning model

Phần này mình sử dụng mình sử dụng 2 loại model là machine learning và Convolutional neural network. Đối với Machine learning model thì đầu tiên mình sử dụng bag of word /tfidf để extract feature. Sau đó sử dụng Logistic regression và SVC để train model. Ở đây mình không sử dụng Random forest hay XGBoost vì feature là sparse nên không phù hợp. Mình tối ưu tham số bằng GridSearchCV. Đối với CNN thì mình sử dụng cấu trúc cơ bản vì bộ dữ liệu này nhỏ, không phù hợp để sd Deep learning

4. Feature important

Sau khi train các model thì LogisticRegression + Bag of word cho kết quả tốt nhất. Mình sử dụng hệ số của mô hình này để tìm feature. Vì các feature có cùng scale nên hệ số càng cao thì feature càng quan trọng

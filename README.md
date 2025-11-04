# 🧠 Dự án Tiền Xử Lý Dữ Liệu

## 👥 Thành viên nhóm
| Họ và tên | MSSV |
|------------|--------|
| Nguyễn Bách Khoa | 23127066 |
| Trương Quang Huy | 23127530 |
| Trần Danh Thiện | 23127120 |

---

## 📘 Tổng quan dự án
Dự án này xây dựng **pipeline tiền xử lý dữ liệu** cho ba loại dữ liệu phổ biến trong lĩnh vực **Machine Learning**:

- 🖼️ **Ảnh (Image)** — CIFAR-10  
- 📊 **Dữ liệu dạng bảng (Tabular)** — Credit Card Fraud Detection  
- 🗞️ **Văn bản (Text)** — Rumor Detection from Twitter  

Mục tiêu của dự án là thực hiện các bước **làm sạch, chuẩn hóa và biểu diễn dữ liệu** để sẵn sàng cho huấn luyện mô hình học máy.

---

## 📂 Cấu trúc dự án
project-root/
├── README.md
├── requirements.txt
├── data/
│ ├── images/ # Dataset CIFAR-10
│ ├── tabular/ # Dataset Credit Card Fraud
│ └── text/ # Dataset Twitter Rumor Detection
├── notebooks/
│ ├── 01_image_preprocessing.ipynb
│ ├── 02_tabular_preprocessing.ipynb
│ └── 03_text_preprocessing.ipynb
└── docs/
└── Report.pdf

yaml
Sao chép mã

---

## 📊 Mô tả Dataset và Nguồn tải

| Loại dữ liệu | Tên Dataset | Mô tả ngắn gọn | Nguồn tải |
|---------------|--------------|----------------|------------|
| 🖼️ Ảnh (Image) | **CIFAR-10** | Bộ dữ liệu gồm **60,000 ảnh màu** kích thước **32x32 pixel** thuộc **10 lớp** khác nhau (máy bay, ô tô, chim, mèo, hươu, chó, ếch, ngựa, tàu thủy, xe tải). Được dùng phổ biến để huấn luyện và đánh giá các mô hình phân loại ảnh. | [https://www.cs.toronto.edu/~kriz/cifar.html](https://www.cs.toronto.edu/~kriz/cifar.html) |
| 📊 Dữ liệu bảng (Tabular) | **Credit Card Fraud Detection** | Gồm **284,807 giao dịch thẻ tín dụng**, trong đó chỉ có **492 giao dịch gian lận (fraud)**. Các đặc trưng đã được ẩn danh bằng PCA. Mục tiêu là phát hiện giao dịch gian lận dựa trên dữ liệu lịch sử. | [https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) |
| 🗞️ Văn bản (Text) | **Rumor Detection ACL 2017** | Gồm các **tweet và bài đăng Twitter** được gán nhãn **rumor / non-rumor**. Dữ liệu được sử dụng trong bài báo ACL 2017, nhằm phát hiện và phân loại tin đồn trên mạng xã hội. | [https://www.kaggle.com/datasets/syntheticprogrammer/rumor-detection-acl-2017](https://www.kaggle.com/datasets/syntheticprogrammer/rumor-detection-acl-2017) |

📌 **Lưu ý:** Sau khi tải dataset, hãy đặt vào thư mục `data/` theo đúng cấu trúc trên để notebook hoạt động chính xác.

---

## ⚙️ Cài đặt môi trường

### 1️⃣ Cài đặt thư viện phụ thuộc
```bash
pip install -r requirements.txt
2️⃣ Yêu cầu hệ thống
Python >= 3.8

Jupyter Notebook hoặc JupyterLab

🚀 Hướng dẫn chạy dự án
Chạy lần lượt các notebook trong thư mục notebooks/ theo thứ tự sau:

1️⃣ 01_image_preprocessing.ipynb
👉 Tiền xử lý dữ liệu ảnh CIFAR-10: resize, chuyển grayscale, chuẩn hóa, phát hiện biên.

2️⃣ 02_tabular_preprocessing.ipynb
👉 Tiền xử lý dữ liệu bảng Credit Card Fraud: chuẩn hóa với RobustScaler, phân tích tương quan, chọn đặc trưng.

3️⃣ 03_text_preprocessing.ipynb
👉 Tiền xử lý dữ liệu văn bản Twitter Rumor: tokenization, stemming, subword BPE, vector hóa (TF-IDF, Word2Vec).

✨ Tính năng chính
🖼️ Ảnh
Thay đổi kích thước (Resize)

Chuyển sang ảnh xám (Grayscale)

Chuẩn hóa giá trị điểm ảnh (Normalization)

Phát hiện biên (Edge Detection)

📊 Dữ liệu bảng
Chuẩn hóa bằng RobustScaler

Phân tích tương quan (Correlation Heatmap)

Lựa chọn đặc trưng (Feature Selection)

🗞️ Văn bản
Tokenization, Stemming / Lemmatization

BPE / WordPiece Subword Tokenization

Vectorization: Bag-of-Words, TF-IDF, Word2Vec

🔗 Liên kết & Tài nguyên ngoài
📦 Credit Card Fraud Dataset (Kaggle)

🗞️ Twitter Rumor Dataset (Kaggle)

🖼️ CIFAR-10 Dataset (University of Toronto)

📄 docs/Report.pdf: Báo cáo chi tiết pipeline và kết quả

📅 Thời gian thực hiện
Năm học 2025

📧 Liên hệ
Nếu có thắc mắc về dự án, vui lòng liên hệ nhóm qua email sinh viên trường.

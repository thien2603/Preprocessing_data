# 🧠 Dự án Tiền Xử Lý Dữ Liệu

## 📘 Tổng quan
Dự án xây dựng **pipeline hoàn chỉnh** cho việc **tiền xử lý ba loại dữ liệu** phổ biến trong Machine Learning:
- 🖼️ **Ảnh (Image)** – CIFAR-10  
- 📊 **Dữ liệu dạng bảng (Tabular)** – Credit Card Fraud  
- 🗞️ **Văn bản (Text)** – Twitter Rumor Detection  

Mỗi loại dữ liệu được xử lý trong một notebook riêng biệt, bao gồm các bước từ làm sạch, chuẩn hóa đến biểu diễn dữ liệu phục vụ mô hình học máy.

---

## 📂 Cấu trúc dự án
```
project-root/
├── README.md
├── requirements.txt
├── data/
│   ├── images/      # Dataset CIFAR-10
│   ├── tabular/     # Dataset Credit Card Fraud
│   └── text/        # Dataset Twitter Rumor
├── notebooks/
│   ├── 01_image_preprocessing.ipynb
│   ├── 02_tabular_preprocessing.ipynb
│   └── 03_text_preprocessing.ipynb
└── docs/
    └── Report.pdf
```

---

## ⚙️ Cài đặt

### 1️⃣ Cài các thư viện cần thiết
```bash
pip install -r requirements.txt
```

### 2️⃣ Môi trường khuyến nghị
- Python >= 3.8  
- Jupyter Notebook hoặc JupyterLab  

---

## 🚀 Sử dụng

Mở và chạy các notebook Jupyter theo thứ tự:

1️⃣ `01_image_preprocessing.ipynb` — Tiền xử lý ảnh CIFAR-10  
2️⃣ `02_tabular_preprocessing.ipynb` — Tiền xử lý dữ liệu gian lận thẻ tín dụng  
3️⃣ `03_text_preprocessing.ipynb` — Tiền xử lý văn bản phát hiện tin đồn trên Twitter  

---

## ✨ Tính năng chính

### 🖼️ Ảnh
- Thay đổi kích thước (Resize)  
- Chuyển ảnh sang thang xám (Grayscale)  
- Chuẩn hóa giá trị điểm ảnh (Normalization)  
- Phát hiện biên (Edge Detection)

### 📊 Dữ liệu bảng
- Chuẩn hóa bằng **RobustScaler**  
- Lựa chọn đặc trưng (Feature Selection)  
- Phân tích tương quan (Correlation Analysis)

### 🗞️ Văn bản
- **Tokenization** (Tách từ)  
- **Stemming / Lemmatization**  
- **BPE / WordPiece** (Subword Tokenization)  
- **Vectorization** (Bag-of-Words, TF-IDF, Word2Vec)

---

## 🧩 Thư viện cần thiết
```
pandas
numpy
scikit-learn
opencv-python
nltk
matplotlib
seaborn
```

---

## 📄 Tài liệu liên quan
- 📘 `docs/Report.pdf` — Báo cáo chi tiết về pipeline và kết quả tiền xử lý  
- 📓 `notebooks/` — Notebook minh họa và code từng bước  

---

## 👨‍💻 Tác giả
**Nguyễn Bách Khoa/ Trần Danh Thiện/ Trương Quang Huy**  


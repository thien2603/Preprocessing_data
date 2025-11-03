markdown
# Dự án Tiền Xử Lý Dữ Liệu

## Tổng quan
Pipeline hoàn chỉnh cho tiền xử lý ba loại dữ liệu: ảnh, dữ liệu dạng bảng và dữ liệu văn bản.

## Cấu trúc dự án
project-root/
├── README.md
├── requirements.txt
├── data/
│ ├── images/ # Dataset CIFAR-10
│ ├── tabular/ # Dataset Credit Card Fraud
│ └── text/ # Dataset Twitter Rumor
├── notebooks/
│ ├── 01_image_preprocessing.ipynb
│ ├── 02_tabular_preprocessing.ipynb
│ └── 03_text_preprocessing.ipynb
└── docs/
└── Report.pdf

text

## Cài đặt
```bash
pip install -r requirements.txt
Sử dụng
Mở và chạy các notebook Jupyter theo thứ tự:

01_image_preprocessing.ipynb - Xử lý ảnh CIFAR-10

02_tabular_preprocessing.ipynb - Dữ liệu gian lận thẻ tín dụng

03_text_preprocessing.ipynb - Phát hiện tin đồn Twitter

Tính năng chính
Ảnh: Thay đổi kích thước, chuyển xám, chuẩn hóa, phát hiện biên

Dữ liệu bảng: RobustScaler, lựa chọn đặc trưng, phân tích tương quan

Văn bản: Tokenization, stemming, BPE, vectorization

Thư viện cần thiết
pandas, numpy, scikit-learn, opencv-python, nltk, matplotlib, seaborn

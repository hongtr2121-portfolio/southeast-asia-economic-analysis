# 📈 Hành trình tăng trưởng GDP Đông Nam Á & Những bước nhảy vọt kinh tế (1960-2024)

## 👥 Thành viên thực hiện (Nhóm 7)
* **Hương Thủy** - Leader
* **Trần Thúy Hồng** (Data Analyst / Developer)
* **Kim Đăng**, **Thanh Thảo**, **Hải Yến**

---

## 📌 1. Giới thiệu Dự án
Dự án tập trung phân tích sự thay đổi, bứt phá và dịch chuyển mô hình kinh tế của 11 quốc gia Đông Nam Á giai đoạn 1960 - 2024 dựa trên bộ dữ liệu từ World Bank. Qua đó, áp dụng các kỹ thuật phân tích dữ liệu và học máy để phân tầng kinh tế và dự báo xu hướng phát triển giai đoạn 2025 - 2030.

## 🎯 2. Mục tiêu Nghiên cứu
* Phân tích mối quan hệ giữa các biến số Kinh tế (GDP, GDP per Capita) và Dân số.
* Làm rõ sự chênh lệch phân tầng phát triển giữa các nước trong khu vực.
* Dự báo quy mô kinh tế của các quốc gia cốt lõi trong ngắn hạn (2025 - 2030).

## 🛠️ 3. Phương pháp & Công nghệ Sử dụng
* **Ngôn ngữ:** Python (Pandas, Numpy, Matplotlib, Seaborn)
* **Trực quan hóa:** Xây dựng Dashboard tổng quan hành trình tăng trưởng GDP và biến động dân số.
* **Học máy (Machine Learning):**
  * **Giảm chiều dữ liệu:** Sử dụng **PCA (Principal Component Analysis)** giảm từ 3 biến số xuống 2 thành phần chính (PC1 giải thích 64.3% về quy mô kinh tế; PC2 giải thích 34.47% về mức độ thịnh vượng). Tổng phương sai giải thích đạt **98.76%**.
  * **Phân cụm:** Áp dụng thuật toán **K-means (K=3)** để phân nhóm các quốc gia thành 3 cụm phát triển rõ rệt (Quy mô lớn, Phát triển Trung bình/Cao, Quy mô/Phát triển Thấp).
  * **Dự báo (Forecasting):** Sử dụng mô hình **Log-Linear Regression** trên dữ liệu thực tế từ 2015 đến nay để mô tả tăng trưởng theo cấp số nhân.

## 📊 5. Kết quả & Insights Quan trọng
* **Sự phân tầng rõ rệt:** Sau 6 thập kỷ, tổng GDP toàn khu vực tăng gần 300 lần (từ 13.4 tỷ USD lên gần 4,000 tỷ USD vào năm 2024).
* **Kết quả phân cụm (2024):**
  * *Cụm 1:* Indonesia (Tách biệt hoàn toàn nhờ quy mô kinh tế và dân số áp đảo).
  * *Cụm 2 (Phát triển Trung bình/Cao):* Malaysia, Philippines, Singapore, Thailand, Viet Nam.
  * *Cụm 3 (Thấp):* Brunei Darussalam, Cambodia, Lao PDR, Myanmar.
* **Dự báo đến năm 2030:** **Việt Nam** được dự báo sẽ duy trì đà tăng trưởng bền bỉ (nhờ dòng vốn FDI mạnh mẽ, tỷ lệ Đầu tư/GDP cao 32%-35% và cơ cấu dân số vàng) để **vượt qua Thái Lan, trở thành nền kinh tế lớn thứ 3 Đông Nam Á** với mức GDP dự báo đạt **740.40 tỷ USD**.
seasia-gdp-analysis/
│
├── data/
├── notebooks/
├── reports/
├── tableau/               # 👈 Tạo thêm thư mục này
│   └── seasia_gdp_dashboard.twbx   # 👈 Bỏ file Tableau gốc vào đây
├── README.md
└── requirements.txt

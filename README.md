# Phân tích các yếu tố ảnh hưởng đến giá nhà tại TP.HCM giai đoạn 2017–2022

## Giới thiệu

Dự án thực hiện phân tích các yếu tố có khả năng ảnh hưởng đến giá nhà tại Thành phố Hồ Chí Minh trong giai đoạn 2017–2022.

Phân tích tập trung vào dữ liệu giá nhà tại 9 quận cùng với các yếu tố kinh tế vĩ mô gồm:

- Tăng trưởng GRDP
- Chỉ số giá tiêu dùng (CPI)
- Lãi suất tái cấp vốn
- Tác động của COVID-19
- Giai đoạn giá nhà tăng trưởng nhanh

---

## Mục tiêu

- Phân tích xu hướng giá nhà tại TP.HCM.
- So sánh mức giá giữa các quận.
- Phân tích mối quan hệ giữa giá nhà và các yếu tố kinh tế vĩ mô.
- Xây dựng mô hình hồi quy tuyến tính OLS.
- Kiểm tra hiện tượng đa cộng tuyến bằng VIF.
- Xác định các yếu tố có ý nghĩa thống kê đối với giá nhà.

---

## Dataset

Dự án sử dụng các nhóm dữ liệu:

| Dataset | Nội dung |
|---|---|
| `HousePricingHCM_v2.csv` | Dữ liệu giá nhà tại 9 quận TP.HCM |
| `hcmc_grdp_2017_2022.csv` | Dữ liệu GRDP và tốc độ tăng trưởng GRDP |
| `vietnam_cpi_worldbank_2017_2022.csv` | Chỉ số giá tiêu dùng CPI |
| `vietnam_refinancing_rate_quarterly_2017_2022.csv` | Lãi suất tái cấp vốn theo quý |

Dữ liệu giá nhà ban đầu gồm 1.996 quan sát và 10 cột, trong đó có ngày tháng và dữ liệu giá của 9 quận.

---

## Quy trình phân tích

```text
Raw Data
   ↓
Data Cleaning
   ↓
Data Transformation
   ↓
Quarterly Aggregation
   ↓
Merge Economic Data
   ↓
Exploratory Data Analysis
   ↓
Correlation Analysis
   ↓
OLS Regression
   ↓
VIF Analysis
   ↓
Interpretation & Conclusion

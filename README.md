# 🛒 Retail Data Warehouse & OLAP Pipeline Project

## 📌 Tổng quan dự án (Project Overview)
- **Mục tiêu:** Xây dựng Data Warehouse và khối OLAP để phân tích dữ liệu bán lẻ, hỗ trợ ra quyết định kinh doanh.
- **Công cụ sử dụng:** SQL Server, SQL Server Integration Services (SSIS), SQL Server Analysis Services (SSAS), MDX.
- **Nguồn dữ liệu:** Flat files chứa ~10.000 bản ghi dữ liệu bán lẻ.

## 🏗️ Kiến trúc dữ liệu (Architecture)
## ⚙️ Chi tiết triển khai
### 1. ETL Pipeline (SSIS)
- Trích xuất dữ liệu từ Flat Files.
- Làm sạch và chuẩn hóa dữ liệu (xử lý null, chuẩn hóa định dạng ngày tháng...).
- Load dữ liệu vào SQL Server Data Warehouse tập trung.

### 2. Mô hình đa chiều - OLAP Cube (SSAS)
- Xây dựng các Dimension (ví dụ: Dim_Time, Dim_Product, Dim_Store) và Fact Table (Fact_Sales).
- Thiết lập phân cấp (Hierarchies) và mối quan hệ giữa các thực thể kinh doanh.

### 3. Phân tích dữ liệu (MDX Queries)
Sử dụng MDX để truy xuất các chỉ số quan trọng. Một số truy vấn nổi bật:
- Phân tích xu hướng doanh thu theo thời gian.
- Lọc hiệu suất bán hàng theo khu vực.



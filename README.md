# HỆ GỢI Ý SẢN PHẨM THỜI TRANG H&M

## 1. Giới thiệu bài toán
Cuộc thi **H&M Personalized Fashion Recommendations** trên Kaggle tập trung vào việc xây dựng hệ thống gợi ý sản phẩm thời trang cá nhân hóa dựa trên lịch sử mua sắm của người dùng. Mục tiêu chính là giúp H&M cung cấp các gợi ý sản phẩm phù hợp với từng người dùng dựa trên sở thích, thói quen mua sắm, và các đặc trưng của sản phẩm.

### Dữ liệu cung cấp
- **Người dùng (customers.csv):** Bao gồm các trường như `customer_id`, lịch sử mua hàng của từng người dùng.
- **Bài giới thiệu sản phẩm (articles.csv):** Gồm các trường như `article_id`, `brand`, `color`, `product_type`, thông tin chi tiết về sản phẩm.
- **Lịch sử giao dịch (transactions.csv):** Bao gồm thông tin về các giao dịch, thời gian mua sắm, sản phẩm mua.

---

## 2. Tiền xử lý dữ liệu
- **Mã hóa các biến phân loại**
- **Xử lý dữ liệu thiếu và ngoại lai**
- **Feature Engineering:**
  - Tính năng liên quan đến giao dịch khách hàng và sản phẩm
  - Tính năng liên quan đến sản phẩm cặp (pair features)
  - Tính năng liên quan đến mức độ phổ biến của sản phẩm
  - Tính năng liên quan đến tỷ lệ mua hàng theo phân khúc khách hàng
  - Tính năng liên quan đến giá cả
  - Tính năng liên quan đến độ tuổi khách hàng
  - Tính năng liên quan đến tần suất mua gần đây
  - Tính năng liên quan đến tỷ lệ mua lại
  - Tính năng liên quan đến kênh bán hàng

---

## 3. Mô hình sử dụng
- **LightGBM (Light Gradient Boosting Machine)**

---

## 4. Kết quả đánh giá
Kết quả đạt được trên tập kiểm tra là **0.02897** (đánh giá bằng Mean Average Precision at 12 (MAP@12)), cho thấy hệ thống khá tốt trong việc gợi ý chính xác sản phẩm trong danh sách top 12 cho từng khách hàng.

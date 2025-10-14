# 📊 DS101 Practice Notebooks

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

## Giới thiệu
Repository này chứa các bài thực hành và đồ án môn **DS101 - Xác suất Thống kê Chuyên sâu** tại **Trường Đại học Công nghệ Thông tin - ĐHQG TP.HCM**. Nội dung bao gồm các bài tập thực hành từ cơ bản đến nâng cao. Các giải pháp được trình bày để tham khảo và có thể chưa tối ưu.

**Thông tin tác giả**:
- **Tác giả**: Nguyễn Bảo Quân
- **MSSV**: 24521436
- **Trường**: Đại học Công nghệ Thông tin - ĐHQG TP.HCM

---
## Thực hành 1: Tìm hiểu thư viện
- Tìm hiểu và sử dụng các thư viện Python: `numpy`, `pandas`, `matplotlib.pyplot`, `scipy.stats`, ... để xử lý dữ liệu, vẽ đồ thị và tính toán thống kê.

## Thực hành 2: Bài tập xác suất và thống kê

### Mức 5 điểm
- **Mô phỏng phân phối**:
  - Thực hiện mô phỏng hàm mật độ của ít nhất 3 phân phối (ví dụ: nhị thức, Poisson, Gauss, mũ, ...).
- **Thống kê mô tả**:
  - Tạo file Excel hoặc CSV, đọc dữ liệu và thực hiện thống kê mô tả (trung bình, phương sai, trung vị, ...).
  - Lấy một tập dữ liệu từ Kaggle, tải lên Python và thực hiện thống kê mô tả.
- **Xác suất thống kê**:
  - Viết chương trình tính xác suất các mặt của xúc xắc bằng phương pháp thống kê.
  - Viết chương trình tính gần đúng số pi.
- **Kỳ vọng và phương sai**:
  - Tính kỳ vọng, phương sai của biến ngẫu nhiên X với hàm xác suất (PMF):
    ```
    X  | 0   | 1   | 2   | 3
    ---+-----+-----+-----+-----
    P  | 0.1 | 0.2 | 0.5 | 0.2
    ```
  - Tìm và vẽ hàm phân phối tích lũy (CDF) của X.
- **Xích Markov**:
  - Cho xích Markov với ma trận chuyển:
    ```
    0.8  0.2
    0.1  0.9
    ```
    Viết chương trình tìm phân phối dừng và xác định thời gian đạt phân phối dừng.
  - Cho xích Markov với ma trận chuyển:
    ```
    0.64  0.32  0.04
    0.40  0.59  0.10
    0.25  0.50  0.25
    ```
    Tìm phân phối dừng và thời gian đạt phân phối dừng.
- **Bước ngẫu nhiên**:
  - Mô phỏng quỹ đạo của quá trình bước ngẫu nhiên X(t) = sum(Y_i, i=0 to t), với Y_i = ±1:
    a) Xác suất 1/2.
    b) Xác suất p, 1-p, với p trong (0,1).
  - Vẽ 3 quỹ đạo trên cùng một đồ thị.

### Mức 7 điểm
- **Tích phân gần đúng**:
  - Tính diện tích miền giới hạn bởi y = sqrt(x) và y = x. So sánh với kết quả giải tích.
  - Tính tích phân hai lớp của hàm z = x^2 + y^2 trên miền:
    a) D = {(x,y) | x^2 + y^2 <= 1}.
    b) D = [0,1] x [0,1].
    So sánh với kết quả giải tích.
- **Xác suất phân phối chuẩn**:
  - Tính P(-1 < X < 2) với X ~ N(1,1) bằng:
    - Thư viện Python.
    - Phương pháp Monte-Carlo.
- **Sinh số ngẫu nhiên**:
  - Sinh số ngẫu nhiên 1, 2, 3, 4 với xác suất 0.1, 0.4, 0.3, 0.2.
  - Chứng minh kết quả bằng phương pháp Monte-Carlo.
- **Hàm Laplace**:
  - Tính gần đúng hàm Laplace cho phân phối chuẩn N(0,1). So sánh với kết quả từ `scipy.stats`.
- **Mô phỏng trò chơi**:
  - **Trò chơi xúc xắc**: Người A tung xúc xắc (1-100). Nếu ra 1-51, nhà cái thắng; 52-100, A thắng. Mô phỏng số tiền A thu được sau 10, 100, 10,000 lần chơi. So sánh với kỳ vọng lý thuyết (-1/50 USD).
  - **Trò chơi bầu cua**: Người chơi đặt a đồng vào ô "cua". Nếu có i > 0 mặt "cua" trong 3 hạt, thưởng i * a đồng; nếu không, mất a đồng. Đánh giá tính công bằng bằng Monte-Carlo.
- **Quá trình Wiener**:
  - Mô phỏng quỹ đạo của quá trình Wiener W(t) (chuyển động Brown) với:
    - W(0) = 0, liên tục, W(t) - W(s) ~ N(0, t-s).
    - Vẽ 3 quỹ đạo trên cùng một đồ thị.

### Mức 9 điểm
- **Dự đoán trạng thái**:
  - Cho 100 đoạn đường với 4 trạng thái (Tốt, Khá, Trung bình, Xấu) và ma trận chuyển:
    ```
    0.82  0.18  0.00  0.00
    0.00  0.73  0.27  0.00
    0.00  0.00  0.67  0.33
    0.00  0.00  0.00  1.00
    ```
    - Véc-tơ trạng thái ban đầu (2007): pi = [0.45, 0.32, 0.16, 0.07].
    - Dự đoán sự xuống cấp của các đoạn đường trong các năm tiếp theo.
- **Trung bình ngẫu nhiên**:
  - Tính trung bình theo thời gian và xác suất của một quá trình ngẫu nhiên.
  - Áp dụng vào một quá trình ngẫu nhiên cụ thể.
- **Thống kê suy diễn**:
  - Thực hiện bài toán thống kê suy diễn (khoảng tin cậy, kiểm định giả thuyết) cho trung bình, tỷ lệ, hoặc phương sai.
  - Áp dụng vào một bài toán cụ thể.

## Đồ án
- **Nội dung**: Đang cập nhật.

---

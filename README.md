# 📊 DS101 Practice Notebooks

- Repo này chứa các bài thực hành môn **DS101 - Xác suất thống kê chuyên sâu** cũng như đồ án môn học sẽ được lưu trong đây 
- Syntax cơ bản, hướng giải quyết có thể chưa được tối ưu nên đây chỉ là tài liệu để tham khảo. 
- Tác Giả: Nguyễn Bảo Quân
- MSSV: 24521436
- Trường Đại học Công nghệ Thông Tin - ĐHQG HCM 

# 📊 Thực hành 1: Tìm hiểu thư viện và cách dùng các hàm trong thư viện (numpy, pandas, matplotlib.pyplot, scipy.stats ...)
# 📊 Thực hành 2: 
- Mức 5Đ:
  + Thực hiện mô phỏng hàm mật độ của ít nhất 3 phân phối (chẳng hạn: nhị thức, Poisson, Gauss, mũ,...)
  + Tạo 1 file excel hoặc *.csv và thực hành đọc dữ liệu từ file này; thực hiện các thống kê mô tả và đọc kết quả hoặc thực hành lấy 1 file data trên Kaggle và tải lên python; thực hiện thống kê mô tả.
  + Viết chương trình Tính xác suất được các mặt bằng phương pháp thống kê.
  + Viết chương trình Tính gần đúng số Pi 
  + Viết chương trình Tính kỳ vọng, phương sai của X. Tìm hàm CDF của X và vẽ nó biết X có PMF bên dưới
                  X  0      1     2      3
                  P 0.1   0.2  0.5   0.2

  + Cho xích Markov có ma trận chuyển [[0.8  0.2] [0.1  0.9]]. Hãy viết chương trình python tìm phân phối dừng của Xích Markov. Hãy cho biết sau bao lâu thì xích Markov này đạt phân phối dừng.
  + Cho ma trận xác suất chuyển của xích Markov có dạng  
                        0.64 0.32 0.04
                        0.40 0.59 0.10
                        0.25 0.50 0.25
    Tìm phân phối dừng của xích Markov này. Hãy cho biết sau bao lâu thì xích Markov này đạt phân phối dừng.
  + Viết chương trình mô phỏng quỹ đạo của quá trình bước ngẫu nhiên X(t) X(t)=sum(i:0->t) Y_i, Y_i nhận giá trị +/- 1 
    a) với xác suất ½, 
    b) với xác suất p, 1-p. p là giá trị được xác định trước trong (0,1). Trình bày 3 quỹ đạo trên cùng một đồ thị.
- Mức 7đ:
  + Viết chương trình tính gần đúng diện tích miền được giới hạn bởi y=sqrt(x) và y=x. So sánh kết quả gần đúng với kết quả giải tích.
  + Viết chương trình  tính gần đúng tích phân hai lớp của hàm z=x^2+y^2 trên miền 
    a) D={(x,y)/x^2+y^2<=1.   b) D= [0,1]x[0,1]
    So sánh kết quả gần đúng từ chương trình với kết quả giải tích
  + Tính xác suất P(-1<X<2) với X~N(1,1) (N là phân phối chuẩn) bằng 2 cách: Sử dụng thư viện của python và tính gần đúng bằng phương pháp Monte-Carlo.
  + Viết chương trình sinh số ngẫu nhiên 1, 2, 3, 4 với xác suất theo thứ tự là 0.1, 0.4, 0.3, 0.2.
  + Viết chương trình chứng minh lại kết quả sinh số trên bằng phương pháp Monte-Carlo.
  + Tính gần đúng hàm Laplace ứng với phân phối chuẩn N(0,1). So sánh với kết quả lấy từ python trong thư viện scipy.stats: 
  + Xét trò chơi người A tung xúc xắc với các mặt từ 1-100. Nếu A được từ 1-51 thì nhà cái thắng, còn từ 52-100 thì người A thắng. Giả sử A cá 1 USD cho 1 game. Viết chương trình mô phỏng số tiền A thu về sau 10 lần cá, 100 lần cá, sau 10.000 lần cá. So sánh kết quả mô phỏng với kết quả      tính theo lý thuyết xác suất (TB = -1/50 USD). Mở rộng sang trò chơi bầu cua: 
    Giả sử một người đặt a đồng vào ô “cua” (một trong 6 ô có tên là: Bầu, cua, cá, gà, tôm cọp). Nhà cái sẽ tung 3 hạt  bầu cua. Nếu được i (i>0) mặt “cua” thì người chơi sẽ được thưởng i lần a đồng, còn nếu không được mặt “cua” nào thì người chơi bị mất a đồng đã đặt. Dùng mô phỏng         Monte-Carlo để đánh giá tính công bằng của trò chơi này. 
  + Viết chương trình mô phỏng quỹ đạo của quá trình Wiener W(t) (hay chuyển động Brown), trình bày k=3 quỹ đạo trên cùng một đồ thị.
    Định nghĩa: Quá trình Wiener thỏa: W(0)=0, W(t) liên tục, W(t)-W(s)~N(0, t-s), t>=s
- Mức 9đ: 
  + Giả sử có 100 đoạn đường với 4 trạng thái (1: Tốt, 2: Khá, 3: Trung Bình, 4: Xấu), không gian trạng thái S{1, 2, 3, 4}. Năm hiện tại là 2007 với véc-tơ trạng thái là π(0.45, 0.32, 0.16, 0.07), dựa vào dữ liệu ở năm 2006 và năm 2007 có được ma trận chuyển như bên dưới, và giả sử xác       suất thay đổi trạng thái của các đoạn đường là không đổi qua các năm. Dự đoán sự xuống cấp của 100 đoạn đường trong các năm tiếp theo.
                        0.82 0.18 0.00 0.00
                        0.00 0.73 0.27 0.00
                        0.00 0.00 0.67 0.33
                        0.00 0.00 0.00 1.00
  + Viết chương trình python tính trung bình theo thời gian, trung bình theo xác suất của một quá trình ngẫu nhiên. Áp dụng vào một QTNN cụ thể (lấy QTNN trong phần lý thuyết để trình bày).
  + Viết chương trình python thực hiện một trong các bài toán về thống kê suy diễn: Khoảng tin cậy gamma cho trung bình/tỉ lệ/phương sai; So sánh trung bình hoặc tỉ lệ với một số (bài toán kiểm định giả thuyết),... Áp dụng vào một bài toán cụ thể (SV có thể tham khảo các bài tập trong        môn học Xác suất thống kê).
- Mức 10đ
  + Tìm hiểu PCA và cài đặt: https://machinelearningcoban.com/2017/06/21/pca2/ . Sử dụng thư viện python và tập dữ liệu iris để thực hành PCA. Xác định số thành phần chính sao cho lượng tin giữ lại đạt 95%.
  + (CA) Tìm hiểu k-mean và cài đặt trong python: https://machinelearningcoban.com/2017/01/01/kmeans/ 
  + Kiểm định phi tham số: Thực hiện được ít nhất 1 bài kiểm định phi tham số
# 📊 Đồ án : ???

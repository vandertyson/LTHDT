# Kiểm tra giữa kỳ môn Lập trình hướng đối tượng

Mỗi sinh viên sẽ dùng số thứ tự của mình trong danh sách lớp (xem trong file danhsach.xlsx) làm mã (ID) của mình để đặt tên cho file
CSDL và biết những hồ sơ nào mình phải xử lý.

## Dữ liệu đầu vào
* File csdl-bk.csv chứa danh sách giả lập điểm thi THPT quốc gia của tất cả thí sinh đăng ký nguyện vọng xét tuyển vào ĐHBKHN
* File dangkynv-bk.csv chứa danh sách giả lập hồ sơ đăng ký nguyện vọng xét tuyển vào ĐHBKHN của tất cả thí sinh
* File TSBK_KhaoSat.PDF chứa thông tin về chỉ tiêu tuyển sinh và công thức tính điểm xét tuyển

## Yêu cầu
1. Tạo 1 project trên github để chứa kết quả của bài kiểm tra này
2. Tạo file CSDL dạng SQLite3 với tên theo quy tắc \<ID\>.db
3. Trong CSDL vừa tạo, tạo bảng nguyện vọng xét tuyển (nvxt) bằng câu lệnh sau: 
    
    *create table nvxt(sbd varchar(9), nvso int, manv varchar(4), diemxt double precision);*
    
4. Xử lý 100 hồ sơ đăng ký xét tuyển (trong file dangkynv-bk.csv) tương ứng với ID của mình (thí dụ sinh viên có ID là 1
sẽ xử lý 100 hồ sơ từ thứ 100 tới 199, sinh viên có ID là 2 sẽ xử lý 100 hồ sơ từ thứ 200 tới 299,...) và ghi kết quả vào bảng nvxt vừa tạo

5. Viết báo cáo (.doc) mô tả thuật toán, kết quả chạy chương trình. Public báo cáo, mã nguồn chương trình và file .db trong thư mục dự án trên github

6. Nộp báo cáo bản in và đường link tới thư mục dự án trên github (với số commit SHA xác định phiên bản) cho lớp trưởng (nhờ lớp trưởng tập hợp các đường link vào file excel giúp).

##Lưu ý
1. Chương trình có thể sử dụng các thư viện mã nguồn mở nhưng phải chỉ rõ nguồn trong chương trình và trong báo cáo
2. Sinh viên phải tự làm bài kiểm tra này, không được copy chương trình, báo cáo của bất kỳ ai và phải viết câu sau ở trang đầu của báo cáo "Tôi cam kết chương trình, kết quả chạy chương trình và báo cáo này do mình tự làm, không sao chép của bất cứ ai."

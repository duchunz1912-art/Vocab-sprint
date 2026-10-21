VOCAB SPRINT — GÓI PWA CHO IPHONE
==================================

Các file:
- index.html: giao diện và chức năng app
- words.json: dữ liệu từ vựng có nghĩa, IPA, cụm từ và ví dụ
- manifest.webmanifest: cấu hình cài lên màn hình chính
- sw.js: cache tài nguyên để dùng lại khi offline
- icon-192.png, icon-512.png: biểu tượng app

LƯU Ý QUAN TRỌNG VỀ SỐ LƯỢNG TỪ
Bản này có 145 mục từ đã có nghĩa, IPA, cụm từ và ví dụ. Đây là bộ khởi đầu có dữ liệu thật, chưa phải đủ 1.500 mục từ đã được kiểm duyệt. Mình không tự điền nghĩa/IPA giả chỉ để báo đủ số lượng. App đã có sẵn bộ khung học, quiz, phát âm bằng giọng đọc của iPhone, lịch ôn thông minh, tìm kiếm, tiến độ và xuất dữ liệu. Cần bổ sung thêm dữ liệu từ vựng đã kiểm duyệt vào words.json để đạt đủ 1.500 từ.

CÁCH DÙNG THỬ TRÊN MÁY TÍNH
1. Giải nén ZIP.
2. Mở terminal trong thư mục này và chạy: python3 -m http.server 8000
3. Mở http://localhost:8000

CÀI TRÊN IPHONE (CẦN HOSTING HTTPS)
1. Đưa toàn bộ file trong thư mục này lên một hosting hỗ trợ static site và HTTPS (ví dụ GitHub Pages).
2. Mở URL HTTPS vừa được tạo bằng Safari (không mở trong khung xem trước của ChatGPT).
3. Nhấn nút Chia sẻ ở Safari.
4. Chọn “Thêm vào Màn hình chính”.
5. Nếu thấy tùy chọn “Mở dưới dạng ứng dụng web”, bật tùy chọn đó rồi chọn Thêm.
6. Mở app từ biểu tượng Vocab Sprint trên màn hình chính.

LƯU Ý
- Không thể cài file HTML trực tiếp thành app native từ ZIP. Đây là PWA (web app cài lên màn hình chính).
- Tiến độ lưu trong bộ nhớ trình duyệt của thiết bị. Xóa dữ liệu Safari có thể làm mất tiến độ; hãy dùng “Xuất tiến độ” định kỳ.
- Phát âm dùng speechSynthesis của Safari/iOS; giọng và khả năng đọc có thể khác theo thiết lập iPhone.
- Cần truy cập HTTPS ít nhất lần đầu để cache tài nguyên. Sau khi cache xong, phần học cơ bản có thể hoạt động offline.

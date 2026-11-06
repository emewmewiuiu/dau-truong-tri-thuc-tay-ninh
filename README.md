# Đấu trường tri thức – Lịch sử Tây Ninh

## Chạy thử
- Giải nén ZIP.
- Mở `index.html` bằng trình duyệt hoặc dùng VS Code Live Server.
- Thí sinh: nhập họ tên và lớp/đội.
- MC: mật khẩu demo `mc123`.
- Admin: mật khẩu demo `admin123`.

## Đưa lên GitHub Pages
1. Tạo repository GitHub mới.
2. Tải toàn bộ nội dung thư mục này lên repository (giữ `index.html` và `app.js` ở thư mục gốc).
3. Vào **Settings → Pages**.
4. Chọn **Deploy from a branch**, chọn nhánh `main`, thư mục `/root`, nhấn Save.
5. Chờ GitHub Pages triển khai và mở URL được cung cấp.

## Tính năng
- 4 vòng thi, mỗi vòng 10 câu hỏi trắc nghiệm.
- Giao diện riêng cho thí sinh, MC và Admin.
- MC điều khiển mở vòng/câu hỏi, công bố đáp án, chuyển câu.
- Tự động cộng 10 điểm cho mỗi câu đúng; bảng xếp hạng.
- Admin sửa câu hỏi, đáp án, giải thích; nhập/xuất bộ câu hỏi JSON.
- Lưu dữ liệu bằng `localStorage`; đồng bộ giữa các tab cùng trình duyệt qua sự kiện storage.

## Lưu ý triển khai thực tế
GitHub Pages chỉ lưu trữ website tĩnh. Bản này dùng `localStorage`, vì vậy dữ liệu không đồng bộ giữa máy thí sinh và máy MC; mật khẩu demo cũng không phải bảo mật thực sự. Nếu muốn tổ chức thi trực tiếp trên nhiều điện thoại/máy tính, cần bổ sung backend như Firebase hoặc Supabase (xác thực, cơ sở dữ liệu và đồng bộ thời gian thực). Hãy kiểm chứng lại mốc/sự kiện lịch sử theo tài liệu chính thống của địa phương trước khi dùng trong cuộc thi chính thức.

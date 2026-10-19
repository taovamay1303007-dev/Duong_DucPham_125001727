# NHẬT KÝ PROMPT ENGINEERING (VIBE CODING LOG)
- **Họ và tên:** [Phạm Đức Dương]
- **MSSV:** [125001727]
- **Tên đề tài Website:** Website Nhận Dự Án & Quản Lý Tiến Độ Xây Dựng Cao Cấp (LUXCON Architecture & Construction Hub)
- **Công cụ AI đã sử dụng:** ChatGPT / Claude / Gemini / (Chọn công cụ bạn đã dùng)

---

## 1. Yêu cầu ban đầu (System/Initial Prompt)
> *Ghi lại prompt tổng quan ban đầu bạn dùng để khởi tạo khung website.*
> 
> **Prompt:** # MASTER PROMPT: WEBSITE NHẬN DỰ ÁN & QUẢN LÝ TIẾN ĐỘ XÂY DỰNG CAO CẤP (LUXCON HUB)

### 1. VAI TRÒ (ROLE)
Bạn là một **Senior Full-Stack Developer & UX/UI Designer hàng đầu**, chuyên thiết kế và lập trình các Web Application cao cấp dành cho các Tập đoàn Xây dựng, Kiến trúc và Bất động sản quốc tế.

### 2. BỐI CẢNH & MỤC TIÊU (CONTEXT & OBJECTIVE)
Tôi cần xây dựng một ứng dụng Web đơn trang (Single Page Application - SPA) đẳng cấp, hiện đại và sang trọng có tên **"LUXCON Architecture & Construction Hub"**. 
Website hướng tới đối tượng chủ đầu tư cao cấp, cung cấp trải nghiệm số toàn diện từ khâu tìm hiểu dịch vụ, xem dự án, tính chi phí tự động cho đến tra cứu tiến độ công trình thời gian thực.

---

### 3. YÊU CẦU THIẾT KẾ & TÍNH NĂNG CHI TIẾT (SPECIFICATIONS)

#### A. Phong cách Thiết kế (UI/UX Design Style)
- **Chủ đề (Theme):** Dark Mode Luxury / Premium Titanium.
- **Tông màu chủ đạo:** Slate/Black Titanium, kết hợp accent Gold Amber/Orange Gradient phản quang.
- **Phong cách:** Glassmorphism (hiệu ứng kính mờ `backdrop-blur`), hiệu ứng viền sáng glowing border, card hover chuyển động mượt mà (smooth transitions).
- **Cấu trúc Semantic HTML:** Bắt buộc sử dụng đúng các thẻ chuẩn SEO & Accessibility (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`).

#### B. Các Phân đoạn Chức năng (Key Features)
1. **Header & Navigation:** 
   - Logo thương hiệu sang trọng.
   - Menu điều hướng nhanh có hiệu ứng cuộn mượt (Smooth Scroll).
   - Nút Call-to-Action (CTA) nổi bật: "Báo Giá Nhanh" & "Tra Cứu Tiến Độ".

2. **Hero Section (Ấn tượng ban đầu):**
   - Tiêu đề hoành tráng, Slogan thể hiện vị thế dẫn đầu.
   - Thống kê chỉ số uy tín (500+ Dự án, 15+ Năm kinh nghiệm, 99% Hài lòng...).
   - Nút tương tác nhanh chuyển hướng tới Form hoặc Tool.

3. **Interactive Portfolio (Bộ sưu tập Dự án):**
   - Bộ lọc danh mục linh hoạt (Tất cả, Biệt thự Luxury, Nhà phố Hiện đại, Penthouse, Công trình công cộng).
   - Tích hợp **Modal xem chi tiết dự án**: Xem ngân sách, quy mô m2, bản vẽ 3D và slide gallery ảnh sắc nét khi click vào card dự án.

4. **Construction Cost Calculator (Công cụ Dự toán Chi phí Tự động):**
   - Nhập diện tích (m2) và số tầng.
   - Tùy chọn Loại móng (Đơn, Cọc, Băng, Bè), Loại mái (Bằng, Thái, Nhật, Tole).
   - Tùy chọn Gói vật tư (Tiêu chuẩn, Cao cấp, Sang trọng) và Phong cách kiến trúc.
   - **Xử lý JS:** Tự động tính tổng diện tích xây dựng (áp dụng hệ số móng/mái) và xuất bảng phân tích ngân sách dự kiến chi tiết.

5. **Interactive Process Timeline (Quy trình làm việc 6 bước):**
   - Minh họa trực quan 6 bước: Tiếp nhận -> Khảo sát -> Thiết kế -> Báo giá -> Thi công -> Bàn giao.
   - Hiệu ứng hoán đổi trạng thái tương tác mượt mà.

6. **Client Project Tracker Portal (Tra cứu Tiến độ Công trình):**
   - Cho phép nhập Mã dự án (Ví dụ thử nghiệm: `PROJ-2026` hoặc `PROJ-LUXURY`).
   - Màn hình hiển thị: Phần trăm hoàn thành, Nhật ký thi công live từng ngày, Tiến độ thanh toán đợt và Khung Live Camera/Webcam công trường giả lập.

7. **Project Registration Form (Form Nhận Dự án & Đặt lịch):**
   - Các trường nhập liệu: Họ tên, SĐT, Email, Loại công trình, Ngân sách dự kiến, Địa điểm thi công.
   - Giả lập tải lên file bản vẽ/mặt bằng (`.pdf`, `.dwg`, `.png`).
   - Xử lý JS xác nhận gửi thành công kèm mã tra cứu tự động sinh.

8. **24/7 AI Construction Assistant (Live Chatbot):**
   - Widget Chatbot cố định ở góc màn hình.
   - Xử lý kịch bản câu hỏi tự động (Tư vấn báo giá, Giấy phép xây dựng, Đặt lịch khảo sát).

---

### 4. YÊU CẦU KỸ THUẬT (TECHNICAL STACK)
- **Kiến trúc code:** Gói gọn trong **1 File HTML duy nhất** (`index.html`) dễ chạy thử nghiệm.
- **CSS Framework:** CDN Tailwind CSS (phiên bản mới nhất v3/v4).
- **Icon Library:** FontAwesome v6 CDN.
- **JavaScript:** ES6+ thuần (Vanilla JS), viết code sạch, tối ưu hàm, không lỗi console, phân chia module logic rõ ràng.

---

### 5. ĐỊNH DẠNG ĐẦU RA (OUTPUT FORMAT)
Nội dung trả về là mã nguồn HTML/JS/CSS hoàn chỉnh, có comment giải thích rõ ràng từng khối chức năng, không viết tắt hay bỏ dở code giữa chừng.

---

## 2. Quá trình tinh chỉnh & Giải quyết sự cố (Iteration Iterations)

### Lần 1: Dựng khung Semantic HTML & CSS Variable / Tailwind CSS
- **Prompt đã dùng:** "Tôi muốn website có giao diện Dark Mode hoành tráng, tông màu Titanium/Gold Amber, sử dụng hiệu ứng Glassmorphism. Cần có các phần: Hero section có chỉ số thống kê, Bộ sưu tập dự án (Portfolio) có bộ lọc thể loại, và Form đăng ký/nhận dự án xây dựng đầy đủ các trường dữ liệu."
- **Kết quả AI tạo ra:** AI đã tạo ra khung HTML giao diện tối, hỗ trợ bộ lọc dự án bằng JS, có form đăng ký đính kèm file và các thẻ thống kê ấn tượng.
- **Nhận xét & Tinh chỉnh của SV:** AI sử dụng một số thẻ `<div>` lặp lại nhiều cho phần danh sách dự án và quy trình. Tôi đã nhắc AI tối ưu lại cấu trúc bằng các thẻ Semantic HTML như `<main>`, `<section>`, `<article>`, `<header>`, `<footer>` để chuẩn SEO và tối ưu accessibility.

### Lần 2: Tích hợp công cụ tính chi phí, Client Portal và Live Chat AI
- **Prompt đã dùng:** "Làm lại tương tự nhưng nâng cấp thêm tính năng nâng cao: Công cụ tính toán chi phí xây dựng (Cost Estimator) tự động theo m2/móng/mái, Client Portal cho phép nhập mã dự án (PROJ-2026) để xem tiến độ/camera công trình, và một khung Live Chatbot AI tư vấn 24/7."
- **Kết quả AI tạo ra:** AI đã nâng cấp toàn bộ ứng dụng thành 1 file HTML hoàn chỉnh tích hợp Tailwind CSS, bổ sung modal tính chi phí tự động, màn hình tra cứu tiến độ thi công công trình và tính năng Chatbot trả lời theo kịch bản.
- **Thách thức gặp phải:**
  - Logic tính toán chi phí xây dựng ban đầu bị nhảy giá không chính xác khi đổi phong cách kiến trúc.
  - Cửa sổ Modal chi tiết dự án không đóng được khi click ra ngoài vùng backdrop.
- **Cách sửa prompt (Debug prompt):** "Hãy kiểm tra lại hàm JavaScript `calculateCost()`, đảm bảo nhân đúng hệ số diện tích móng, mái và loại vật liệu. Đồng thời thêm sự kiện `addEventListener('click')` cho vùng ngoài Modal để người dùng có thể tắt Modal dễ dàng."

---

## 3. Đánh giá cá nhân về quá trình Vibe Coding
- **AI đã giúp bạn tiết kiệm thời gian ở phần nào nhất?**
  - Tiết kiệm hơn 80% thời gian trong việc viết các lớp CSS phức tạp (Tailwind CSS) cho giao diện Dark Mode Glassmorphism.
  - Tự động sinh ra cấu trúc JavaScript xử lý logic tính toán chi phí và lọc dữ liệu mượt mà mà không cần cài đặt thêm library bên ngoài.
- **Bài học rút ra khi đặt câu hỏi (Prompt) cho AI trong thiết kế web?**
  - **Mô tả bối cảnh rõ ràng:** Cần định hình rõ vai trò của AI (ví dụ: *Chuyên gia Lập trình Web Senior*), phong cách thiết kế (*Dark Luxury, Glassmorphism*), và đối tượng người dùng (*Chủ đầu tư, Khách hàng xây nhà*).
  - **Chia nhỏ tính năng:** Yêu cầu AI từng bước hoặc đưa ra danh sách tính năng cụ thể (Form, Calculator, Client Portal, Chatbot) thay vì chỉ nói chung chung.
  - **Kiểm soát Semantic & Clean Code:** Luôn kiểm tra và nhắc nhở AI tuân thủ chuẩn Semantic HTML, viết code gọn gàng, có comment giải thích rõ ràng.
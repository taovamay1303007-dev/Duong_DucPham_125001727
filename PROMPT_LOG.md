# NHẬT KÝ PROMPT ENGINEERING (VIBE CODING LOG)
- **Họ và tên:** [ĐIỀN HỌ TÊN]
- **MSSV:** [ĐIỀN MSSV]
- **Tên đề tài Website:** Rang Coffee - Landing Page quán cà phê rang xay thủ công
- **Công cụ AI đã sử dụng:** Claude (Anthropic)

## 1. Yêu cầu ban đầu (System/Initial Prompt)
> Tạo landing page cho quán cà phê rang xay "Rang Coffee" bằng HTML/CSS thuần (index.html, style.css, thư mục assets/). Bắt buộc dùng Semantic HTML5 (header, nav, main, section, article, footer), hạn chế thẻ div. Dùng CSS Variables trong :root cho màu, font, spacing. Layout dùng Flexbox và Grid, responsive. Tích hợp Animate.css cho hero/tiêu đề/nút CTA và AOS cho các section khi cuộn. Tự viết hiệu ứng :hover, :focus cho nút và card. Tông màu nâu cà phê ấm, tiếng Việt, các phần: Hero, Câu chuyện, Thực đơn, Vì sao chọn, Liên hệ.

## 2. Quá trình tinh chỉnh & Giải quyết sự cố (Iteration)

### Lần 1: Dựng khung Semantic HTML & CSS Variable
- **Prompt đã dùng:** "Dựng khung trang với header > nav, main chứa các section, footer chứa address và copyright. Khai báo CSS Variables cho màu, font, spacing, radius, shadow."
- **Kết quả AI tạo ra:** Khung HTML với header, nav, main, 5 section, article cho từng card, figure/figcaption, address trong footer; :root có ~15 biến.
- **Nhận xét & Tinh chỉnh của SV:** [Ghi nhận xét của bạn, ví dụ: danh sách card ban đầu dùng div, đã yêu cầu đổi sang ul > li > article cho đúng ngữ nghĩa.]

### Lần 2: Tích hợp thư viện Animate.css & AOS
- **Prompt đã dùng:** "Thêm Animate.css qua CDN cho h1, đoạn mô tả và nút CTA ở hero. Thêm AOS cho các section bên dưới, dùng delay so le cho các card."
- **Kết quả AI tạo ra:** Link CDN Animate.css 4.1.1 và AOS 2.3.4, class animate__ ở hero, thuộc tính data-aos ở các section, gọi AOS.init() ở cuối body.
- **Thách thức gặp phải:** [Ví dụ: AOS không chạy khi cuộn trang / hiệu ứng lặp lại gây rối mắt.]
- **Cách sửa prompt (Debug prompt):** [Ví dụ: "AOS không hiện, kiểm tra thứ tự nạp script và đặt once: true để hiệu ứng chỉ chạy một lần."]

### Lần 3: Hiệu ứng :hover/:focus, responsive và hoàn thiện UI
- **Prompt đã dùng:** "Viết hiệu ứng hover/focus-visible cho nút, card, link nav, ô input. Thêm media query cho màn hình nhỏ và prefers-reduced-motion."
- **Kết quả AI tạo ra:** Card nâng lên khi hover, nút đổi màu và nổi, input có viền focus; grid chuyển 1 cột trên mobile.
- **Nhận xét & Tinh chỉnh của SV:** [Ghi nhận xét, ví dụ: giảm độ nảy của nút CTA cho đỡ chói mắt.]

### Lần 4: Thiết kế lại giao diện chuyên nghiệp, bắt mắt hơn
- **Prompt đã dùng:** "Làm lại trang web giao diện chuyên nghiệp bắt mắt hơn" (giữ nguyên các yêu cầu Semantic HTML5, CSS Variables, Flexbox/Grid, Animate.css, AOS).
- **Kết quả AI tạo ra:** Bảng màu mới lấy từ các giai đoạn của hạt cà phê, font Fraunces + Be Vietnam Pro, hero có biểu đồ đường cong nhiệt độ mẻ rang vẽ bằng SVG, hạt cà phê vẽ bằng CSS, menu bố cục bất đối xứng, form báo kết quả ngay trên trang.
- **Nhận xét & Tinh chỉnh của SV:** [Ghi nhận xét của bạn, ví dụ: màu nào cần chỉnh, hiệu ứng nào thấy rối mắt và đã yêu cầu giảm.]

### Lần 5: Đưa lên GitHub Pages
- **Prompt đã dùng:** "Hướng dẫn tạo repo Ten_Ho_MSSV, push code và bật GitHub Pages."
- **Kết quả AI tạo ra:** Các bước git init, commit, push và bật Pages ở Settings > Pages.
- **Nhận xét & Tinh chỉnh của SV:** [Ghi lại link live của bạn.]

## 3. Đánh giá cá nhân về quá trình Vibe Coding
- **AI đã giúp bạn tiết kiệm thời gian ở phần nào nhất?** [Ví dụ: dựng khung HTML/CSS và viết sẵn bộ biến màu, spacing.]
- **Bài học rút ra khi đặt câu hỏi (Prompt) cho AI trong thiết kế web?** [Ví dụ: nêu rõ ràng buộc kỹ thuật (thẻ ngữ nghĩa, CSS Variables) ngay từ đầu, và chia nhỏ yêu cầu thành từng bước để dễ kiểm tra, sửa lỗi.]

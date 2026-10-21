# E-commerce UI Improvement

## 1. Giới thiệu
Đây là bài tập cá nhân Chương 1 môn Phát triển ứng dụng WEB/TMĐT. Dự án tập trung vào việc khảo sát các website thương mại điện tử thực tế và thực hiện cải tiến giao diện khu vực hiển thị **Thẻ sản phẩm (Product Card)** nhằm tối ưu hóa trải nghiệm người dùng (UI/UX).

## 2. Website tham khảo
- **Tên website:** Grimm DC
- **URL:** https://grimmdc.com/
- **Khu vực đã khảo sát:** Trang chủ, Danh mục sản phẩm, Chi tiết sản phẩm, Tìm kiếm, Giỏ hàng.
- **Khu vực chọn để cải tiến:** Giao diện Thẻ sản phẩm (thuộc Trang chủ / Danh mục sản phẩm).

## 3. Chức năng
- Hiển thị danh sách sản phẩm theo dạng lưới (Grid layout).
- Hiển thị đầy đủ trực quan: hình ảnh, nhãn giảm giá (Sale badge), tên sản phẩm, giá gốc (gạch ngang) và giá khuyến mãi.
- Nút thao tác "Thêm vào giỏ" (Call-to-Action) hiển thị trực tiếp.
- Bố cục responsive hỗ trợ nhiều kích thước màn hình: hiển thị 4 sản phẩm/hàng trên máy tính và 2 sản phẩm/hàng trên điện thoại.

## 4. Công nghệ
- HTML5 (Cấu trúc giao diện)
- CSS3 (Tổ chức layout với Grid, Flexbox và Media Queries)

## 5. Cách chạy
- Clone repository này về máy tính.
- Mở file `index.html` bằng bất kỳ trình duyệt web nào (Google Chrome, Microsoft Edge, Safari,...).
- Khuyến nghị dùng Chrome DevTools (F12) > Toggle Device Toolbar để kiểm tra giao diện trên màn hình điện thoại.
- *Xem trực tiếp (Live Demo):* [Chèn link GitHub Pages của bạn vào đây nếu có]

## 6. Cải tiến đã thực hiện
- **Vấn đề ban đầu:** Trên một số giao diện thực tế và mobile, thẻ sản phẩm chưa làm nổi bật được giá khuyến mãi, tỷ lệ giảm giá (%), đồng thời người dùng phải bấm vào trang chi tiết mới có thể thêm hàng vào giỏ, gây kéo dài hành trình mua sắm.
- **Thay đổi đã thực hiện:** 
  1. Thiết kế lại thẻ sản phẩm tích hợp nhãn `-X%` nổi bật ở góc ảnh. 
  2. Hiển thị song song giá gốc và giá bán để kích thích quyết định mua. 
  3. Bổ sung nút "Thêm vào giỏ" ngay trên thẻ. 
  4. Tôi đã tự tinh chỉnh mã CSS: đổi màu nền (background-color) của nút "Thêm vào giỏ" thành màu xanh cyan (`#0ee4ff`) và chữ màu đen để tăng độ tương phản, giúp nút bấm nổi bật hơn hẳn so với nền trắng, thu hút sự chú ý của người dùng.

## 7. Hỗ trợ từ AI
- **Phần AI hỗ trợ:** Phân tích ưu nhược điểm của website Grimm DC, đề xuất cấu trúc HTML ngữ nghĩa (semantic) và khung CSS (sử dụng CSS Grid để chia cột). AI cũng hỗ trợ tạo bộ khung mã nguồn cơ bản.
- **Phần tôi đã kiểm tra và điều chỉnh:** Tôi đã đối chiếu kết quả phân tích của AI với website gốc, gạch bỏ những tính năng AI tự bịa ra (như bộ lọc màu sắc, kích thước không hề có trên Grimm DC). Về phần code, tôi đã chạy thử, kiểm tra responsive trên Chrome DevTools, tự tay điều chỉnh lại màu sắc (background-color, color) và giải thích được nguyên lý hoạt động của Flexbox/Grid trong bài làm.

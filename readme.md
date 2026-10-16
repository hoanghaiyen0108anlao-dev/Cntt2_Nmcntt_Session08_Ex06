# PHẦN 1. PHÂN TÍCH

## 1. Những sai lầm trong tư duy của Nam

**Sai lầm 1: Sử dụng Rich Text (.docx) để viết tài liệu dự án trên GitHub.**

- File Word chứa nội dung và nhiều thông tin định dạng như phông chữ, màu sắc, bố cục.
- Git khó so sánh trực tiếp những thay đổi nhỏ bên trong file `.docx`.
- Markdown (`.md`) là văn bản thuần, hiển thị trực tiếp trên GitHub và hỗ trợ Git Diff theo từng dòng.

**Sai lầm 2: Cho rằng Word phù hợp để quản lý phiên bản tài liệu dự án.**

- Khi sửa một dấu phẩy, Git có thể không hiển thị rõ thay đổi bên trong file Word.
- Với Markdown, Git Diff có thể chỉ ra chính xác dòng nào được thêm, sửa hoặc xóa, giúp nhóm dễ phát hiện và giải quyết xung đột.

## 2. Tại sao Markdown an toàn và nhẹ hơn?

| Tiêu chí | Word (.docx) | Markdown (.md) |
|---|---|---|
| Bản chất | Định dạng tài liệu phức tạp | Văn bản thuần |
| Dung lượng | Thường lớn hơn | Thường nhẹ hơn |
| Git Diff | Khó đọc thay đổi trực tiếp | So sánh từng dòng |
| GitHub | Có thể cần công cụ hỗ trợ | Hiển thị trực tiếp |
| Khả năng phục hồi | Có thể khó khôi phục khi cấu trúc tệp hỏng | Dễ đọc, sửa bằng trình soạn thảo văn bản |

## 3. Đối chiếu bẫy dữ liệu

- **File Word:** Nếu mất một byte làm hỏng cấu trúc ZIP/XML, file có thể không mở được hoặc bị lỗi một phần.
- **File Markdown:** Nếu mất một byte, thường chỉ một ký tự hoặc một phần nội dung bị ảnh hưởng; phần văn bản còn lại vẫn có thể đọc và chỉnh sửa.

*Lưu ý:* Không phải cứ mất một byte là file Word hỏng hoàn toàn. Mức độ hư hại phụ thuộc vào vị trí dữ liệu bị mất.

## 4. Kết luận

Nam nên sử dụng Markdown để viết tài liệu `README.md` cho dự án GreenTech vì Markdown nhẹ, dễ đọc, hiển thị trực tiếp trên GitHub và hỗ trợ Git Diff hiệu quả, giúp các thành viên cộng tác và quản lý phiên bản thuận tiện hơn.
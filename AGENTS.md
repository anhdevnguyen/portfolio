# AGENTS.md - Portfolio

## Project Identity
- Name: Portfolio
- Purpose: Website portfolio cá nhân
- Stack: HTML/CSS/JS thuần (vanilla), không framework, không build tool
- Knowledge Base: D:\DEV\Knowledge\DevKnowledge\01-Projects\Portfolio\

## Architecture Rules
- Cấu trúc: assets/, css/, js/, data/, tests/. Giữ nguyên convention này, không tự ý thêm build tool/framework mà không hỏi trước.
- index.html và project-detail.html là 2 entry point chính.

## Configuration Rules
- manifest.json, robots.txt, sitemap.xml phục vụ SEO/PWA — kiểm tra nội dung hiện tại trước khi sửa, tránh phá vỡ metadata.

## Testing Rules
- Có thư mục tests/ — kiểm tra cách chạy test hiện tại (đọc README.md của project) trước khi thêm test mới.
- Mở thử index.html/project-detail.html trên trình duyệt để verify thay đổi UI bằng mắt.

## Documentation Rules
- Thay đổi cấu trúc lớn (thêm framework, đổi cách tổ chức file) → ghi ADR trong 01-Projects\Portfolio\decisions\.

## AI Rules
Agent phải theo thứ tự:
1. Inspect repository (cấu trúc, git status)
2. Đọc AGENTS.md này
3. Đọc README.md của project (đã có sẵn, ưu tiên đọc trước Knowledge Base vì đây là project đơn giản)
4. Thực hiện thay đổi nhỏ nhất cần thiết
5. Verify bằng mắt trên trình duyệt
6. Review git diff

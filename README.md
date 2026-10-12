# Bài 4: Khai báo GitHub Secrets và cấu hình Đăng nhập Container Registry

Thư mục này chứa tệp cấu hình CI (`.github/workflows/ci.yml`) để thiết lập xác thực đăng nhập tự động vào GitHub Container Registry (GHCR).

## Yêu cầu đối với GitHub Repository
Để workflow này chạy thành công, bạn cần cấu hình trên GitHub như sau:
1. Truy cập **Settings -> Developer Settings -> Personal access tokens -> Tokens (classic)** và tạo token mới với quyền `write:packages`.
2. Vào **Settings -> Secrets and variables -> Actions** của Repository chứa mã nguồn.
3. Tạo Secret mới có tên `REGISTRY_TOKEN` và dán token vừa tạo vào.

## Sản phẩm nộp bài
- File `.github/workflows/ci.yml` (đã cung cấp trong thư mục này).
- **Lưu ý**: Bạn cần chụp ảnh màn hình mục **Repository Secrets** trên GitHub cho thấy biến `REGISTRY_TOKEN` đã được tạo để hoàn thiện bài nộp.

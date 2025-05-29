# Docker Redis

Triển khai Redis bằng Docker Compose với cấu hình password.

## Hướng dẫn sử dụng

1. Tạo file `.env` từ mẫu:

   ```bash
   cp .env.example .env
   ```

   Sau đó chỉnh sửa giá trị password và tên container nếu cần.

2. Khởi động Redis:

   ```bash
   docker-compose up -d
   ```

3. Kết nối Redis:
   - Host: `localhost`
   - Port: `6379`
   - Password: giá trị `REDIS_PASSWORD` trong file `.env`

## Cấu trúc file

- `docker-compose.yml`: Cấu hình dịch vụ Redis.
- `.env.example`: Mẫu biến môi trường.
- `.gitignore`: Loại trừ file/thư mục không cần thiết khỏi git.

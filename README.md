# Docker Redis

Triển khai Redis bằng Docker Compose với cấu hình password.

## Hướng dẫn sử dụng

1. Tạo Docker network dùng chung (nếu chưa có):

   ```bash
   docker network create share-network
   ```

2. Tạo file `.env` từ mẫu:

   ```bash
   cp .env.example .env
   ```

   Sau đó chỉnh sửa giá trị password và tên container nếu cần.

3. Khởi động Redis:

   ```bash
   docker-compose up -d
   ```

4. Kết nối Redis:
   - Host: `localhost`
   - Port: `6379`
   - Password: giá trị `REDIS_PASSWORD` trong file `.env`

## Cấu trúc file

- `docker-compose.yml`: Cấu hình dịch vụ Redis.
- `.env.example`: Mẫu biến môi trường.
- `.gitignore`: Loại trừ file/thư mục không cần thiết khỏi git.

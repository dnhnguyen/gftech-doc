# Tài liệu API Đăng Nhập

## URL
- **URL**: `https://api-sanbox.bhdt.vn/api/auth/login`

## Mô tả đầu vào (Request)

- **Phương thức (Method)**: `POST`
- **Header**:
  - `Content-Type: application/json`
- **Dữ liệu yêu cầu (Request Data)**:
  ```json
  {
      "username": "0376024652",
      "password": "a13456789@1"
  }
  
## Mô tả đầu ra (Response)
- **Phản hồi thành công (Success Response) **:
  ```json
  {
        "data": {
            "id": 1,
            "username": "0376024652",
            "token": "eyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ7XCJp...",
            "apiKey": "SJTSNGJUYCqGVCmJKUHU",
            "roles": "Lấy Roles trong JWToken",
            "ipAddress": "118.70.175.108"
        },
        "code": 1,
        "message": "Đăng nhập thành công"   
    }
## Phản hồi lỗi (Response)
  ```json
  {
      "code": 0,
      "message": "Tài khoản không tồn tại"
  }
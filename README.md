# Practice-Postman

## Mục tiêu:

- Nắm vững các khái niệm cơ bản về kiểm thử API.
- Rèn luyện kỹ năng sử dụng Postman để thực hiện các thao tác kiểm thử API.
- Áp dụng kiến thức đã học để thực hiện một bài tập thực tế.

## API Được Chọn

- https://jsonplaceholder.typicode.com/todos một danh sách các công việc với thông tin đầy đủ.

## API Endpoints

1. Kiểm Thử 1: Lấy thông tin của một người dùng cụ thể


   - **URL**: `https://jsonplaceholder.typicode.com/todos/23`
   - **Method**: POST
   - **Expected Response Code**: `201 Created` -![alt text](kt1.jpeg)

2. **Get Users (GET)**

   - **URL**: `https://jsonplaceholder.typicode.com/users`
   - **Method**: GET
   - **Expected Response Code**: `200 OK`
   - ![alt text](image.png)

3. **Update User (PUT)**

   - **URL**: `https://jsonplaceholder.typicode.com/users/1`
   - **Method**: PUT
   - **Request Body**:
     ```json
     {
       "name": "John Doe Updated",
       "email": "johndoe_updated@example.com",
       "phone": "1-770-736-8031",
       "website": "johndoeupdated.com"
     }
     ```
   - **Expected Response Code**: `200 OK`
   - ![alt text](image-2.png)

4. **Delete User (DELETE)**
   - **URL**: `https://jsonplaceholder.typicode.com/users/1`
   - **Method**: DELETE
   - **Expected Response Code**: `200 OK`
   - ![alt text](image-3.png)

## Báo Cáo Kiểm Thử Chi Tiết

1. Mục Tiêu Kiểm Thử:
   - Kiểm thử các chức năng cơ bản của API quản lý người dùng bao gồm tạo mới người dùng, xem danh sách người dùng, cập nhật thông tin người dùng và xóa người dùng.
   - Đảm bảo rằng các phương thức GET, POST, PUT và DELETE hoạt động chính xác và trả về kết quả mong đợi.
2. Phạm Vi Kiểm Thử:
   - Kiểm thử tất cả các endpoint của API:
     - GET /users
     - POST /users
     - PUT /users/{id}
     - DELETE /users/{id}
3. Kết Quả Kiểm Thử:
   - GET /users:
     - Kết quả: Thành công
     - Mô tả: API trả về danh sách các người dùng như mong đợi.
   - POST /users:
     - Kết quả: Thành công
     - Mô tả: API tạo mới người dùng và trả về thông tin của người dùng mới.
   - PUT /users/{id}:
     - Kết quả: Thành công
     - Mô tả: API cập nhật thông tin của người dùng có ID tương ứng.
   - DELETE /users/{id}:
     - Kết quả: Thành công
     - Mô tả: API xóa người dùng có ID tương ứng.
4. Khuyến Nghị:
   - Kiểm thử bổ sung: Tiếp tục kiểm thử để đảm bảo tính toàn vẹn và độ tin cậy của API trong các điều kiện và tình huống khác nhau, bao gồm kiểm thử với dữ liệu đầu vào không hợp lệ.
   - Tài liệu API chi tiết: Bổ sung tài liệu API với các ví dụ và hướng dẫn cụ thể cho các khách hàng và nhà phát triển sử dụng API.
   - Xác thực và phân quyền: Đảm bảo rằng API đã triển khai các cơ chế xác thực và phân quyền mạnh mẽ để bảo vệ dữ liệu người dùng.
   - Giảm thiểu lỗi: Kiểm tra các điều kiện biên và xử lý lỗi để giảm thiểu lỗi và cải thiện trải nghiệm người dùng cuối.
# HTTP request

Định nghĩa: Cho phép bạn gửi yêu cầu HTTP/HTTPS đến máy chủ web. Nó cũng cho phép bạn kiểm soát việc JMeter có phân tích cú pháp các tệp HTML để tìm hình ảnh và các tài nguyên nhúng khác hay không và gửi các yêu cầu HTTP để truy xuất chúng



|                            |                                                                                                                                                                                                                                              |       |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----- |
| Name                       | Mô tả cho mẫu này được hiển thị trong tree                                                                                                                                                                                                   | Không |
| Request                    | Tên miền hoặc địa chỉ IP của máy chủ web                                                                                                                                                                                                     | Có    |
| Content encoding           | Mã hóa nội dung sẽ được sử dụng (cho POST , PUT , PATCH và FILE ). Đây là mã hóa ký tự sẽ được sử dụng và không liên quan đến tiêu đề HTTP Content-Encoding.                                                                                 |       |
| Redirect Automatically     | Tự động theo dõi các chuyển hướng, do đó JMeter không nhìn thấy chúng và do đó sẽ không xuất hiện dưới dạng mẫu. Chỉ nên sử dụng cho các yêu cầu GET và HEAD . Trình lấy mẫu HttpClient sẽ từ chối các nỗ lực sử dụng nó cho POST hoặc PUT . |       |
| Follow Redirect            | Chỉ có hiệu lực nếu " Tự động chuyển hướng " không được bật.                                                                                                                                                                                 |       |
| Use keepalive              |                                                                                                                                                                                                                                              |       |
| Use multipart/form-data    |                                                                                                                                                                                                                                              |       |
| Browser-compatible headers |                                                                                                                                                                                                                                              |       |
| Parameter name             |                                                                                                                                                                                                                                              |       |


# Jsr223 assertion

Định nghĩa: Xác nhận JSR223 cho phép sử dụng mã lệnh JSR223 để kiểm tra trạng thái của mẫu trước đó.



| Thuộc tính                         | Mô tả                                                                                                                                                                                                                                            | Yêu cầu |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------- |
| Name                               | Mô tả tên cho phần tử này được hiển thị trong tree                                                                                                                                                                                               | Không   |
| Language                           | Ngôn ngữ JSR223 được sử dụng                                                                                                                                                                                                                     | Có      |
| Parameter                          | <p>Các tham số để truyền vào tập lệnh. Các tham số được lưu trữ trong các biến sau:</p><ul><li>Parameters - chuỗi chứa các tham số dưới dạng một biến duy nhất</li><li>args - Mảng chuỗi chứa các tham số, phân tách theo khoảng trắng</li></ul> | Không   |
| File Name                          | Một tệp chứa tập lệnh để chạy, nếu sử dụng đường dẫn tệp tương đối, thì nó sẽ tương đối với thư mục được tham chiếu bởi thuộc tính hệ thống                                                                                                      | Không   |
| Cache compiled script if available | sử dụng để lưu trữ kết quả biên dịch Script nếu ngôn ngữ được sử dụng hỗ trợ giao diện                                                                                                                                                           | Không   |
| Script                             | Tập lệnh để chạy                                                                                                                                                                                                                                 |         |

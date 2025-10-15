# JSR223 PreProcessor

Định nghĩa: Bộ xử lý trước JSR223 cho phép áp dụng mã lệnh JSR223 trước khi lấy mẫu



| Thuộc tính                         | Mô tả                                                                                                                                                                                                                                                                                                       | Yêu cầu |
| ---------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------- |
| Name                               | Mô tả cho phần tử này được hiển thị trong tree                                                                                                                                                                                                                                                              | Không   |
| Language                           | Ngôn ngữ JSR223 được sử dụng                                                                                                                                                                                                                                                                                | Có      |
| Parameter                          | <p></p><p>Các tham số để truyền vào tập lệnh. Các tham số được lưu trữ trong các biến sau:</p><ul><li>Tham số - chuỗi chứa các tham số dưới dạng một biến duy nhất</li><li>args - Mảng chuỗi chứa các tham số, phân tách theo khoảng trắng</li></ul>                                                        | Không   |
| File Name                          | Một tệp chứa tập lệnh để chạy, nếu sử dụng đường dẫn tệp tương đối, thì nó sẽ tương đối với thư mục được tham chiếu bởi thuộc tính hệ thống " user.dir "                                                                                                                                                    | Không   |
| Cache compiled script if available | Chuỗi duy nhất trên toàn bộ Kế hoạch kiểm tra mà JMeter sẽ sử dụng để lưu trữ kết quả biên dịch Script nếu ngôn ngữ được sử dụng hỗ trợ giao diện [Compilable](https://docs.oracle.com/javase/8/docs/api/javax/script/Compilable.html) (Groovy là một trong số đó, java, beanshell và javascript thì không) | Không   |
| Script                             | Tập lệnh để chạy                                                                                                                                                                                                                                                                                            | Có      |


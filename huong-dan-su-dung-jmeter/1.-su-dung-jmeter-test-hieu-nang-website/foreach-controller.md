# Foreach controller

Hãy tưởng tượng tình huống này: Bạn cần thực hiện cùng một hành động nhiều lần — chẳng hạn như truy cập tất cả các liên kết trên một trang web hoặc đặt chuyến bay từ tất cả các sân bay có thể. Thay vì sao chép và dán yêu cầu nhiều lần hoặc lưu thủ công danh sách các liên kết hoặc đích đến, bạn có thể lấy danh sách một cách động và lưu vào Biến JMeter. Sau đó, bạn có thể để Bộ điều khiển ForEach chạy một  [Sampler](https://www.blazemeter.com/blog/jmeter-dummy-sampler) (hoặc nhiều Sampler) cho mỗi biến trong danh sách

Định nghĩa: Foreach controller lặp qua các giá trị của một tập hợp các biến liên quan.Khi bạn thêm các bộ lấy mẫu (hoặc bộ điều khiển) vào Foreach controller , mỗi mẫu (hoặc bộ điều khiển) được thực thi một hoặc nhiều lần, trong đó trong mỗi vòng lặp, biến có một giá trị mới. Đầu vào phải bao gồm một số biến, mỗi biến được mở rộng bằng một dấu gạch dưới và một số. Mỗi biến như vậy phải có một giá trị. Vì vậy, ví dụ khi biến đầu vào có tên là inputVar , các biến sau đây phải được định nghĩa:

* inputVar\_1 = wendy
* inputVar\_2 = charles
* inputVar\_3 = peter
* inputVar\_4 = john

Lưu ý: dấu phân cách " \_ " hiện là tùy chọn.



| Thuộc tính                     | Mô tả                                                                                                                            | Bắt buộc |
| ------------------------------ | -------------------------------------------------------------------------------------------------------------------------------- | -------- |
| Name                           | Mô tả tên cho bộ điều khiển này được hiển thị trong Tree                                                                         | Không    |
| Comment                        | Mô tả nội dung cần giải thích, lưu ý,...                                                                                         | Không    |
| Input variable prefix          | Tiền tố cho tên biến được sử dụng làm đầu vào. Mặc định là chuỗi rỗng làm tiền tố.                                               | Không    |
| Start index for loop           | Chỉ mục bắt đầu (không bao gồm) cho vòng lặp qua các biến (phần tử đầu tiên nằm ở chỉ mục bắt đầu + 1)                           | Không    |
| End index for loop (inclusive) | Chỉ mục kết thúc (bao gồm) cho vòng lặp qua các biến                                                                             | Không    |
| Output variable name           | Tên của biến có thể được sử dụng trong vòng lặp để thay thế trong các mẫu. Mặc định là tên biến trống, có lẽ là không mong muốn. | Không    |
| Use Separator                  | Add "\_" before number?                                                                                                          | Có       |

# Random Controller

Định nghĩa: Random Controller làm cho tất cả các user request chạy theo thứ tự ngẫu nhiên trong mỗi vòng lặp.

Ví dụ: bạn có 3 user request đến trang web [https://crm.anhtester.com/admin/authentication](https://crm.anhtester.com/admin/authentication) theo thứ tự sau:

3 HTTP request chạy 5 lần; vậy có tổng số 5 user request sẽ được gửi đến máy chủ&#x20;



| Thuộc tính                   | Mô tả                                                                                                                                                                  | Yêu cầu |
| ---------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------- |
| Name                         | Mô tả tên cho bộ điều khiển này được hiển thị trong trê                                                                                                                | Không   |
| ignore sub-controller blocks | Nếu được chọn, bộ điều khiển xen kẽ sẽ xử lý các bộ điều khiển phụ như các phần tử yêu cầu đơn lẻ và chỉ cho phép một yêu cầu trên mỗi bộ điều khiển tại một thời điểm | Không   |

Thiết lập chạy 5 lần

<figure><img src="../../.gitbook/assets/image (268).png" alt=""><figcaption></figcaption></figure>

Tạo 3 request: HTTP request, FTP request, JDBC request giống nhau khác tên&#x20;

<figure><img src="../../.gitbook/assets/image (269).png" alt=""><figcaption></figcaption></figure>

Report:

<figure><img src="../../.gitbook/assets/image (270).png" alt=""><figcaption></figcaption></figure>

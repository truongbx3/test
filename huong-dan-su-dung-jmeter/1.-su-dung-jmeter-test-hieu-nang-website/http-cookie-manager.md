# Http cookie manager

Định nghĩa: Phần tử Cookie Manager có hai chức năng: Đầu tiên, nó lưu trữ và gửi cookie giống như trình duyệt web. Nếu bạn có Yêu cầu HTTP và phản hồi chứa cookie, Cookie Manager sẽ tự động lưu trữ cookie đó và sẽ sử dụng cookie đó cho tất cả các yêu cầu trong tương lai đến trang web cụ thể đó. Mỗi luồng JMeter có "khu vực lưu trữ cookie" riêng. Vì vậy, nếu bạn đang thử nghiệm một trang web sử dụng cookie để lưu trữ thông tin phiên, mỗi luồng JMeter sẽ có phiên riêng

**standard:** Tuân thủ theo thông số kỹ thuật được xác định bởi [RFC 6265](https://www.ietf.org/rfc/rfc6265.txt) , phần 4. Khuyến nghị!

**standard-strict:** Tuân thủ theo cấu hình hoạt động tốt được xác định bởi RFC 6265, phần 4. Được khuyến nghị!

**ignoreCookies:** Tất cả cookie đều bị bỏ qua. Tương tự như xóa hoặc tắt Cookie Manager.

**netscape**

**default:** Chọn RFC 2965, RFC 2109 hoặc triển khai tuân thủ bản thảo Netscape dựa trên thuộc tính cookie được gửi cùng với phản hồi HTTP

**rfc2109:** Tuân thủ theo thông số kỹ thuật được xác định bởi [RFC 2109](https://www.ietf.org/rfc/rfc2109.txt)&#x20;

**rfc2965:** Tuân thủ theo thông số kỹ thuật được xác định bởi [RFC 2965](https://www.ietf.org/rfc/rfc2965.txt)

**compatibility:** Mô phỏng hành vi của các phiên bản trình duyệt cũ hơn như Mozilla FireFox và Internet Explorer

Ví dụ: [https://blazedemo.com/login](https://blazedemo.com/login)

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

Kết quả

<figure><img src="../../.gitbook/assets/image (277).png" alt=""><figcaption></figcaption></figure>


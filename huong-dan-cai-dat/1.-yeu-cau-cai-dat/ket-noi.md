# Kết nối

Để cài đặt hệ thống, chúng tôi cần mở các kết nối sau:



<table><thead><tr><th width="148">Địa chỉ nguồn</th><th width="217">Địa chỉ đích</th><th width="82">Port</th><th>Mục đích</th></tr></thead><tbody><tr><td>Server</td><td>repo.viettelsoftware.com</td><td>8088</td><td>Kết nối tới image repository. <mark style="color:red;">Bạn chỉ cần mở trong quá trình cài đặt và có thể close khi cài đặt hoàn tất</mark>.</td></tr><tr><td>Server</td><td>auto.viettelsoftware.com</td><td>443</td><td>Thực hiện kết nối từ Runner tới hệ thống TestManager để report kết quả test.</td></tr><tr><td>27.72.144.189</td><td>Server</td><td>8000</td><td>Thực hiện kết nối từ TestManager tới hệ thống Runner để chạy các tiến trình Autotest theo yêu cầu.</td></tr></tbody></table>



_**Server**: là địa chỉ cài đặt Connector của bạn._

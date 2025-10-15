# Once Only Controller

Định nghĩa: Bộ điều khiển logic một lần duy nhất yêu cầu JMeter xử lý bộ điều khiển bên trong nó chỉ một lần cho mỗi luồng và chuyển qua bất kỳ yêu cầu nào bên dưới nó trong các lần lặp lại tiếp theo thông qua kế hoạch thử nghiệm

Once Only Controller bây giờ sẽ luôn thực thi trong lần lặp đầu tiên của bất kỳ bộ điều khiển cha lặp nào. Do đó, nếu Once Only Controller được đặt dưới một Loop Controller được chỉ định để lặp 5 lần, thì Once Only Controller sẽ chỉ thực thi trong lần lặp đầu tiên thông qua Loop Controller (tức là cứ sau 5 lần).

Lưu ý điều này có nghĩa là Once Only Controller vẫn sẽ hoạt động như mong đợi trước đó nếu được đặt trong Nhóm luồng (chỉ chạy một lần cho mỗi lần kiểm tra trên mỗi luồng), nhưng giờ đây người dùng có nhiều sự linh hoạt hơn khi sử dụng Once Only Controller.

Đối với thử nghiệm yêu cầu đăng nhập, hãy cân nhắc đặt yêu cầu đăng nhập trong bộ điều khiển này vì mỗi luồng chỉ cần đăng nhập một lần để thiết lập phiên.



| Thuốc tính | Mô tả                                                 | Yêu cầu |
| ---------- | ----------------------------------------------------- | ------- |
| Name       | Mô tả cho bộ điều khiển này được hiển thị trong tree. | Không   |

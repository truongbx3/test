# Switch Controller

Định nghĩa: Switch Controller nó chạy một trong các phần tử phụ trên mỗi lần lặp, nhưng thay vì chạy chúng theo trình tự, bộ điều khiển chạy phần tử được xác định bởi giá trị chuyển đổi

Nếu giá trị chuyển đổi nằm ngoài phạm vi, nó sẽ chạy phần tử thứ không, do đó đóng vai trò là mặc định cho trường hợp số. Nó cũng chạy phần tử thứ không nếu giá trị là chuỗi rỗng.

Nếu giá trị không phải là số (và không rỗng), thì Bộ điều khiển chuyển đổi sẽ tìm kiếm phần tử có cùng tên (phân biệt chữ hoa chữ thường là quan trọng). Nếu không có tên nào khớp, thì phần tử có tên " default " (phân biệt chữ hoa chữ thường không quan trọng) sẽ được chọn. Nếu không có default, thì không có phần tử nào được chọn và bộ điều khiển sẽ không chạy bất cứ thứ gì.



| Thuộc tính   | Mô tả                                                                                | Yêu cầu |
| ------------ | ------------------------------------------------------------------------------------ | ------- |
| Name         | Mô tả tên cho bộ điều khiển này được hiển thị trong tree                             | Không   |
| Switch Value | Số (hoặc tên) của phần tử phụ được gọi. Các phần tử được đánh số từ 0. Mặc định là 0 | Không   |

# While controller

Định nghĩa: While controller Chạy các phần tử con của nó cho đến khi điều kiện là " sai "&#x20;

Các giá trị điều kiện có thể:

* blank - thoát khỏi vòng lặp khi mẫu cuối cùng trong vòng lặp bị lỗi
* LAST - thoát khỏi vòng lặp khi mẫu cuối cùng trong vòng lặp bị lỗi. Nếu mẫu cuối cùng ngay trước vòng lặp bị lỗi, không vào vòng lặp.
* Nếu không - thoát (hoặc không vào) vòng lặp khi điều kiện bằng chuỗi " false "



| Thuộc tính | Mô tả                                       | Bắt buộc |
| ---------- | ------------------------------------------- | -------- |
| Name       | Tên của Controller được hiển trị trong Tree | Không    |
| Condition  | blank, LAST, or variable/function           | Không    |


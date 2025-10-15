# Transaction controller

Định nghĩa: Bộ điều khiển giao dịch tạo ra một mẫu bổ sung để đo tổng thời gian cần thiết để thực hiện các phần tử thử nghiệm lồng nhau

Có hai chế độ hoạt động:

* mẫu bổ sung được thêm vào sau các mẫu lồng nhau
* mẫu bổ sung được thêm vào như là phần tử cha của các mẫu lồng nhau

| Thuộc tính                                                            | Mô tả                                                                                                                | Yêu cầu |
| --------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | ------- |
| Name                                                                  | Mô tả tên cho bộ điều khiển này được hiển thị trong Tree                                                             | Có      |
| Generate parent sample                                                | Nếu được chọn, mẫu sẽ được tạo ra như là mẫu cha của các mẫu khác, nếu không, mẫu sẽ được tạo ra như một mẫu độc lập | Có      |
| Include duration of timer and pre-post processord in generated sample | Có nên bao gồm bộ đếm thời gian, độ trễ trước và sau khi xử lý trong mẫu được tạo hay không. Mặc định là sai         | Có      |


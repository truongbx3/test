# Http cache manager

Định nghĩa: HTTP Cache Manager được sử dụng để thêm chức năng lưu trữ đệm vào các yêu cầu HTTP trong phạm vi của nó để mô phỏng tính năng lưu trữ đệm của trình duyệt. Mỗi luồng Người dùng ảo có Cache riêng. Theo mặc định, Cache Manager sẽ lưu trữ tối đa 5000 mục trong bộ nhớ đệm cho mỗi luồng Người dùng ảo, sử dụng thuật toán LRU. Sử dụng thuộc tính " maxSize " để sửa đổi giá trị này. Lưu ý rằng bạn càng tăng giá trị này thì HTTP Cache Manager sẽ sử dụng nhiều bộ nhớ hơn, vì vậy hãy đảm bảo điều chỉnh tùy chọn -Xmx JVM cho phù hợp.


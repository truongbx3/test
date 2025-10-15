---
description: 'Tạo file Jmeter: test-case -> New JMeter Test Case'
coverY: 0
---

# 1. Sử dụng JMeter test hiệu năng website

### Giới thiệu các thành phần trong Jmeter <a href="#gioi-thieu-cac-thanh-phan-trong-jmeter" id="gioi-thieu-cac-thanh-phan-trong-jmeter"></a>

Jmeter bao gồm các thành phần sau

* **Test plan**
* **Thread Groups**
* **Sample**
* **Config element**
* **Test Fragment**
* **Logic controller**
* **PreProcessor**
* **PostProcessor**
* **Assertion**
* **Report**

**Tạo kịch bản kiểm thử với Jmeter**

1. Tạo 1 thread group: _TestPlan > New Threads (Users) > Thread group_

<figure><img src="../../.gitbook/assets/image (265).png" alt=""><figcaption></figcaption></figure>

Một Thread Group đại diện cho một nhóm người dùng, và nó chứa tất cả những yếu tố khác.Mỗi Thread Group sẽ mô phỏng những người dùng để thực hiện một trường hợp thử nghiệm cụ thể. Thread Group cho phép tester thực hiện những tùy chỉnh về

<figure><img src="../../.gitbook/assets/image (266).png" alt=""><figcaption></figcaption></figure>

* **Name**: đặt tên cho ThreadGroup
* **Number of Threads(users**) : số lượng người dùng mà ta muốn mô phỏng.&#x20;
* **Ramp-up Period (in seconds)**: Cho biết thời gian để JMeter tạo ra tất cả những thread cần thiết. Ví dụ nếu tham số này là 10 thì trong 10 giây tất cả các Number of Threads đã khai báo ở trên sẽ được gửi đi trong 10 giây, nếu đặt tham số này là 0 thì tất cả các yêu cầu sẽ được gửi đi cùng một lúc.
* **Loop Count Forever** : 1 các thread được tạo sẽ thực hiện 1 lần( thay 1 bằng n thì số các thread sẽ lặp n lần)

VD: Number of Threads: 100, Ram-Up Period: 100, Loop Count: 1. Tức là Jmeter sẽ giả lập thao tác cho 100 user thực hiện trong 600s, tức là mỗi user sẽ tiến hành thực hiện cách nhau 1s (100s/100) và lặp lại 1 lần.

2. Tạo các Request đến server: 1 thread(tương ứng 1 user) có thể tạo nhiều request http gửi lên server . Chuột phải vào Thread group > New Sample > Http Request&#x20;

<figure><img src="../../.gitbook/assets/image (267).png" alt=""><figcaption></figcaption></figure>

Với các phần tử:

* **Name**: Đặt tên Request
* **Request**: bao gồm&#x20;

&#x20;           \* **Method**: Phương thức để các HTTP request. có các method: GET, POST, HEAD, PUSH..

&#x20;           \* Đường dẫn các nguồn để xử lý các request

VD: Nhập [https://crm.anhtester.com/admin/tasks/table](https://crm.anhtester.com/admin/tasks/table)

<figure><img src="../../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

Chuột phải Thread Group -> New Config Element -> CSV data Config

<figure><img src="../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

File CSV gồm

<figure><img src="../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

Bước 3: Nhấn button Save và Run Test case

Report Result Table

<figure><img src="../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

Report bao gồm các thành phần

* **#Samples**: Tổng số lần run của request. Samples = Number of Thread (users)\*Loop Count&#x20;
* **Average (ms)**: Thời gian phản hồi trung bình (Response Time) của request, tính cho đến lần run cuối cùng
* **Min (ms)**: Respone Time thấp nhất của request tính cho toàn bộ tất cả các lần run.
* **Max (ms)**: Respone Time cao nhất của request tính cho toàn bộ tất cả các lần run.
* **Sdt. Dev. (ms)**:độ lệch chuẩn đo lường sự thay đổi của 1 tập hợp data, dựa trên thống kê.
* **Throughput (requests/sec**) : Lượng requests được hệ thống (server) xử lý trong 1 đơn vị thời gian, có thể là giây, phút, hoặc giờ. Avg. Bytes: dung lượng trung bình của 1 lần response tính bằng bytes.
* **% Error**: % số lượng request bị fail, lỗi.
* **Time**: Thời gian chạy của từng request
* **Thread Name**: Tên của Thread Group
* **Label**: Hiển thị tên của từng requests có trong test plan
* **URL**: Đương dẫn url
* **Response Code**: Mã trạng thái
* **Status**: Trạng thái
* **Response Time**: THẤP và Thoughput THẤP --> Trường hợp này sẽ không bao giờ xảy ra. Vì Response Time THẤP nghĩa là thời gian đáp ứng rất nhanh, nhưng Throughput THẤP lại chỉ ra rằng số request được xử lý rất ít. Điều này là vô lý
* Response Time THẤP và Throughput CAO --> Đây là một kết quả lý tưởng . Thời gian xử lý thấp và số lượng request xử lý cùng đồng thời lại cao. Điều này chứng tỏ rằng Server đang rất tốt.
* Response Time CAO và Throughput THẤP --> Test chỉ ra rằng thời gian xử lý quá cao, và lượng request được xử lý lại rất thấp. Phải xem xét để improve về phía sever.
* Response Time CAO and Throughput CAO --> Throughput cao, tức là server đang làm việc rất tốt, vậy tại sao thời gian xử lý lại cũng cao (không tốt). Có thể vấn đề lúc này đế từ phía Client, hoặc cụ thể là đến từ JMeter, có thể đoạn script của bạn viết chưa được tối ưu, khiến quá trình nó xử lý mất nhiều thời gian chẳng hạn
* **Sent Bytes**: Thông lượng KB gửi đi/giây










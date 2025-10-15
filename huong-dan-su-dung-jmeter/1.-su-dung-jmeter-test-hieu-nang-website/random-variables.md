# Random variables

Định nghĩa: Phần tử cấu hình biến ngẫu nhiên được sử dụng để tạo chuỗi số ngẫu nhiên và lưu trữ chúng trong biến để sử dụng sau

| Thuộc tính        | Mô tả                                                                                                                                                                                                                                | Yêu cầu |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------- |
| Name              | Mô tả tên cho phần tử này được hiển thị trong cây                                                                                                                                                                                    | Có      |
| Variable Name     | Tên của biến dùng để lưu trữ chuỗi ngẫu nhiên.                                                                                                                                                                                       | Có      |
| Output Format     | Chuỗi định dạng java.text.DecimalFormat sẽ được sử dụng. Ví dụ " 000 " sẽ tạo ra các số có ít nhất 3 chữ số hoặc " USER\_000 " sẽ tạo ra đầu ra có dạng USER\_nnn . Nếu không được chỉ định, mặc định là tạo số bằng Long.toString() | Không   |
| Minimum Value     | Giá trị nhỏ nhất ( dài ) của số ngẫu nhiên được tạo ra.                                                                                                                                                                              | Có      |
| Maximum Value     | Giá trị lớn nhất ( dài ) của số ngẫu nhiên được tạo ra.                                                                                                                                                                              | Có      |
| Per Thread (User) | Nếu False , trình tạo được chia sẻ giữa tất cả các luồng trong nhóm luồng. Nếu True , thì mỗi luồng có trình tạo ngẫu nhiên riêng.                                                                                                   | Có      |

<figure><img src="../../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

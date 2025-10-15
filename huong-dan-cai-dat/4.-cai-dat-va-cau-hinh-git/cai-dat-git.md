# Cài đặt Git

Mục đích của việc cài đặt Git là để lưu trữ và quản lý các testcase được viết ra bởi tester.

> _Nếu bạn đã có sử dụng Git chỉ cần tạo một project để quản lý các testcase này mà **không cần cài đặt** lại._

Để cài đặt GitLab trên một server của bạn, bạn có thể làm theo các bước sau:

#### Yêu cầu hệ thống

1. **Hệ điều hành**: GitLab hỗ trợ nhiều hệ điều hành như Ubuntu, CentOS, Debian, và Fedora.
2. **Yêu cầu phần cứng**: GitLab có yêu cầu tối thiểu về tài nguyên (RAM, CPU, lưu trữ) mà bạn cần kiểm tra trước khi cài đặt.

### Bước 1: Cài đặt GitLab CE t**rên CentOS 7/8** (Community Edition)

1.  **Cài đặt các gói cần thiết**:

    ```bash
    sudo yum install -y curl policycoreutils-python openssh-server postfix
    sudo systemctl enable sshd postfix
    sudo systemctl start sshd postfix
    ```
2.  **Thêm GitLab repository**:

    ```bash
    curl https://packages.gitlab.com/install/repositories/gitlab/gitlab-ee/script.rpm.sh | sudo bash
    ```

    Đối với GitLab CE, thay `gitlab-ee` bằng `gitlab-ce`.
3.  **Cài đặt GitLab**:

    ```bash
    sudo EXTERNAL_URL="http://your-domain-name.com" yum install -y gitlab-ce
    ```
4.  **Khởi động GitLab**:

    ```bash
    sudo gitlab-ctl reconfigure
    ```
5.  **Truy cập GitLab**:

    Mở trình duyệt và truy cập vào `http://your-domain-name.com`. Hoàn thành việc thiết lập tài khoản admin đầu tiên.

### Bước 2: Cấu hình GitLab (Tùy chọn)

1. **Thiết lập cơ sở dữ liệu**: GitLab có thể sử dụng PostgreSQL hoặc MySQL/MariaDB. Theo mặc định, nó sử dụng PostgreSQL.
2. **Cấu hình SMTP**: Để GitLab gửi email thông báo, bạn cần cấu hình SMTP server.
3. **Cấu hình HTTPS**: Cấu hình HTTPS để bảo mật kết nối với GitLab.

### Lưu ý

* **Firewall**: Mở các port cần thiết (HTTP, HTTPS, SSH) để cho phép truy cập vào GitLab trong trường hợp bạn muốn truy cập từ public.

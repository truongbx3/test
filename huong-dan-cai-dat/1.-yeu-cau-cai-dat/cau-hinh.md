# Cấu hình

Để triển khai hệ thống, chúng tôi đề xuất cấu hình tối thiểu như sau:

### 1. Server (cài đặt môi trường Automation)



| Yêu cầu | Thông số | Ghi Chú |
| ------- | -------- | ------- |
| CPU     | 16 core  |         |
| RAM     | 32 GB    |         |
| HDD     | 300 GB   |         |
| OS      | CENTOS 7 |         |

### 2. Máy tính người dùng (cài đặt ứng dụng IDE)



| Yêu cầu | Thông số                                     | Ghi Chú |
| ------- | -------------------------------------------- | ------- |
| CPU     | <p>Window: 4 cores (x86) <br>Mac: Chip M</p> |         |
| RAM     | 8 GB RAM (64-bit)                            |         |
| HDD     | 2GB Free                                     |         |
| OS      | <p>Windows: 10 + <br>MacOS : 14.4+</p>       |         |

### 3. Các tài nguyên khác

**Git** : Hệ thống quản lý source code, lưu trữ các version kịch bản kiểm thử, chia sẻ, cấp quyền cho tester truy cập vào kịch bản kiểm thử ([hướng dẫn cài đặt](../4.-cai-dat-va-cau-hinh-git/))

**CICD**: Hệ thống build source code và đẩy các kịch bản kiểm thử lên ứng dụng runner. Có thể sử dụng Gitlab Runner hoặc Jenkin

**Jira**: Hệ thống quản lý task. Hệ thống Automation sẽ đồng bộ thông tin dự án, member dự án, log bug


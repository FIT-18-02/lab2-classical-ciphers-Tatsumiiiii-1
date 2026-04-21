# Report 1 Page – FIT4012 Lab 2

## 1. Mục tiêu
Tóm tắt ngắn gọn mục tiêu của bài lab.

## 2. Cách làm
- Hoàn thiện Caesar Cipher cho chữ thường, dấu cách và giải mã.
- Hoàn thiện Rail Fence Cipher cho giải mã, giữ dấu cách, kiểm tra đầu vào và đọc file.
- Chạy thử trên nhiều test case.

## 3. Kết quả chính
### 3.1 Caesar Cipher
| Input | Key | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 3 | L ORYH BRX | Đúng, mã hóa chuẩn với key = 3 |
| hello world | 5 | mjqqt btwqi | Đúng, mã hóa chuẩn với key = 5 |
| LORYH BRX | 3 | I LOVE YOU | Đúng, giải mã chính xác |

### 3.2 Rail Fence Cipher
| Input | Rails | Ciphertext / Plaintext | Nhận xét |
|---|---:|---|---|
| I LOVE YOU | 2 | ILV O OEYU | Đúng, zigzag 2 dòng |
| I LOVE YOU | 4 | IY LOEOVU | Đúng, phân bổ theo 4 rails |
| IOEOLVYU | 2 | I LOVE YOU | Đúng, giải mã chính xác |

### 3.3 Input validation / file input
- Trường hợp đầu vào không hợp lệ:
 - Ký tự đặc biệt → bị từ chối
  - Số → bị từ chối
- Kết quả đọc từ `data/input.txt`:
Message from file: I LOVE YOU
Enter rails: 2
Ciphertext: ILV O OEYU

## 4. Kết luận

Từ bài lab, em đã hiểu sâu hơn về nguyên lý vận hành của các thuật toán mã hóa cổ điển, nhất là sự khác nhau giữa mã hóa thay thế (Caesar) và mã hóa hoán vị (Rail Fence). Điểm khó nhất nằm ở khâu giải mã Rail Fence, vì cần xác định chính xác vị trí từng ký tự trên mô hình zigzag. Nhờ thử nghiệm với nhiều bộ dữ liệu và rà soát từng bước, em đã thành thạo cách cài đặt, đồng thời nâng cao kỹ năng lập trình cũng như tư duy giải thuật.

# Test Cases Log - SkyTicket

## Mục tiêu

Kiểm tra hệ thống có chặn được các trường hợp dữ liệu không hợp lệ hay không.

| STT | Mật khẩu | Hộ chiếu | Tuổi | Hạng vé  | Số dư | Kết quả mong đợi              |
| --- | -------- | -------- | ---: | -------- | ----: | ----------------------------- |
| 1   | Sai      | 12345    |   25 | Class    |  2000 | Chặn - Mật khẩu không đúng    |
| 2   | 12345    | abc      |   25 | Class    |  2000 | Chặn - ID hộ chiếu không khớp |
| 3   | 12345    | 12345    |   17 | Class    |  2000 | Chặn - Chưa đủ tuổi           |
| 4   | 12345    | 12345    |   25 | Class    |   500 | Chặn - Số dư không đủ         |
| 5   | 12345    | 12345    |   25 | Class    |  1000 | Thành công                    |
| 6   | 12345    | 12345    |   25 | Business |  1500 | Chặn - Không đủ tiền          |
| 7   | 12345    | 12345    |   25 | Business |  2000 | Thành công                    |
| 8   | 12345    | 12345    |   25 | Vip      |  3000 | Thành công                    |

## Kết quả chạy thử

- Case 1: PASS
- Case 2: PASS
- Case 3: PASS
- Case 4: PASS
- Case 5: PASS
- Case 6: PASS
- Case 7: PASS
- Case 8: PASS

# Water Level Control Using AT89S52

## Giới thiệu

Nước là một nguồn tài nguyên quan trọng, đóng vai trò thiết yếu trong cuộc sống hàng ngày và nhiều lĩnh vực sản xuất. Tuy nhiên, việc quản lý và sử dụng nước, đặc biệt ở vùng nông thôn, vẫn còn nhiều hạn chế. Hệ thống truyền thống sử dụng bồn nước đặt trên cao để cung cấp nước bằng trọng lực có nhiều bất tiện như:

- Không thể kiểm tra mực nước hiện tại.
- Việc bơm nước phải thực hiện thủ công, gây lãng phí thời gian và công sức.

Dự án **"Water Level Control Using AT89S52"** được thiết kế nhằm giải quyết các vấn đề trên bằng cách cung cấp một giải pháp tự động kiểm soát mức nước thông qua vi điều khiển **AT89S52**. Hệ thống bao gồm hai chức năng chính:

1. **Kiểm tra mực nước trong bể chứa.**  
2. **Tự động điều khiển bơm nước dựa trên mức nước hiện tại.**

---

## Mục tiêu

- Xây dựng một hệ thống kiểm soát mức nước hiệu quả, linh hoạt và tự động.
- Cung cấp giao diện thân thiện với người dùng qua màn hình **LCD** và bàn phím.
- Giúp tiết kiệm nước, tối ưu hóa việc sử dụng tài nguyên.

---

## Thiết kế hệ thống

### Ý tưởng

- Sử dụng các **cảm biến mực nước** để đo mức nước trong bể chứa.
- Vi điều khiển **AT89S52** xử lý tín hiệu từ cảm biến và điều khiển bơm nước.
- Hiển thị thông tin mức nước và trạng thái bơm trên **màn hình LCD 16x2**.
- Người dùng có thể điều chỉnh chế độ hoạt động thông qua **bàn phím 4x4**.

### Cấu trúc hệ thống

Hệ thống bao gồm các khối chức năng chính:

1. **Khối cảm biến mực nước**: Xác định mức nước trong bể và gửi tín hiệu đến vi điều khiển.  
2. **Khối xử lý tín hiệu**: Vi điều khiển **AT89S52** tiếp nhận và xử lý tín hiệu từ cảm biến, hiển thị thông tin và điều khiển bơm.  
3. **Khối điều khiển bơm nước**: **Relay** và **transistor** kiểm soát việc bật/tắt máy bơm theo tín hiệu từ vi điều khiển.  
4. **Khối giao diện người dùng**: **LCD 16x2** hiển thị thông tin và **bàn phím 4x4** giúp người dùng điều khiển hệ thống.  

---

## Linh kiện sử dụng

| Linh kiện          | Mô tả                        |
|--------------------|----------------------------|
| **Vi điều khiển**  | AT89S52                     |
| **Màn hình LCD**   | 16x2                         |
| **Bàn phím**       | Keypad 4x4                   |
| **Relay**         | 5V                           |
| **Transistor**     | 2N2222A                      |
| **Cảm biến mực nước** | Dây dẫn điện với các mức nước **High, Medium, Low** |
| **Nguồn điện**     | 5V và 12V DC                 |

---

## RENDER 3D
![PCB 3D](Render3d/Render3d.png)


## Nguyên lý hoạt động

- Khi **mực nước thấp (Low)**, hệ thống sẽ **tự động bật bơm nước**.
- Khi **mực nước đạt mức cao (High)**, hệ thống sẽ **tắt bơm nước**.
- Người dùng có thể giám sát và điều khiển hệ thống thông qua **màn hình LCD** và **bàn phím**.

---

## Hướng dẫn sử dụng

1. Kết nối hệ thống theo sơ đồ mạch điện.
2. Cấp nguồn **5V** cho vi điều khiển và **12V** cho bơm nước.
3. Theo dõi mức nước trên **màn hình LCD**.
4. Nhấn các phím trên **keypad** để điều chỉnh chế độ hoạt động nếu cần.

---

## Ứng dụng thực tế

- Quản lý nước trong **hộ gia đình, nông nghiệp, và hệ thống cấp nước đô thị**.
- Giúp **tiết kiệm nước** và **tối ưu hóa việc sử dụng tài nguyên**.

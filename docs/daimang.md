- Trước khi đến với các dải mạng thì chúng ta nên tìm hiểu đến Switch ảo (Virtual Switch), card mạng máy ảo, DHCP và LAN Segment.
### 1. Switch ảo (Virtual Switch)
- Tương tự như một [Switch vật lý](https://vi.wikipedia.org/wiki/Switch_(m%E1%BA%A1ng)) thì Switch ảo kết nối các thành phần mạng ảo với nhau.
- Những  switch ảo hay còn gọi là mạng ảo, chúng có tên là VMnet0, VMnet1, VMnet2… một số switch ảo được gắn vào mạng một cách mặc định.
- Khi ta tạo các VMnet, thì trên máy thật sẽ tạo ra những card mạng ảo tương ứng với VMnet đó, dùng để kết nối Virtual Switch với máy tính thật, giúp máy thật và máy ảo có thể liên lạc được với nhau.
### 2. Card mạng máy ảo
- Khi bạn tạo một máy ảo mới, card mạng được tạo ra cho máy ảo, những card mạng này hiển thị trên hệ điều hành máy ảo với tên thiết bị như là AMD PCNET PCI hay Intel Pro/1000 MT Server Adapter.
>Lưu ý: Khi copy một máy ảo thì nên thay đổi địa chỉ MAC của nó, vì địa chỉ MAC là địa chỉ duy nhất, vậy nên chúng ta nên thay đổi địa chỉ MAC để tránh gặp lỗi khi làm việc với thệ thống.
```
Địa chỉ MAC: là địa chỉ định danh duy nhất hay còn gọi là số nhận dạng của mỗi thiết bị được các nhà sản xuất gán trên mỗi thiết bị.
```
### 3. DHCP server ảo của VMnet
- DHCP (Dynamic Host Configuration) server ảo đảm nhiệm việc cung cấp địa chỉ IP cho các máy ảo trong việc kết nối máy ảo vào các Switch ảo không có tính năng Bridged (VMnet0) là NAT và host only.
### 4. LAN Segment.
- Các card mạng của máy ảo có thể gắn kết với nhau thành từng LAN Segment. Không giống như VMnet, LAN Segment chỉ kết nối các máy ảo được gán trong một LAN Segment lại với nhau mà không có những tính năng như DHCP và LAN Segment không thể kết nối ra máy thật như các Virtual Switch VMnet.
## Dải mạng trong máy ảo
- Mỗi máy ảo sẽ có 3 loại dải mạng để lựa chọn kết nối:
  - Dải mạng Brided.
  - Dải mạng NAT.
  - Dải mạng host only.

## Dải mạng trong máy ảo
- Mỗi máy ảo sẽ có 3 loại dải mạng để lựa chọn kết nối:
  - Dải mạng Brided.
  - Dải mạng NAT.
  - Dải mạng host only.
- Nhưng trước khi tìm hiểu đến các dải mạng thì chúng ta nên tìm hiểu đến Switch ảo (Virtual Switch):
### 1. Switch ảo (Virtual Switch)
- Tương tự như một [Switch vật lý](https://vi.wikipedia.org/wiki/Switch_(m%E1%BA%A1ng)) thì Switch ảo kết nối các thành phần mạng ảo với nhau.
- Những  switch ảo hay còn gọi là mạng ảo, chúng có tên là VMnet0, VMnet1, VMnet2… một số switch ảo được gắn vào mạng một cách mặc định.
- Khi ta tạo các VMnet, thì trên máy thật sẽ tạo ra những card mạng ảo tương ứng với VMnet đó, dùng để kết nối Virtual Switch với máy tính thật, giúp máy thật và máy ảo có thể liên lạc được với nhau.

## Ảo hóa là gì?
- Là một cách gọi khi tạo các máy ảo trên một máy tính lớn.
## Lợi ích
- Chắc chắn chúng ta sẽ không làm nếu nó vô ích, vậy nó mang lợi ích gì? Đại loại chúng ta sẽ hình dung một nhà với nhiều thế hệ gia đình cùng chung sống nhưng bên trong căn nhà đấy lại chỉ có một phòng, điều này dẫn đến việc khiến cho xung đột giữa mọi người ở các thế hệ với nhau trong sinh hoạt hàng ngày hay sở thích, sở ghét riêng. Để giải quyết việc này thì ta cần làm là mua thêm vài căn nhà cho vừa đủ với mọi người trong các thế hệ của gia đình đây là giải pháp bạn không có gì ngoài điều kiện, hoặc với nguồn tài sản có hạn thì việc xây thêm phòng riêng cho mọi người trong các thế hệ là giải pháp hợp lý (tất nhiên nhà bạn phải có đủ không gian để cho mỗi phòng có diện tích thoải mái) lúc này thì mọi người lại vui vẻ với nhau ít xảy ra xung đột hơn vì ai cũng đã có không gian riêng của mình. Về với ảo hóa, nếu như bạn dùng nhiều chức năng trên một máy tính thì đôi khi các tính năng lại xung đột với nhau gây ra các lỗi và chính bạn sẽ là người phải sửa lỗi thì ảo hóa có thể giúp chúng ta tạo ra những căn phòng riêng (gọi là máy ảo - Virtual Machine) cho mỗi chức năng để tránh các xung đột, điều này sẽ tiết kiệm tối đa chi phí chứ không cần phải mua các căn nhà mới (máy tính) cho mỗi chức năng.
## Hypervisor là gì?
- Hypervisor hay còn có tên khác là Virtual machine monitor (VMM) là từ dùng để chỉ các phần mềm, firmware hoặc thậm chí là một phần cứng chuyên dụng dùng để tạo ra các máy ảo (virtual machine). Nói vui vẻ thì đại loại muốn ảo hóa máy tính thì cài hypervisor vào.
### Hypervisor hoạt động như thế nào?
- Vậy **NÓ** hoạt động như thế nào? Đại loại **NÓ** sẽ biến máy tính của mình trở thành một host để có thể ảo hóa máy tính.
- Giờ thì làm sao để cài đặt **NÓ**? Bạn có thể cài đặt **NÓ** như các phần mềm thông thường hoặc cài **NÓ** như một OS (hệ điều hành).
- Chúng ta sẽ phân nó ra làm 2 loại:
  - Hypervisor Type 1 ( native hay Bare-metal ).
  - Hypervisor Type 2.
#### 1. Hypervisor Type 1 - Native - Bare metal - Hypervisor based:
- Đây là loại hypervisor chạy trực tiếp trên phần cứng của máy chủ, không thông qua một OS (hệ điều hành) nào cả, vì vậy còn có tên gọi là Bare-metal.
- Vị trí hoạt động của nó dựa vào mô hình sau:
<img src = "https://github.com/toan207/VMware-note/blob/master/images/1%20-%20Hypervisor%20Type%201%20-%201.png"> 

- Đúng với tên gọi bare-metal của nó những hypervisor này được cài đặt trực tiếp lên máy chủ mà không thông qua bất kỳ 1 OS nào và thường sẽ được đính kèm theo một phần mềm quản trị để người dùng có thể tiện thao tác  
>Ví dụ như với VMware ESX thì có phần mềm kèm theo là VMware vSphere Client.

<img src = "https://github.com/toan207/VMware-note/blob/master/images/1%20-%20Hypervisor%20Type%201%20-%202.png">

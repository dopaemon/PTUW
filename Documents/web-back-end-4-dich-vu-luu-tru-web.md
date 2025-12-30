# Web back-end - Ứng dụng web bán hàng

## Ứng dụng web bán hàng
Trong các nguồn tài liệu, **ứng dụng web bán hàng** được sử dụng làm dự án thực tế để tìm hiểu về quy trình phát triển web chuyên sâu (Project-Based Learning), cụ thể là dự án **phát triển ứng dụng web bán quần áo** với tên gọi gợi ý là **TeoShop**,.

Dưới đây là các thông tin chi tiết về việc phát triển một ứng dụng web bán hàng:

#### 1. Các cách để tạo ra ứng dụng web bán hàng
Có ba phương pháp chính để xây dựng một ứng dụng bán hàng, tùy thuộc vào nhu cầu và nguồn lực:

*   **Sử dụng hệ quản trị nội dung (CMS):** Đây là cách nhanh nhất, không cần kiến thức lập trình chuyên sâu. Các CMS phổ biến chuyên cho thương mại điện tử/bán hàng bao gồm: **WordPress, Shopify, Wix, Magento, Joomla và Drupal**.
*   **Sử dụng Framework và thư viện hỗ trợ:** Phương pháp này được các lập trình viên và công ty chuyên nghiệp ưu tiên vì tăng tốc độ phát triển và đảm bảo bảo mật. Ví dụ: Sử dụng **React, Angular** cho giao diện (Frontend) và **Express.js, Laravel, hoặc Django** cho hệ thống xử lý (Backend).
*   **Viết thuần (Code tay):** Tự viết toàn bộ mã nguồn từ đầu để có toàn quyền kiểm soát và tối ưu hóa hệ thống, nhưng đòi hỏi kiến thức chuyên môn rất cao và tốn nhiều công sức.

#### 2. Quy trình phát triển (Vòng đời dự án)
Một dự án ứng dụng web bán hàng cần trải qua **6 giai đoạn cơ bản**:
1.  **Lấy và phân tích yêu cầu:** Xác định các tính năng cần có (ví dụ: giỏ hàng, thanh toán, quản lý kho).
2.  **Thiết kế:** Xây dựng giao diện người dùng và cấu trúc dữ liệu.
3.  **Lập trình:** Hiện thực hóa các thiết kế thành mã nguồn (đây là giai đoạn tốn nhiều thời gian nhất).
4.  **Kiểm thử:** Đảm bảo ứng dụng chạy đúng và không có lỗi đặt hàng hay thanh toán.
5.  **Triển khai:** Đưa ứng dụng lên internet thông qua các Web server như **Nginx, Apache hoặc Node.js**.
6.  **Vận hành và Bảo trì:** Theo dõi hoạt động và cập nhật tính năng mới.

#### 3. Công nghệ sử dụng (Ví dụ dự án TeoShop)
Để phát triển một ứng dụng bán hàng hiện đại như TeoShop, các công nghệ sau thường được kết hợp:
*   **Phía Client (Trình duyệt người dùng):** Sử dụng **HTML** để tạo khung giao diện, **CSS** để trang trí và **JavaScript** để xử lý hiệu ứng, trao đổi dữ liệu.
*   **Phía Server (Máy chủ xử lý):** Sử dụng ngôn ngữ **JavaScript** với framework **Express**.
*   **Cơ sở dữ liệu:** Sử dụng **PostgreSQL** để lưu trữ thông tin sản phẩm, khách hàng và đơn hàng.
*   **Quản lý mã nguồn:** Sử dụng **Git và GitHub** để theo dõi lịch sử thay đổi và cộng tác nhóm.
*   **Công cụ lập trình:** Phổ biến nhất là **VS Code** để viết mã và tổ chức thư mục dự án.

***

Để dễ hiểu, việc tạo một ứng dụng web bán hàng giống như **mở một cửa hàng trong thực tế**: 
*   **Sử dụng CMS** giống như bạn thuê một gian hàng có sẵn trong trung tâm thương mại; mọi thứ đã có khung sẵn, bạn chỉ cần bày biện hàng hóa vào là bán được ngay. 
*   **Sử dụng Framework** giống như việc bạn thuê một đơn vị thi công chuyên nghiệp xây cửa hàng theo bản thiết kế riêng; nó độc đáo hơn nhưng vẫn dựa trên các tiêu chuẩn xây dựng an toàn. 
*   **Viết thuần** giống như việc bạn tự mình đúc từng viên gạch và tự tay xây nên cửa hàng từ bãi đất trống; cực kỳ vất vả nhưng bạn sẽ có một ngôi nhà hoàn toàn theo ý muốn và hiểu rõ từng ngóc ngách của nó.

### Thông tin về dự án
Dựa trên các nguồn tài liệu, dưới đây là thông tin chi tiết về dự án phát triển ứng dụng web được đề cập:

#### 1. Tổng quan dự án
*   **Tên dự án:** Phát triển ứng dụng web bán quần áo.
*   **Tên thương mại gợi ý:** **TeoShop** (tên ngắn gọn phù hợp cho kinh doanh thực tế).
*   **Phương pháp tiếp cận:** Học tập dựa trên dự án (**Project-Based Learning - PBL**). Dự án này tập trung chủ yếu vào giai đoạn **Lập trình** trong vòng đời gồm 6 bước của một phần mềm.

#### 2. Môi trường và Công cụ phát triển
Để thực hiện dự án này, các công nghệ và công cụ sau được sử dụng,:

*   **Lập trình phía Client (Client-side):**
    *   **HTML:** Tạo cấu trúc giao diện.
    *   **CSS:** Định dạng hiển thị và trang trí.
    *   **JavaScript:** Xử lý hiệu ứng và trao đổi dữ liệu với server.
*   **Lập trình phía Server (Server-side):**
    *   **Ngôn ngữ:** JavaScript.
    *   **Framework:** Express.
    *   **Web server:** Nodejs.
*   **Cơ sở dữ liệu:**
    *   **Hệ quản trị:** PostgreSQL.
    *   **Công cụ quản lý:** pgAdmin.
*   **Quản lý mã nguồn:** Git và GitHub để theo dõi lịch sử thay đổi và cộng tác,.
*   **Công cụ viết mã:** **VS Code** (được chọn để tạo, tổ chức thư mục và viết mã nguồn).

#### 3. Quy trình thực hiện ban đầu
Dự án bắt đầu với các bước thiết lập nền tảng cơ bản:
*   **Tạo cấu trúc:** Tạo thư mục dự án (ví dụ: `E:\TeoShop`).
*   **Nhúng Git:** Sử dụng lệnh `git init` trong cửa sổ dòng lệnh để khởi tạo kho chứa (repository). 
*   **Kho lưu trữ:** Sau khi nhúng thành công, một thư mục ẩn tên là `.git` sẽ xuất hiện, đây là nơi lưu trữ toàn bộ lịch sử thay đổi của dự án.

#### 4. Vòng đời dự án
Dự án tuân theo quy trình chuẩn của một phần mềm, bao gồm các giai đoạn:
1. Lấy và phân tích yêu cầu.
2. Thiết kế.
3. **Lập trình** (trọng tâm của tài liệu này).
4. Kiểm thử.
5. Triển khai.
6. Vận hành và Bảo trì.

***

Để dễ hình dung, **dự án TeoShop giống như việc bạn xây dựng một cửa hàng thời trang**: 
*   **Phần Client (HTML/CSS)** là mặt tiền, kệ sách và cách bài trí cửa hàng để khách hàng nhìn thấy. 
*   **Phần Server (Nodejs/Express)** giống như đội ngũ nhân viên và quản lý đứng sau hậu trường để xử lý đơn hàng. 
*   **Cơ sở dữ liệu (PostgreSQL)** là kho hàng lưu trữ thông tin sản phẩm. 
*   **Git** giống như một cuốn nhật ký ghi chép lại mọi thay đổi của cửa hàng từ lúc mới xây móng, giúp bạn có thể kiểm tra lại hoặc sửa sai bất cứ lúc nào.

### Tải và cài đặt VS Code
Để tải và cài đặt **VS Code** (Visual Studio Code) phục vụ cho việc phát triển ứng dụng web, bạn thực hiện theo các hướng dẫn sau:

#### 1. VS Code là gì?
VS Code là một **Code Editor** (trình soạn thảo mã nguồn), được sử dụng làm công cụ chính để **tạo, tổ chức thư mục, tập tin và viết mã nguồn** cho các dự án web,. So với các công cụ khác như Notepad (Text editor) hay Eclipse (IDE), VS Code là lựa chọn phổ biến cho các dự án phát triển web hiện nay,.

#### 2. Các bước tải và cài đặt
*   **Bước 1 - Tải phần mềm:** Bạn truy cập vào trang chủ chính thức tại địa chỉ: **[https://code.visualstudio.com/](https://code.visualstudio.com/)** để tải bộ cài đặt về máy tính.
*   **Bước 2 - Cài đặt:** Sau khi tải về, bạn mở tập tin và thực hiện cài đặt **như một chương trình thông thường** trên hệ điều hành của mình.

#### 3. Vai trò của VS Code trong dự án
Trong quá trình phát triển ứng dụng (ví dụ như dự án bán hàng TeoShop), VS Code được sử dụng để:
*   **Viết mã nguồn:** Soạn thảo các tập tin HTML, CSS, JavaScript cho phía Client và mã nguồn phía Server,.
*   **Chỉnh sửa cấu hình:** Bạn có thể dùng VS Code để mở và chỉnh sửa các tệp cấu hình hệ thống như `nginx.conf` của máy chủ Nginx,.
*   **Quản lý dự án:** Giúp tổ chức cây thư mục dự án một cách khoa học và rõ ràng.

Việc sử dụng thành thạo một Code Editor như VS Code sẽ giúp bạn tăng tốc độ phát triển và cải thiện chất lượng mã nguồn đáng kể khi thực hiện dự án,.

***

Để dễ hình dung, nếu việc lập trình là viết một cuốn sách, thì **VS Code chính là một chiếc máy đánh chữ hiện đại**: nó không chỉ cung cấp giấy và mực (nơi viết mã) mà còn hỗ trợ bạn sắp xếp các chương hồi (thư mục), kiểm tra lỗi chính tả và định dạng trang sách sao cho đẹp mắt và chuyên nghiệp nhất.

### Tải và cài đặt Git
Để tải và cài đặt **Git** phục vụ cho việc quản lý mã nguồn trong dự án phát triển ứng dụng web, bạn có thể thực hiện theo các bước chi tiết sau đây:

#### 1. Tải và cài đặt Git
Vì Git là một phần mềm, bạn cần tải bộ cài đặt về máy tính và thực hiện cài đặt như một phần mềm thông thường,:
*   **Bước 1:** Truy cập vào trang chủ chính thức: **[https://git-scm.com/](https://git-scm.com/)**,.
*   **Bước 2:** Chọn phiên bản phù hợp với hệ điều hành bạn đang sử dụng (Windows, macOS, Linux) để tải về,.
*   **Bước 3:** Sau khi tải xong, mở tập tin và tiến hành cài đặt theo các hướng dẫn trên màn hình,.

#### 2. Kiểm tra cài đặt thành công
Sau khi cài đặt, bạn cần xác nhận xem Git đã sẵn sàng hoạt động trên máy tính hay chưa bằng cách:
1.  Nhấn tổ hợp phím **Cửa sổ + R**, gõ `cmd` và nhấn Enter để mở cửa sổ dòng lệnh (Command Line),.
2.  Nhập lệnh: `git --version` hoặc `git -v`,.
3.  **Kết quả:** Nếu màn hình hiển thị thông tin về phiên bản của Git (ví dụ: *git version 2.x.x*), nghĩa là bạn đã cài đặt thành công và có thể bắt đầu sử dụng,.

#### 3. Khởi tạo Git trong dự án (Nhúng Git)
Để Git bắt đầu quản lý các phiên bản của một thư mục dự án cụ thể (ví dụ thư mục `TeoShop`), bạn thực hiện:
*   Sử dụng lệnh `cd` trong cửa sổ dòng lệnh để di chuyển vào thư mục dự án đó,.
*   Gõ lệnh: **`git init`**,.
*   **Dấu hiệu thành công:** Bạn sẽ nhận được thông báo *"Initialized empty Git repository..."* và trong thư mục dự án sẽ xuất hiện một thư mục ẩn tên là **`.git`**,. Đây là "kho chứa" lưu trữ toàn bộ lịch sử thay đổi của dự án, bạn không nên thay đổi nội dung trong thư mục này,.

#### 4. Tại sao cần sử dụng Git?
Git cung cấp các tính năng quan trọng giúp việc lập trình chuyên nghiệp hơn:
*   **Theo dõi lịch sử:** Lưu lại từng thay đổi nhỏ nhất, cho phép quay lại các phiên bản cũ khi cần,.
*   **Cộng tác:** Nhiều người có thể cùng làm việc trên một dự án và hợp nhất các thay đổi dễ dàng,.
*   **Phân nhánh (Branch):** Thử nghiệm tính năng mới ở một nhánh riêng mà không ảnh hưởng đến mã nguồn chính,.
*   **Hoạt động phân tán:** Bạn có thể làm việc ngay cả khi không có kết nối mạng và đồng bộ hóa lại sau đó,.

Mặc dù có thể sử dụng Git qua giao diện đồ họa (GUI) hoặc tích hợp trong VS Code, nhưng tài liệu khuyến khích bạn **sử dụng giao diện dòng lệnh** để hiểu rõ bản chất các lệnh và đạt hiệu quả học tập tốt nhất,.

***

Để dễ hình dung, **Git giống như một "Cỗ máy thời gian" và "Nhật ký công việc" cho mã nguồn của bạn**: 
Nó không chỉ ghi lại chi tiết ai đã sửa gì, vào lúc nào (nhật ký) mà còn cho phép bạn "nhảy" về bất kỳ thời điểm nào trong quá khứ nếu chẳng may lỡ tay làm hỏng ứng dụng (cỗ máy thời gian), giúp dự án luôn được bảo vệ an toàn.

### Tạo thư mục dự án và nhúng Git:
Việc **tạo thư mục dự án và nhúng Git** là bước khởi đầu quan trọng trong giai đoạn lập trình để quản lý mã nguồn một cách chuyên nghiệp,. Dưới đây là các bước thực hiện chi tiết theo hướng dẫn:

#### 1. Tạo thư mục dự án
Bạn sử dụng **File Explorer** để tạo một thư mục dành riêng cho dự án của mình. 
*   **Ví dụ:** Trong ổ đĩa **E:\**, bạn tạo một thư mục có tên là **TeoShop**. Lúc này, đây vẫn là một thư mục rỗng thông thường.

#### 2. Nhúng Git vào thư mục dự án
Để Git có thể theo dõi và quản lý các phiên bản của dự án, bạn cần thực hiện "nhúng" (khởi tạo) Git vào thư mục vừa tạo. Cách hiệu quả nhất là sử dụng **giao diện dòng lệnh (command line)** theo các bước sau,:

*   **Bước 1:** Mở cửa sổ dòng lệnh (CMD hoặc PowerShell),.
*   **Bước 2:** Di chuyển vào thư mục dự án bằng lệnh `cd`. 
    *   *Lưu ý:* Nếu thư mục nằm ở ổ đĩa khác, bạn cần gõ tên ổ đĩa kèm dấu hai chấm (ví dụ `E:`) rồi nhấn Enter, sau đó mới dùng lệnh `cd TeoShop`.
*   **Bước 3:** Gõ lệnh **`git init`** và nhấn Enter. Chữ "init" là viết tắt của *initialize*, có nghĩa là khởi tạo.

#### 3. Kiểm tra kết quả
Nếu thực hiện thành công, hệ thống sẽ hiển thị thông báo: **"Initialized empty Git repository in E:/TeoShop/.git/"**.

*   **Sự thay đổi trong thư mục:** Khi mở thư mục dự án, bạn sẽ thấy xuất hiện thêm một **thư mục ẩn tên là .git**. 
*   **Vai trò của thư mục .git:** Đây chính là **kho chứa (repository)** lưu trữ toàn bộ lịch sử thay đổi của dự án. 
*   **Lưu ý quan trọng:** Bạn **không nên thay đổi nội dung** bên trong thư mục `.git` này vì nó phục vụ cho các tác vụ quản lý của phần mềm Git.
*   **Mẹo nhỏ:** Nếu không thấy thư mục `.git`, bạn hãy vào menu **View** trong File Explorer và đánh dấu chọn vào mục **Hidden items** để hiển thị các mục ẩn.

Việc nhúng Git thành công sẽ giúp bạn bắt đầu quá trình theo dõi lịch sử, cộng tác và bảo mật mã nguồn cho ứng dụng web của mình,.

***

Để dễ hình dung, việc tạo thư mục và nhúng Git giống như việc bạn **lập một cuốn sổ nhật ký công trình cho một ngôi nhà mới xây**: 
*   **Thư mục dự án** là mảnh đất bạn dùng để xây nhà. 
*   **Lệnh `git init`** giống như việc bạn đặt cuốn sổ nhật ký vào một ngăn tủ kính bảo mật tại công trình. Từ giây phút đó, mọi viên gạch được đặt xuống hay bất kỳ thay đổi nào trong thiết kế đều sẽ được cuốn sổ này ghi chép lại tỉ mỉ, giúp bạn có thể kiểm tra lại lịch sử xây dựng bất cứ lúc nào.

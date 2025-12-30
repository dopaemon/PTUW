# Web back-end - Nodejs và NPM

## Nodejs và NPM
### Nodejs
**Nodejs** là một **môi trường thực thi (runtime environment)** mã nguồn JavaScript đa nền tảng, mã nguồn mở và hoàn toàn miễn phí,. Đây là một thành phần quan trọng trong hạ tầng ứng dụng web, cho phép lập trình viên tạo ra các máy chủ (web server), ứng dụng web và các công cụ dòng lệnh,.

#### 1. Bản chất của Nodejs
Nhiều người thường nhầm lẫn về khái niệm này, nhưng cần lưu ý rằng:
*   Nodejs **không phải là một ngôn ngữ lập trình** và cũng **không phải là một framework**.
*   Nó là một **nền tảng (platform)** hoặc một môi trường cung cấp các thành phần cần thiết để thực thi mã nguồn JavaScript.
*   Lập trình viên sẽ viết mã bằng JavaScript thuần hoặc dùng framework (như Express), sau đó Nodejs sẽ chịu trách nhiệm **dịch mã và thực thi** chương trình để xuất kết quả.

#### 2. Các thành phần cốt lõi
Nodejs là một phần mềm phức hợp bao gồm nhiều thành phần bên trong, tiêu biểu là:
*   **V8 Engine:** Bộ phận chịu trách nhiệm dịch và thực thi mã JavaScript.
*   **HTTP Module:** Thành phần giúp tạo ra các máy chủ web (web server).
*   **NPM (Node Package Manager):** Chương trình quản lý các gói và thư viện dùng cho ứng dụng,.
*   **Các module và thư viện khác:** Hỗ trợ lập trình ứng dụng web chuyên sâu.

#### 3. NPM – Người bạn đồng hành cùng Nodejs
NPM là công cụ quản lý thư viện đi kèm mặc định khi bạn cài đặt Nodejs,.
*   Vì các ứng dụng web hiện nay thường sử dụng rất nhiều thư viện (gọi là các **package**), NPM giúp quản lý các thành phần phụ thuộc này một cách tự động thay vì phải làm thủ công,.
*   NPM gồm 3 thành phần chính: **Website** (để tìm kiếm thư viện), **CLI** (công cụ dòng lệnh để cài đặt) và **Registry** (kho lưu trữ các thư viện).

#### 4. Cài đặt và Kiểm tra
Để sử dụng Nodejs trong các dự án (như dự án bán hàng TeoShop), bạn thực hiện các bước sau,:
*   **Tải về:** Truy cập trang chủ [nodejs.org](https://nodejs.org/en) để tải bộ cài đặt phù hợp,.
*   **Cài đặt:** Thực hiện cài đặt như một phần mềm thông thường trên máy tính.
*   **Kiểm tra:** 
    *   Mở cửa sổ dòng lệnh (CMD hoặc Powershell) và gõ lệnh **`node -v`** để kiểm tra phiên bản Nodejs,.
    *   Gõ lệnh **`npm -v`** để kiểm tra phiên bản của công cụ quản lý thư viện.

Trong mô hình phát triển ứng dụng web hiện đại, Nodejs đóng vai trò là **Web Server** ở phía backend, giúp xử lý các yêu cầu từ người dùng và tương tác với cơ sở dữ liệu,.

***

Để dễ hình dung, bạn có thể coi **Nodejs giống như một căn bếp chuyên dụng**:
Trong đó, **JavaScript** chính là các công thức nấu ăn mà bạn viết ra. Bản thân công thức không thể tự biến thành món ăn nếu thiếu bếp. **Nodejs (Căn bếp)** cung cấp các dụng cụ như **V8 Engine (Bếp nấu)** để thực hiện việc nấu nướng và **NPM (Tủ chứa nguyên liệu)** để cung cấp sẵn các loại gia vị, thực phẩm cần thiết, giúp bạn hoàn thành món ăn (ứng dụng web) một cách nhanh chóng và hiệu quả.

### Tải và cài đặt Nodejs
Để tải và cài đặt Nodejs nhằm phục vụ cho việc phát triển ứng dụng web (như dự án TeoShop), bạn có thể thực hiện theo các bước chi tiết sau đây:

#### 1. Tải Nodejs
*   Bạn truy cập vào trang chủ chính thức của Nodejs tại địa chỉ: **[https://nodejs.org/en](https://nodejs.org/en)**,.
*   Tại đây, bạn tải bộ cài đặt phù hợp với hệ điều hành của mình. Nodejs là một môi trường thực thi JavaScript đa nền tảng, mã nguồn mở và hoàn toàn miễn phí.

#### 2. Cài đặt Nodejs
*   Sau khi tải về, bạn mở tập tin và tiến hành **cài đặt như một chương trình thông thường** trên máy tính.
*   Khi bạn cài đặt Nodejs, hệ thống sẽ tự động cài đặt kèm theo **NPM (Node Package Manager)** – một công cụ quan trọng để quản lý các thư viện (package) cho ứng dụng web,.
*   Quá trình cài đặt cũng sẽ tự động thiết lập biến môi trường, cho phép bạn chạy lệnh `node` ở bất kỳ vị trí nào trong cửa sổ dòng lệnh.

#### 3. Kiểm tra cài đặt thành công
Sau khi cài đặt xong, bạn cần xác nhận Nodejs và NPM đã sẵn sàng hoạt động bằng cách sử dụng cửa sổ dòng lệnh (CMD, PowerShell hoặc Command Prompt),:

*   **Kiểm tra Nodejs:** Gõ lệnh **`node -v`**. Nếu màn hình hiển thị thông tin phiên bản (ví dụ: `v22.14.0`), nghĩa là Nodejs đã được cài đặt thành công,.
*   **Kiểm tra NPM:** Gõ lệnh **`npm -v`**. Nếu xuất hiện thông tin phiên bản (ví dụ: `10.9.2`), nghĩa là chương trình NPM đã sẵn sàng làm việc.
*   **Kiểm tra thư mục:** Bạn cũng có thể kiểm tra thủ công trong thư mục cài đặt (thường là `C:\Program Files\nodejs`) để đảm bảo có sự hiện diện của các tập tin như `node.exe` và `npm`,.

#### 4. Lưu ý quan trọng
*   Việc cài đặt thành công chỉ có nghĩa là phần mềm đã có trên máy, bạn **chưa chạy bất kỳ thành phần cụ thể nào** của Nodejs cho đến khi thực thi một đoạn mã cụ thể.
*   Nodejs bao gồm các thành phần cốt lõi như **V8 Engine** (để dịch và thực thi mã JavaScript) và **HTTP module** (để tạo web server).
*   Lập trình viên sẽ viết mã nguồn bằng JavaScript, sau đó chuyển cho Nodejs để dịch mã, thực thi chương trình và xuất kết quả.

***

Để dễ hình dung, việc cài đặt Nodejs giống như bạn **thiết lập một xưởng thủ công mỹ nghệ**: 
*   **Nodejs** chính là cái xưởng (môi trường làm việc) cung cấp đầy đủ không gian và máy móc. 
*   **JavaScript** là bản vẽ thiết kế món đồ bạn muốn làm. 
*   **NPM** giống như một cuốn danh mục phụ tùng, giúp bạn đặt mua nhanh chóng các loại ốc vít hay vật liệu có sẵn mà không cần tự mình chế tạo lại từ đầu. Khi xưởng đã dựng xong và máy móc đã sẵn sàng (đã cài đặt và kiểm tra lệnh thành công), bạn mới có thể bắt đầu bắt tay vào chế tạo sản phẩm.

### NPM
**NPM (Node Package Manager)** là một công cụ cực kỳ quan trọng trong hệ sinh thái Nodejs, được sử dụng để **quản lý các thư viện và gói phần mềm (package)** cho ứng dụng web,.

#### 1. Vai trò và Tầm quan trọng
*   **Quản lý tự động:** Do các ứng dụng web hiện nay sử dụng rất nhiều thư viện để thực hiện các chức năng, việc quản lý thủ công là không khả thi. NPM giúp tự động hóa việc cài đặt, cập nhật và quản lý các thành phần này.
*   **Thành phần phụ thuộc (Dependencies):** Các thư viện mà ứng dụng web gọi ra được coi là các "package" hoặc "thành phần phụ thuộc".

#### 2. Cấu trúc của NPM
NPM không chỉ là một phần mềm đơn lẻ mà bao gồm **3 thành phần chính**,:
*   **Website (https://www.npmjs.com/):** Nơi để lập trình viên tìm kiếm các gói thư viện cần thiết cho dự án.
*   **Công cụ dòng lệnh (Command Line Interface - CLI):** Công cụ mà lập trình viên sử dụng để tương tác, cài đặt và quản lý thư viện trực tiếp từ cửa sổ lệnh.
*   **Registry:** Một kho lưu trữ khổng lồ chứa tất cả các thư viện được chia sẻ bởi cộng đồng.

#### 3. Cách thức hoạt động
Khi bạn muốn sử dụng một thư viện (ví dụ: framework Express), quy trình diễn ra như sau:
1.  Tìm kiếm gói "express" trên **Website** NPM,.
2.  Mở **CLI** trên máy tính và gõ lệnh để tải về.
3.  CLI sẽ tự động kết nối tới **Registry** để tải gói đó về máy và tiến hành cài đặt vào dự án.

#### 4. Cài đặt và Kiểm tra
*   **Mặc định:** NPM được **cài đặt mặc định** cùng với Nodejs, vì vậy bạn không cần cài đặt nó riêng biệt,.
*   **Kiểm tra:** Để biết NPM đã sẵn sàng làm việc hay chưa, bạn mở cửa sổ dòng lệnh và gõ lệnh **`npm -v`**. Nếu màn hình hiển thị số phiên bản (ví dụ: `10.9.2`), nghĩa là chương trình đã được cài đặt thành công.
*   **Vị trí:** Bạn cũng có thể tìm thấy tập tin thực thi của `npm` trong thư mục cài đặt Nodejs (thường là `C:\Program Files\nodejs`).

***

Để dễ hiểu, bạn có thể coi **NPM giống như một "Cửa hàng ứng dụng" (App Store) dành riêng cho lập trình viên**:
*   **Website** là cái catalog để bạn xem mẫu mã.
*   **Registry** là cái kho hàng tổng chứa mọi thứ.
*   **CLI** giống như một nhân viên giao hàng; bạn chỉ cần đọc tên món đồ cần mua qua "điện thoại" (dòng lệnh), nhân viên này sẽ tự vào kho lấy đúng món đó và mang về lắp đặt tận nơi vào "ngôi nhà" (dự án) của bạn.

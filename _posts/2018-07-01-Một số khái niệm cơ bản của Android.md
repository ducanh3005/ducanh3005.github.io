---
title: Một số khái niệm cơ bản của Android
tags: Android
---

## Một số khái niệm cơ bản trong Android

---

- [Một số khái niệm cơ bản trong Android](#một-số-khái-niệm-cơ-bản-trong-android)
  - [Application là gì?](#application-là-gì)
  - [Context là gì](#context-là-gì)
  - [Quá trình build một ứng dụng trong Android](#quá-trình-build-một-ứng-dụng-trong-android)
  - [Phân biệt Service, Intent Service, AsyncTask và Thread.](#phân-biệt-service-intent-service-asynctask-và-thread)
  - [Job Scheduling là gì](#job-scheduling-là-gì)
  - [Sự khác nhau của Activity và Fragment](#sự-khác-nhau-của-activity-và-fragment)
  - [Activity lifecycle (Vòng đời của Activity)](#activity-lifecycle-vòng-đời-của-activity)
  - [Vòng đời của Fragment](#vòng-đời-của-fragment)


### Application là gì?
Lớp Application trong Android là lớp cơ sở trong ứng dụng Android chứa tất cả các component khác activity và service. Lớp Application hoặc bất kỳ lớp con nào của lớp nó sẽ được khởi tạo trước bất kỳ lớp nào khác khi process cho ứng dụng của bạn được khởi tạo

### Context là gì
Một **Context** là một đối tượng để phục vụ các xử lý liên quan tới hệ thống hay cung cấp thông tin của môi trường hệ thống. Nó cung cấp các dịch vụ để giải quyết resouce (Lấy image, string...), lấy quyền truy cập cơ sở dữ liệu và Preferences,... **Context** có thể được coi là thành phần xử lý về môi trương mà ứng dụng đang hoạt động trong đó:

**Application Context** là một context gắn liền với vòng đời của một ứng dụng. Application context có thể sử dụng khi bạn cần một context có vòng đời riêng biệt với vòng đời hiện tại hoặc khi sử dụng ngoài phạm vi của **activity**

**Activity Context** là context có sẵn trong activity, nó gắn liền với vòng đời của activity.

### Quá trình build một ứng dụng trong Android

![markdown](https://images.viblo.asia/f3c64a9c-1049-4bd4-ad50-cba2b5cdcb81.png)

### Phân biệt Service, Intent Service, AsyncTask và Thread.

* **Service** là một thành phần được sử dụng để thực hiện các tác vụ ở background ví dụ như chơi nhạc. Nó không có giao diện người dùng (user interface). Service có thể chạy ở trong background vô thời hạn ngay cả khi ứng dụng bị hủy

* **AsyncTask** cho phép bạn thực hiện các công việc bất đồng bộ ở background thread và publish kết quả lên trên UIThread mà không yêu cầu bạn xử lý các thread hay handler hoạt động

* **IntentService** là một loại *Service* để xử lý lần lượt các yêu cầu bất đồng bộ (qua Intent) ở background thread. Client sẽ yêu cầu thông qua việc gọi startService(Intent) và nó cũng không yêu cầu bạn phải "động tới" tới việc xử lý thread/ handler

* Một **Thead** là một luồng thực thi tuần tự trong một chương trình. Thread có thể coi là một *mini-process* chạy ở trong *main process*.

### Job Scheduling là gì
**Job Scheduling API** như tên gọi của nó cho phép chúng ta lên lịch công việc trong khi hệ thống sẽ thực hiện công việc tối ưu hóa dựa trên bộ nhớ, nguồn và trạng thái kết nối.

**JobSchedule** hỗ trợ lập lịch biểu các công việc. Hệ thống Android có thể kết hợp các công việc này để giảm tiêu thụ pin

**JobManager** giúp việc xử lý upload dễ dàng hơn vì nó tự động xử lý các trạng thái kết nối của mạng. Nó cũng sẽ sống sót ngay cả khi ứng dụng bị khởi động lại.

Ví dụ:
* Các tác vụ cần được thực hiện khi thiết bị được kết nối với nguồn điện.
* Các tác vụ yêu cầu truy cập mạng hoặc kết nối Wi-Fi.
* Các tác vụ không quan trọng hay không được người dụng chú ý đến.
* Các tác vụ cần được chạy thường xuyên dưới dạng hàng loạt trong đó yếu tố thời gian không quá quan trọng.

### Sự khác nhau của Activity và Fragment

* Activity là một màn hình độc lập trong ứng dụng, trong khi Fragment là một phần giao diện người dùng có thể được thêm vào hoặc xóa từ Activity
* Activity chỉ có một giao diện người dùng trong khi Fragment có thể có nhiều hơn một
* Fragment có thể tái sử dụng và chia sẻ giữa các Activity khác nhau

### Activity lifecycle (Vòng đời của Activity)
![markdown](https://images.viblo.asia/4a53c8a8-f709-4153-925e-f1add8dccdb8.png)

Như bạn có thể thấy hình vẽ phía trên biểu diễn cho 1 vòng đời của Activity.

Sơ đồ bắt đầu khi Activity launched, nghĩa là khi activity được start và hệ thống đẩy vào Backstack. Sau khi kích hoạt, lần lượt các callback như **onCreate(), onStart() và onResume** sẽ được hệ thống lần lượt call vào.

Sau khi được call vào thì Activity chính thức được xem là hoạt động (Activity Running)

Lúc này nếu có bất kỳ Activity nào đè lên, thì Activity hiện tại sẽ rơi vào trạng thái onPause. Nếu sự hiển thị của Activiy khác làm cho Activity hiện tại không còn thấy được nữa thì onStop sẽ được gọi vào ngay sau đó, ví dụ:

*Khi đang chơi game trên điện thoại và người dùng nhận được cuộc gọi, họ sẽ chuyển sang màn hình cuộc gọi và game sẽ bị tạm dừng*

Nếu người dùng ở trường hợp trên từ màn hình cuộc gọi quay lại màn hình Activity cũ đang ở trạng thái onPause() thì lúc này onResume() sẽ được gọi. Trường hợp onStop() đã được gọi thì onRestart() sẽ được gọi

Ở trường hợp người dùng ấn nút back hoặc gọi hàm finish() thì onDestroy sẽ được kích hoạt và Activity sẽ kết thúc vòng đời của nó.

### Vòng đời của Fragment

Fragment được giới thiệu ở phiên bản Android 3.0 (Honeycomb), các đối tượng Fragment là một công cụ tuyệt vời xử lý nhiều vấn đề còn tồn đọng trong Android cũ. Fragment cho phép tổ chức các thành phần giao diện người dùng của dự án cho các thiết bị khác nhau bằng cách cho bạn khả năng hiển thị nhiều phần giao diện người dùng trên 1 màn hình lớn hơn, chẳng hạn như một tablet...

Chúng cũng giúp phân đoạn code thành các khối dễ quản lý hơn thay vì code tất cả trong một Activity lớn. 

Một tính năng cuối cùng và có giá trị nhất là các Fragment cho phép ứng dụng dễ dàng điều hướng và cung cấp một cách đơn giản để giao tiếp qua lại giữa các thành phần khác nhau của ứng dụng

Một số điểm quan trọng về Fragment :

* Fragment cũng có layout của riêng của nó, cũng có các hành vi và vòng đời riêng.

* Chúng ta có thể thêm hoặc xóa Fragment trong một Activity trong khi Activity này đang chạy.

* Có thể kết hợp nhiều Fragment trong một Activity để xây dựng giao diện người dùng đa khung.

* Một Fragment có thể được sử dụng trong nhiều Activitiy.

* Vòng đời của Fragment có quan hệ chặt chẽ với vòng đời của Activity đang dùng nó, nghĩa là khi Activity bị tạm dừng thì các Fragment sẽ dừng lại.

* Fragment có thể thực hiện một hành vi mà không có trong thành phần giao diện người dùng.

![markdown](https://images.viblo.asia/e9b2f810-1e3a-4627-bcdd-0f5e0c5e6194.jpg)

Khi 1 Fragment được tạo ra nó sẽ đi qua 1 số trạng thái:

**onAttach(), onCreate(), onCreateView(), onActivityCreated()**

Sau khi fragment được hiển thị

**onStart(), onResume()**

Khi Fragment chạy ẩn dưới nền

**onPause() onStop()**

Và khi Hủy Fragment

**onPause() onStop() onDestroyView() onDestroy() onDetach()**

Các phương thức trong Fragment

Các phương thước trong Fragment :

**onAttach()** :Sự thể hiện (instance) của Fragment được gắn kết với một sự thể hiện của activity. Fragment và Activity không hoàn toàn được khởi tạo. Đặc biệt khi bạn lấy trong phương thức này một tham chiếu tới activity mà sử dụng Fragment cho công việc khởi tạo xa hơn.

**onCreate()** Hệ thống gọi phương thức này khi tạo Fragment. Bạn nên khởi tạo các thành phần cơ bản của Fragment mà bạn muốn duy trì khi Fragment bị dừng hoặc tạm dừng, sau đó được phục hồi lại.

**onCreateView()** Hệ thống gọi phương này khi cần Fragment đó để vẽ giao diện UI lần đầu tiên. Để vẽ một UI cho Fragment của bạn, bạn phải trả về một thành phần View từ phương thức này. Đó là root của layout. Bạn có thể trả về null nếu Fragment không cung cấp một giao diện UI.

**onActivityCreated()** Được gọi sau phương thức onCreateView() khi host activity được tạo. Sự thể hiện của Activity và Fragment đã được tạo cùng với cấu trúc view của activity đó. Tại điểm này, View có thể được truy cập với phương thức findViewById(). Ví dụ, trong phương thức này bạn có thể khởi tạo các đối tượng mà cần một đối tượng Context.

**onStart()** : khi Fragment hoạt động

**onResume()** Fragment hoạt động trở lại.

**onPause()** Hệ thống gọi phương thức này khi có dấu hiệu chỉ rằng người dùng đang rời khỏi Fragment này.

**onStop()** Fragment đang bị dừng bằng cách gọi phương thức này.

**onDestroyView()** Fragment view sẽ hủy sau khi gọi phương thức này.

**onDestroy()** : Được gọi để xóa trạng thái của Fragment.





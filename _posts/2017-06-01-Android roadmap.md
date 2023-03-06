---
title: Lộ trình phát triển Android
tags: roadmap android
article_header:
  type: roadmap android
  image:
    src: /screenshot.jpg
---
# Lộ trình học Android cho người mới bắt đầu 2023
Mục đích chính của bài viết này là hướng dẫn bạn có một cái nhìn tổng quát để phát triển ứng dụng Android, hỗ trợ bạn tìm thấy lối đi cho việc lập trình Android của bạn.
## Mục lục
- [Lộ trình học Android cho người mới bắt đầu 2023](#lộ-trình-học-android-cho-người-mới-bắt-đầu-2023)
  - [Mục lục](#mục-lục)
  - [Lộ trình  Android trở thành Android Developer năm 2023](#lộ-trình--android-trở-thành-android-developer-năm-2023)
  - [Ngôn ngữ lập trình Android ( Android Programming Languages)](#ngôn-ngữ-lập-trình-android--android-programming-languages)
    - [Java](#java)
    - [Kotlin](#kotlin)
  - [Các kỹ năng chung để phát triển](#các-kỹ-năng-chung-để-phát-triển)
  - [IDE để phát triển ứng dụng (Android Studio)](#ide-để-phát-triển-ứng-dụng-android-studio)
  - [Kiến thức lập trình ứng dụng](#kiến-thức-lập-trình-ứng-dụng)
  - [SQL](#sql)
  - [Git](#git)
  - [Testing (Kiểm thử phần mềm)](#testing-kiểm-thử-phần-mềm)
  - [Tổng kết](#tổng-kết)

## Lộ trình  Android trở thành Android Developer năm 2023
Lộ trình mà tôi đưa ra đây không phải là con đường duy nhất giúp bạn  trở thành Android Developer mà nó sẽ giúp bạn tiếp cận một cách khoa học  hơn. Từ đó bạn sẽ nhanh chóng phát triển kĩ năng lập trình của mình hơn

Hình ảnh phía dưới đây đã chia nhỏ các thành phần bạn cần quan tâm để lập trình Android:

![markdown](https://blog.freec.asia/wp-content/uploads/2022/04/android-developer-roadmap.png)

Nhìn vào hình vẽ phía trên thì có 13 vấn đề bạn cần quan tâm :

## Ngôn ngữ lập trình Android ( Android Programming Languages)

Các ứng dụng Android có thể phát triển bằng cách sử dụng một trong hai ngôn ngữ Kotlin, Java (ngoài ra bạn có thể sử dụng các ngôn ngữ cross khác như Dart, React Native ...) hoặc C/C++


![markdown](https://blog.freec.asia/wp-content/uploads/2022/04/ngon-ngu-android-kotlin-java.png)

Để giúp bạn hiểu rõ hơn về Kotlin và Java thì tôi sẽ phân tích rõ hơn giúp bạn

### Java

Vào hơn một tập kỷ trước, Google sử dụng Java làm ngôn ngữ chính để phát triển ứng dụng Android.

Có thể nói Java là một trong những ngôn ngữ lập trình được sử dụng phổ biến nhất. Và đây cũng là ngôn ngữ lập trình rất dễ học và hoạt động tốt trên máy ảo Dalvik. Ngoài ra, Java còn có thể di động đối với hầu hết mọi thiết bị và hệ điều hành hiện nay.

### Kotlin

Khi mới được sinh ra từ JetBrains, Kotlin được thiết kế dành cho môi trường JVM (Java Virtual Machine) và kết hợp lập trình hướng đối tượng và chức năng. Từ năm 2019, Google đã công bố Kotlin là ngôn ngữ lập trình được ưu tiên để phát triển các ứng dụng Android và các lĩnh vực khác.

Kể từ khi Google công bố, số lượng ứng dụng Android được xây dựng bằng ngôn ngữ Kotlin đã tăng lên theo cấp số nhân. Nếu bạn đang trên hành trình tìm hiểu về lộ trình học lập trình Android, hãy bắt đầu từ Kotlin. Sau đây là một số lý do:

* Khả năng tương tác: Kotlin có thể tương tác 100% với Java và với các môi trường JVM.
* An toàn: Theo số liệu mà chính Android cung cấp, các ứng dụng Android có chứa mã Kotlin có nguy cơ gặp sự cố thấp hơn 20% so với Java.
* Tính không đồng bộ (không chặn): Việc sử dụng coroutines của Kotlin cho phép ứng dụng cung cấp hỗ trợ lập trình không đồng bộ.
 

Sau khi đã có kiến thức vững vàng về cú pháp và cấu trúc của Java hay Kotlin. Bạn còn phải tìm hiểu các khái niệm sau để lập trình tốt hơn:

* Các nguyên tắc cơ bản về cách hướng đối tượng
* Biến và các kiểu dữ liệu
* Danh sách
* Câu điều kiện và vòng lặp
* ...

## Các kỹ năng chung để phát triển

* Git Version Control: Git là một hệ thống quản lý phiên bản mã nguồn mở. Git được sử dụng để theo dõi sự thay đổi trong mã nguồn của một dự án phần mềm, cho phép các thành viên của nhóm làm việc trên các phiên bản khác nhau của cùng một dự án một cách đồng bộ. Git cũng cung cấp các công cụ để quản lý các nhánh của mã nguồn, phục hồi các phiên bản cũ, và hợp nhất các thay đổi từ các nhánh khác nhau.

* HTTP/HTTPS Protocol: HTTP và HTTPS là hai giao thức truyền tải dữ liệu giữa máy tính của người dùng và máy chủ web. HTTP (Hyper Text Transfer Protocol) là giao thức truyền tải dữ liệu trên mạng Internet. HTTPS (Hyper Text Transfer Protocol Secure) cung cấp một lớp bảo mật bổ sung trên HTTP bằng cách sử dụng mã hóa để bảo vệ các dữ liệu được truyền tải.

* Terminal Usage: Terminal là một công cụ dòng lệnh được sử dụng để tương tác với hệ điều hành. Terminal cho phép người dùng nhập các lệnh để thực thi các tác vụ, tạo và quản lý tệp và thư mục, cài đặt và cấu hình các ứng dụng và hệ thống, và nhiều tác vụ khác.

* Data Structures & Algorithm: Cấu trúc dữ liệu và thuật toán là những khái niệm cơ bản trong lập trình. Cấu trúc dữ liệu là các cách tổ chức dữ liệu trong bộ nhớ của máy tính để có thể truy cập và xử lý dữ liệu hiệu quả. Thuật toán là các bước để giải quyết một vấn đề bằng cách sử dụng các cấu trúc dữ liệu và các thao tác xử lý dữ liệu.

* Design Patterns: Design patterns là các mô hình thiết kế phần mềm được sử dụng để giải quyết các vấn đề lặp lại trong thiết kế phần mềm. Các mẫu thiết kế được phát triển và cung cấp những giải pháp chuẩn hóa cho các vấn đề thường gặp trong thiết kế phần mềm. Sử dụng các design patterns có thể giúp cho việc thiết kế phần mềm trở nên dễ dàng hơn và dễ bảo trì

## IDE để phát triển ứng dụng (Android Studio)

Để lập trình được ứng dụng Android, bạn cần tìm hiểu về Môi trường phát triển tích hợp (IDE), cụ thể là Android Studio. Càng sớm làm quen với nó, làm việc sẽ càng hiệu quả hơn. Đặc biệt, Android Studios cung cấp cho bạn môi trường viết code tốt hơn nhờ các công cụ kiểm thử và debug được tích hợp trong chúng.

## Kiến thức lập trình ứng dụng

Dưới đây là danh sách các mục mà bạn cần quan tâm khi lập trình Android:

![markdown](https://blog.freec.asia/wp-content/uploads/2022/04/xay-dung-mot-ung-dung-android-roadmap.png)

* Chu kỳ sống của một ứng dụng (Android Lifecycle): Đây là thời gian mà một hoạt động trong ứng dụng Android tồn tại và chạy trên màn hình, bao gồm các trạng thái như khởi tạo, bắt đầu,tiếp tục, tạm dừng, dừng và hủy.
* [Xây dựng giao diện Android linh hoạt](https://developer.android.com/guide/components/activities/intro-activities): Đây là cách thiết kế giao diện trong ứng dụng Android linh hoạt bằng cách sử dụng Android, Fragment để chia nhỏ giao diện thành các phần nhỏ hơn, sử dụng Fragment giúp tạo ra các giao diện tái sử dụng và tương thích với nhiều kích thước màn hình khác nhau.
* [Gỡ lỗi Android Studio](https://developer.android.com/studio/debug): Đây là công cụ được tích hợp trong Android Studio để giúp lập trình viên tìm và sửa lỗi trong mã nguồn ứng dụng, tôi sẽ có 1 bài viết chi tiết về cách sử dụng gỡ lỗi trong Android Studio.
* [Sử dụng Intents và Intent Filters](https://developer.android.com/guide/components/intents-filters): Đây là cách để ứng dụng Android tìm kiếm các hoạt động (Activity) hoặc dịch vụ (Service) khác trong hệ thống để thực hiện một nhiệm vụ cụ thể.
* [Tìm hiểu đa luồng trong Android](https://developer.android.com/guide/background): Đây là khả năng của Android để thực hiện nhiều nhiệm vụ đồng thời, giúp cải thiện hiệu suất và trải nghiệm người dùng của ứng dụng.
* [Bảo mật dữ liệu](https://www.kodeco.com/6901838-data-privacy-for-android) và [bảo mật dữ liệu mạng](https://www.kodeco.com/10056112-securing-network-data-tutorial-for-android): Đây là các kỹ thuật để bảo vệ dữ liệu của người dùng trong ứng dụng Android, bao gồm các phương pháp mã hóa dữ liệu và kiểm soát truy cập đến dữ liệu.
* [Dependency injection in Android](https://developer.android.com/training/dependency-injection) Đây là một kỹ thuật giúp quản lý các phụ thuộc trong ứng dụng Android bằng cách cho phép các đối tượng được cấp phép thông qua việc chèn (inject) chúng vào các thành phần khác trong ứng dụng, thay vì phải khởi tạo chúng bên trong các thành phần đó.
* [Content Provider](https://developer.android.com/guide/topics/providers/content-providers):Đây là các ứng dụng hoặc dịch vụ khác trong hệ thống Android cung cấp dữ liệu cho ứng dụng của bạn thông qua các giao diện định sẵn (API).
* Crashlytics: Đây là một dịch vụ của Firebase của Google để giúp quản lý và giám sát lỗi trong ứng dụng Android.
* GSON: Đây là một thư viện Java/Android để chuyển đổi các đối tượng Java thành định dạng JSON và ngược lại.
* Navigation: Đây là một thành phần của Android Jetpack giúp quản lý điều hướng giữa các màn hình và phân mảnh trong ứng dụng.
* [Trình quản lý công việc (Work Manager)](https://developer.android.com/topic/libraries/architecture/workmanager): Đây là một thành phần của Android để quản lý các tác vụ trong ứng dụng, đảm bảo các tác vụ được thực hiện đúng thứ tự và đủ tài nguyên.
* Live Data, Data Binding : Đây là một cách để kết nối dữ liệu giữa thành phần giao diện và dữ liệu được lưu trữ trong cơ sở dữ liệu hoặc bất kỳ nguồn dữ liệu nào khác. Kỹ thuật này giúp tạo ra các giao diện dễ dàng thay đổi và đáp ứng các thay đổi dữ liệu một cách tự động.
* [RxJava](https://github.com/ReactiveX/RxJava), [RxKotlin](https://github.com/ReactiveX/RxKotlin): Đây là các thư viện để xử lý các sự kiện bất đồng bộ trong ứng dụng Android bằng cách sử dụng các khái niệm Reactive programming.
* [Tổng quan về quản lý bộ nhớ](https://developer.android.com/topic/performance/memory-overview?hl=vi): Đây là các kỹ thuật để quản lý bộ nhớ trong ứng dụng Android, bao gồm cách quản lý bộ nhớ đệm (cache), loại bỏ các tài nguyên không cần thiết và giải phóng bộ nhớ.
 

## SQL

Mọi ứng dụng Android đều cần lưu trữ dữ liệu dù cho đó là dữ liệu của ứng dụng hay dữ liệu của người dùng. Bên cạnh đó, ứng dụng của bạn phải được tích hợp với cơ sở dữ liệu để dễ quản lý.

Vì vậy, nếu muốn trở thành Android Developer, trong lộ trình học lập trình Android, bạn phải nắm được kiến thức SQL thật chắc.

## Git
Lập trình viên Android nói riêng và lập trình viên phần mềm nói chung đều phải học sử dụng Git để quản lý mã nguồn của mình. Bạn nên tìm hiểu những điều cơ bản về Git như tạo và sử dụng kho lưu trữ, biết cách commit, thay đổi commit…

##XML
XML là viết tắt của Extensible Markup Language được sử dụng chủ yếu trong việc lập trình web. Nhưng nó cũng là một công nghệ không thể thiếu để lập trình ứng dụng Android.

Sở dĩ bạn nên tìm hiểu về XML vì nhiều ứng dụng Android thường yêu cầu chuyển dữ liệu sang Web Services và ngược lại. Hiểu về XML là một kỹ năng phải có nếu bạn muốn trở thành một Android Developer chính hiệu.

##Nguyên tắc thiết kế Material
Mọi ứng dụng Android đều phải được lập trình tuân theo các nguyên tắc về Material Design. Các nguyên tắc liên quan đến những yếu tố cần thiết trong ứng dụng như vị trí phần tử, chuyển tiếp, màu sắc, sắc thái… Nếu ứng dụng Android không tuân thủ các nguyên tắc này sẽ không được Google chấp thuận để xuất bản lên Google Play.

##Web Back end
Bạn có thể tìm hiểu về kiến thức này để trở thành một lập trình viên Android Full Stack có thể lập trình cả ứng dụng di động và Web.

Nếu định hướng của bạn không phải trở thành Android Full Stack mà là một Android Developer chuyên nghiệp thì cũng nên tìm hiểu về kiến thức này. Vì hiểu về nghiệp vụ Web Back end giúp bạn thuận tiên hơn để phối hợp với team (Vì ứng dụng di động và Web thường đi song song với nhau)

## Testing (Kiểm thử phần mềm)
Sau khi viết xong một ứng dụng, việc kiểm thử giúp bạn phát hiện các sai sót trong quá trình code. Tất nhiên các Công ty lớn sẽ có bộ phận Tester riêng.

Tuy nhiên hiểu về kiến thức này giúp bạn nhanh chóng phát hiện các lỗi trong mã nguồn và xác định rằng ứng dụng vẫn đang hoạt động tốt. Vì vậy, trong lộ trình học Android, hãy học thêm về Testing

Bạn có thể thực hiện kiểm tra ứng dụng sau khi lập trình ứng dụng thông qua các phương pháp sau:

Unit Testing
Jasmine
ESLint
Karma
Jest
E2E Testing
Protractor
Cypress

##App Manifest
Mọi dự án Android được lập trình phải có tệp AndroidManifest.xml nhằm mục tiêu mô tả thông tin cần thiết về ứng dụng để theo dõi như tên gói, điểm nhập, quyền, thành phần và siêu dữ liệu.

![markdown](https://blog.freec.asia/wp-content/uploads/2022/04/app-manifest.png)

## Tổng kết

Với bài viết này, Mình hi vọng bạn sẽ có lộ trình cụ thể về Android) chỉnh chu, chuyên nghiệp giúp bạn sẽ có định hướng tốt nhất cho các bạn theo đuổi và phát triển sự nghiệp của mình





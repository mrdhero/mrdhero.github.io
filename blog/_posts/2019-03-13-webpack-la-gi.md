## Webpack là gì?

Là một lập trình viên Frontend chắc hẳn bạn đã từng nghe đến khái niệm Webpack. Nếu bạn đã từng trải qua cảm giác nhức đầu khi sử dụng Gulp để đóng gói asset hay các dependence thì xin chúc mừng, Webpack là sự thay thế tuyệt vời dành cho bạn. 

Webpack, đơn giản là một công cụ giúp đóng gói toàn bộ asset (CSS, JS, Image, Font,...) thành một (hoặc nhiều file) theo cách ngăn nắp, khoa học và đảm bảo được sự phụ thuộc giữa các dependence.

## Tại sao nên sử dụng Webpack?

Để hiểu lý do tại sao nên sử dụng webpack, xin nhắc lại một chút rằng có hai cách để chạy Javascript trong trình duyệt. 

Đầu tiên là import một file .js tương ứng với mỗi chức năng. Giải pháp này giúp việc quản lý trở nên dễ dàng hơn nhưng lại khó mở rộng, vì cần phải đảm bảo thứ tự, sự phụ thuộc lẫn nhau giữa các phần, chưa kể việc trình duyệt phải tải quá nhiều JS có thể dẫn tới tắc nghẽn. 

Tùy chọn thứ hai là sử dụng một file .js lớn chứa tất cả code của bạn, nhưng cách này lại làm phát sinh các vấn đề về scope, kích thước file, khả năng đọc hiểu và maintain code. 

Và Webpack đã ra đời giải quyết vấn đề của cả hai cách trên. Bạn vẫn có thể thoải mái chia code thành từng phần, chức năng nhỏ trong khi Webpack sẽ giúp bạn gom tất cả lại một chỗ. Ngoài ra Webpack còn "bonus" thêm cho bạn nhiều tính năng như cache, optimize code, watch file,... quá tuyệt vời phải không nào?

## Cài đặt Webpack

Để cài đặt phiên bản mới nhất của Webpack, chúng ta chạy lệnh sau
```shell
npm install --save-dev webpack
```
Câu lệnh sẽ tiến hành cài đặt Webpack vào folder của project.

> Lưu ý: Webpack nên được cài đặt local tại folder của project thay vì cài đặt global. Thường thì chúng ta chỉ sử dụng Webpack trong quá trình develop. Việc cài đặt global có thể gây ảnh hưởng đến những project sử dụng các phiên bản Webpack khác với phiên bản được cài.

Ngoài ra chúng ta cũng cần cài đặt Webpack CLI
```shell
npm install --save-dev webpack-cli
```
Đây chính là cách mà chúng ta tương tác với Webpack thông qua giao diện Command Line.

Ở bài tiếp theo chúng ta sẽ cùng nhau tìm hiểu cách sử dụng Webpack trong một dự án JS.
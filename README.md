# WEBPACK
* Webpack là gì? Tại sao phải sử dụng Webpack
Là 1 cách để đóng gói các module bundler đơn lẻ, nó tạo ra các modules với các dependencies và tạo ra các assets tĩnh đại diện cho các module này.
* Sử dụng Webpack với HTML source/Phaser được không?

### Concepts
![N|Solid](https://cdn.scotch.io/1/OgOa3kqeStetJOfDqZyI_1HB2N57.png)

### Bắt đầu sử dụng
```
npm install webpack - g
```

### Tạo một project Webpack
* Tạo source (index.html và bundle.js)
* chạy lệnh để bundle app
```
webpack ./app.js bundle.js
```
* Khai báo file config
```
module.exports = {
  entry: "./app.js",
  output: {
    filename: "bundle.js"
  }
}
```
* entry: tạm hiểu như là 1 FILE khởi tạo đầu tiên (có thể là file đơn lẻ hoặc mảng các file) - mà chúng ta cần nhúng vào và build.
* output: là 1 file file đối tượng chứa tất cả cấu hình output.
* Chạy app
```
webpack
```
Sau khi đã tạo file webpack.config.js chúng ta có thể sử dụng lệnh webpack như trên.

### Mở rộng các hàm trong file config và webpack
* ------- Watchmode -------
Có tác dụng 'watch' các files và một khi các files thay đổi, nó lập tức build lại và tạo lại các các file output.
* Có 2 cách để bật chế độ watchmode
* Sử dụng command line
```
webpack --watch
```
* Go vào file config, và thêm key gọi là watch và đặt là "true"
```
module.exports = {
  entry: "./app.js",
  output: {
    filename: "bundle.js"
  },
  watch: true
}
```
* ------- Webpack Dev Server -------

Webpack có 1 web server được gọi là webpack-dev-server
Từ command line, chúng ta cài đặt webpack-dev-server cho globally:

```
npm install webpack-dev-server -g
```

* Sau khi cài đặt server chúng ta có thể vào folder web app và chạy lệnh

```
webpack-dev-server
```
* Sau khi chạy có thể vào server với link sau, tùy port của chúng ta khi chạy thì có thể thay "8080" thành port tương ứng của bundle
```
localhost:8080
```

* Để xem log của Webpack có thể truy cập như sau để xem
```
http://localhost:8080/webpack-dev-server/
```

### Nguồn tham khảo
* [Guide to Webpack] - bài viết ở medium rất chi tiết về cách sử dụng và các tính năng của webpack

### Editors

* [Sublime Text] - Light weight editor and easy to code and hightlight your work.
* [Atom] - Powerful code editor now with thoundsand of plugins.

### Todos


**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [Webpack JS]: <https://webpack.js.org/>
   [Guide to Webpack]: <https://medium.com/@dabit3/beginner-s-guide-to-webpack-b1f1a3638460>

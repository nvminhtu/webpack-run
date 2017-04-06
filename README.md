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
* 1. Sử dụng command line
```
webpack --watch
```
* 2. Go vào file config, và thêm key gọi là watch và đặt là "true"
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

### Editors

* [Sublime Text] - Light weight editor and easy to code and hightlight your work.
* [Atom] - Powerful code editor now with thoundsand of plugins.

### Todos


**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)

   [Webpack JS]: <https://webpack.js.org/>
   [Atom]: <https://atom.io/>
   [Freebies UI Kit]: <http://freebiesbug.com/psd-freebies/ui-kits/>
   [Sketch App Resources]: <https://www.sketchappsources.com/category/ui.html>

   [Kenney.nl]: <http://www.kenney.nl>
   [OpenGameArt.org]: <http://www.OpenGameArt.org>
   [Untamed.wild-refuge.net]: <http://www.Untamed.wild-refuge.net>
   [Crateboy.itch.io]: <http://www.Crateboy.itch.io>
   [Opengamegraphics.com]: <http://www.Opengamegraphics.com>
   [Gameart2d.com]: <http://www.Gameart2d.com>
   [Wigdetworx.com]: <http://www.Wigdetworx.com>
   [GlitchtheGame.com]: <http://www.GlitchtheGame.com>
   [Dumbanex.com]: <http://www.Dumbanex.com>
   [Reinerstilesets.de]: <http://www.Reinerstilesets.de>
   [Sharecg.com]: <http://www.Sharecg.com>
   [Roenica.com]: <http://www.Roenica.com>
   [Blogoscoped.com]: <http://www.Blogoscoped.com>
   [Lostgarden.com]: <http://www.Lostgarden.com>
   [Subtlepatterns.com]: <http://www.Subtlepatterns.com>
   [Openclipart.org]: <http://www.Openclipart.org>

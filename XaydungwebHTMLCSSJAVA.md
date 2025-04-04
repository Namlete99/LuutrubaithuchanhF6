# Xây dựng web bằng HTML; CSS; Java 

***

## `index.html`
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Kỉ yếu lớp 12A</title>
    <link rel="stylesheet" href="./test.css" type="text/css" />
  </head>
  <body>
    <!--Phần đầu lớp web-->
    <table class="customtable">
      <!--Phần Tiêu đề trang-->
      <tr>
        <td colspan="2" class="customtable1">
          <p class="title">Kỉ yếu lớp 12A</p>
        </td>
      </tr>
    </table>

    <!--Phần thân trang web -->
    <table border="1" class="customtable2">
      <!--Phần mục (bảng 1)-->
      <tr>
        <td><a href="gioithieu.html" target="iframe_noidung">Trang chủ</a></td>
      </tr>
      <tr>
        <td><a href="hoatdong.html" target="iframe_noidung">Hoạt động</a></td>
      </tr>
      <tr>
        <td>
          <a href="thanhvienlop.html" target="iframe_noidung">Thành viên lớp</a>
        </td>
      </tr>
    </table>

    <!--Phần nội dung của mục (bảng 2)-->
    <table class="table1">
      <tr>
        <td class="customtd"></td>
        <td>
          <iframe
            src="gioithieu.html"
            name="iframe_noidung"
            class="customeiframe"
          ></iframe>
        </td>
      </tr>
    </table>
    <hr />
    <!--Chân trang-->
    <center>
      <header>
        <h2>Dễ dàng truy cập và theo dõi</h2>
        <br />
        <p>
          Bạn đang ghé thăm kỉ yếu lớp 12A6 - Xin cảm ơn đã quan tâm kỉ yếu của
          lớp 12A6
        </p>
        <br />
      </header>
      <footer>© Copyright, Lớp 12A6 2024 - 2025</footer>
    </center>
  </body>
</html>

```

***

## `test.css`

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
/* Xóa gạch chân & đổi màu mặc định */
a {
  text-decoration: none;
  color: rgb(35, 42, 238); /* Màu bình thường */
  font-size: 15px;
  font-family: "Times New Roman", serif;
  transition: color 0.3s ease; /* Hiệu ứng mượt */
}

/* Khi di chuột vào, đổi màu */
a:hover {
  color: orange; /* Đổi thành màu đỏ */
}

table a:hover {
  color: orange;
}

/* Nội dung */

/* Phần tiêu đề */
.title {
  font-family: "Times New Roman", serif;
  color: coral;
  font-size: 50px;
  font-weight: bold;
}

/* Phần thân trang mục 1 */
.customtable {
  width: 100%;
  border-spacing: 0;
}

.customtable1 {
  text-align: center;
}

.customtable2 {
  width: 10%;
  border-spacing: 0;
  vertical-align: top; /* Căn nội dung lên trên */
}

/* Phần thân trang mục 2 */
.table1 {
  width: 100%;
  height: 1000px;
  border: none;
  border-spacing: 0;
}

.customtd {
  width: 10%;
  vertical-align: top;
}

.customeiframe {
  width: 100%;
  height: 1000px;
  border: none;
}

/* Chân trang */
.footer,
.header {
  font-family: "Times New Roman", Times, serif;
  font-size: 3px;
}
/* thanhvienlop.html */

.title1 {
  font-family: "Times New Roman", serif;
  color: rgb(44, 105, 220);
  font-size: 20px;
  font-weight: bolder;
}

.title2 {
  font-family: "Times New Roman", serif;
  font-style: normal;
  color: rgb(36, 93, 199);
  font-size: 30px;
  font-weight: bolder;
}

.title3 {
  font-family: "Times New Roman", Times, serif;
  color: rgb(36, 93, 199);
  font-size: 17px;
}
.table {
  border-collapse: collapse;
  border: 1px solid cornflowerblue; /* Viền xanh nước biển */
}

.table th,
.table td {
  border: 1px solid cornflowerblue; /* Viền xanh nước biển */
  padding: 8px;
  text-align: center;
}

```

***

##  `thanhvienlop.htmlhtml`

```thanhvienlop.html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Thành viên lớp</title>
    <link rel="stylesheet" href="./test.css" type="text/css" />
  </head>
  <body>
    <!--Tiêu đề bảng-->
    <table width="700" valign="top">
      <tr>
          <td colspan="2" align="center"><div class="title2">Thành viên lớp</div></td>
      </tr>
    </table>
    <!--Bảng thành viên lớp-->
    <table class="table" id="studentTable">
      <thead>
        <tr>
          <th width="10%">STT</th>
          <th width="40%">Họ và tên</th>
          <th width="15%">Ngày sinh</th>
          <th width="20%">Chức vụ</th>
          <th width="15%"></th>
        </tr>
      </thead>
      <tbody>
      </tbody>

      <!--Tạo bảng so clean bằng json và java-->
      <script src="./script.js"></script>
  </body>
</html>
```

***

## `script.js`

```java
// Lấy dữ liệu từ file JSON và hiển thị trong bảng
fetch("students.json")
  .then((response) => response.json()) // Chuyển đổi dữ liệu JSON thành đối tượng JavaScript
  .then((students) => {
    const tbody = document.querySelector("#studentTable tbody");
    students.forEach((student) => {
      let row = `<tr>
                <td>${student.STT}</td>
                <td>${student.HoTen}</td>
                <td>${student.NgaySinh}</td>
                <td>${student.ChucVu ? student.ChucVu : "-"}</td>
                <td><a href="#">${student.ChiTiet}</a></td>
            </tr>`;
      tbody.innerHTML += row;
    });
  })
  .catch((error) => console.error("Lỗi khi tải JSON:", error));
```

***

## `students.json`

```Json
[
  {
    "STT": 1,
    "HoTen": "Lê Huỳnh Duy Anh",
    "NgaySinh": "25/06/2007",
    "ChucVu": "TNXK",
    "ChiTiet": "Xem chi tiết"
  },
  {
    "STT": 2,
    "HoTen": "Nguyễn Việt Anh",
    "NgaySinh": "29/07/2007",
    "ChucVu": "",
    "ChiTiet": "Xem chi tiết"
  },
  {
    "STT": 3,
    "HoTen": "Phạm Đào Quốc Anh",
    "NgaySinh": "20/05/2007",
    "ChucVu": "TNXK",
    "ChiTiet": "Xem chi tiết"
  },
  {
    "STT": 4,
    "HoTen": "Lương Hồng Kim Bảo",
    "NgaySinh": "20/05/2007",
    "ChucVu": "",
    "ChiTiet": "Xem chi tiết"
  }
]
```

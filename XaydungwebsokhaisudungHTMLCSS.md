# Xây dựng web sơ khai khi chỉ sử dụng HTML; CSS

***

## index.html

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
        <td colspan="2" class="customtable1"><p class="title">Kỉ yếu lớp 12A</p></td>
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
        <td><a href="thanhvienlop.html" target="iframe_noidung">Thành viên lớp</a></td>
      </tr>
    </table>

    <!--Chân trang-->
    <center>
      <header>
        <h2>Dễ dàng truy cập và theo dõi</h2>
        <p>Bạn đang ghé thăm kỉ yếu lớp 12A6 - Xin cảm ơn đã quan tâm kỉ yếu của lớp 12A6</p>
      </header>
      <footer>© Copyright, Lớp 12A6 2024 - 2025</footer>
    </center>
  </body>
</html>
```

***

## test.css

``` css
/* Xóa gạch chân & đổi màu mặc định */
a {
  text-decoration: none;
  color: blue; /* Màu bình thường */
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
  color: orange;
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
  font-style: normal;
  color: blue;
  font-size: 20px;
}

.title2 {
  font-family: "Times New Roman", serif;
  font-style: normal;
  color: blue;
  font-size: 30px;
}

.table {
  border-collapse: collapse;
  border: 1px solid blue; /* Viền xanh nước biển */
}

.table th,
.table td {
  border: 1px solid blue; /* Viền xanh nước biển */
  padding: 8px;
  text-align: center;
}
```

***

## `thanhvienlop.html`

```html
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
        <td colspan="2" align="center">
          <font face="Times New Roman" color="blue" size="6px"><b>Thành viên lớp</b></font>
      </td>
      </tr>
    </table>
    <!--Bảng thành viên lớp-->
    <table class="table" width="700" height="10">
      <tr>
        <th width="10%">STT</th>
        <th width="40%">Họ và tên</th>
        <th width="15%">Ngày sinh</th>
        <th width="20%">Chức vụ</th>
        <th width="15%"></th>
      </tr>
      <tr>
        <td>1</td>
        <td><p align="left">Lê Huỳnh Duy Anh</p></td>
        <td>25/06/2007</td>
        <td>TNXK</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr>
        <td>2</td>
        <td><p align="left">Nguyễn Việt Anh</p></td>
        <td>29/07/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr>
        <td>3</td>
        <td><p align="left">Phạm Đào Quốc Anh</p></td>
        <td>20/05/2007</td>
        <td>TNXK</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr>
        <td>4</td>
        <td><p align="left">Lương Hồng Kim Bảo</p></td>
        <td>14/12/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr>
        <td>5</td>
        <td><p align="left">Ngô Quốc Bình</p></td>
        <td>17/11/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr>
        <td>6</td>
        <td><p align="left">Huỳnh Ngọc Lan Chi</p></td>
        <td>26/12/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiế</a>t</td>
      </tr>
      <tr>
        <td>7</td>
        <td><p align="left">Nguyễn Ngọc Kiên Cường</p></td>
        <td>22/08/2007</td>
        <td>TNXK</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr>
        <td>8</td>
        <td><p align="left">Đỗ Nguyễn Ngọc Duy</p></td>
        <td>08/01/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr>
        <td>9</td>
        <td><p align="left">Lê Thị Ngọc Điệp</p></td>
        <td>29/12/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr>
        <td>10</td>
        <td><p align="left">Phan Hữu Đức</p></td>
        <td>29/03/2007</td>
        <td>Tổ trưởng tổ 1</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr>
        <td>11</td>
        <td><p align="left">Trịnh Ngọc Hải</p></td>
        <td>08/08/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr>
        <td>12</td>
        <td><p align="left">Nguyễn Lê Ngọc Hân</p></td>
        <td>07/09/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr>
        <td>13</td>
        <td><p align="left">Võ Huỳnh Ngọc Hân</p></td>
        <td>30/01/2007</td>
        <td>Sao đỏ</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>14</td>
        <td><p align="left">Châu Thị Kim Hoa</p></td>
        <td>02/06/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      <tr>
          <td>15</td>
          <td><p align="left">Nguyễn Hoàng Huy</p></td>
          <td>28/09/2007</td>
          <td>Lớp phó lao động</td>
          <td><a href="#">Xem chi tiết</a></td>
      </tr>
      </tr>
      <tr>
        <td>16</td>
        <td><p align="left">Nguyễn Phúc Gia Hưng</p></td>
        <td>02/08/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr>
        <td>17</td>
        <td><p align="left">Nguyễn Bách Khang</p></td>
        <td>22/07/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>18</td>
        <td><p align="left">Tạ Vũ Chí Khang</p></td>
        <td>28/08/2007</td>
        <td>Phó bí thư</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>19</td>
        <td><p align="left">Trần Minh Khang</p></td>
        <td>19/10/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>20</td>
        <td><p align="left">Nguyễn Thành Luân</p></td>
        <td>05/06/2007</td>
        <td>TNXK</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>21</td>
        <td><p align="left">Trương Xuân Ngọc Mai</p></td>
        <td>25/09/2007</td>
        <td>Sao đỏ</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>22</td>
        <td><p align="left">Nguyễn Lê Nam</p></td>
        <td>15/08/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>23</td>
        <td><p align="left">Mai Phương Ngân</p></td>
        <td>16/08/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>24</td>
        <td><p align="left">Nguyễn Tuyết Ngân</p></td>
        <td>20/12/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>25</td>
        <td><p align="left">Vũ Ngọc Thy Ngân</p></td>
        <td>05/07/2007</td>
        <td>Tổ trưởng tổ 2</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>26</td>
        <td><p align="left">Trần Thị Tuyết Nhung</p></td>
        <td>11/08/2007</td>
        <td>Tổ trưởng tổ 4</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>27</td>
        <td><p align="left">Cao Văn Phúc</p></td>
        <td>13/08/2007</td>
        <td>Lớp trưởng</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>28</td>
        <td><p align="left">Ngô Trần Anh Phúc</p></td>
        <td>04/10/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>29</td>
        <td><p align="left">Tôn Thất Minh Quân</p></td>
        <td>08/11/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>30</td>
        <td><p align="left">Phan Trần Ngọc Quý</p></td>
        <td>14/02/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>31</td>
        <td><p align="left">Mai Thúc Sinh</p></td>
        <td>16/08/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>32</td>
        <td><p align="left">Lê Đỗ Minh Tài</p></td>
        <td>22/04/2007</td>
        <td>TNXK</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>33</td>
        <td><p align="left">Đinh Nguyễn Minh Thơ</p></td>
        <td>13/10/2007</td>
        <td>TNXK</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>34</td>
        <td><p align="left">Nguyễn Huỳnh Ánh Thư</p></td>
        <td>16/07/2007</td>
        <td>Bí thư</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>35</td>
        <td><p align="left">Nguyễn Khánh Thy</p></td>
        <td>01/04/2007</td>
        <td>lớp phó học tập</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>36</td>
        <td><p align="left">Vũ Thủy Tiên</p></td>
        <td>24/12/2007</td>
        <td>Thủ quỹ</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>37</td>
        <td><p align="left">Đào Nguyễn Diệp Tiền</p></td>
        <td>14/05/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>38</td>
        <td><p align="left">Lê Minh Tiến</p></td>
        <td>30/11/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>39</td>
        <td><p align="left">Huỳnh Đặng Quỳnh Trang</p></td>
        <td>23/10/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>40</td>
        <td><p align="left">Phạm Minh Trang</p></td>
        <td>17/11/2007</td>
        <td>Tổ trưởng tổ 3</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>41</td>
        <td><p align="left">Trần Ngọc Thanh Trúc</p></td>
        <td>03/11/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>42</td>
        <td><p align="left">Lê Thành Trường</p></td>
        <td>25/02/2007</td>
        <td>TNXK</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>43</td>
        <td><p align="left">Nguyễn Quang Vịnh</p></td>
        <td>02/03/2007</td>
        <td>TNXK</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>44</td>
        <td><p align="left">Nguyễn Thảo Vy</p></td>
        <td>13/08/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>45</td>
        <td><p align="left">Phan Thị Kim Yến</p></td>
        <td>10/03/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr >
        <td>46</td>
        <td><p align="left">Hoàng Hải Đăng</p></td>
        <td>09/07/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
    </table>
  </body>
</html>
```

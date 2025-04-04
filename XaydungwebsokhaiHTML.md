# Xây dựng web sơ khai khi chỉ sử dụng HTML

## index.html


```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Kỉ yếu lớp 12A</title>
  </head>
  <body>
    <!--Phần đầu lớp web-->
    <table width="100%" border="0" cellspacing="0">
      <!--Phần Tiêu đề trang-->
      <tr>
        <td colspan="2" align="center">
            <font face="Times New Roman" size="10px" color="coral">
                <b>Kỉ yếu lớp 12A</b>
            </font>
        </td>
      </tr>
    </table>

    <!--Phần thân trang web -->
    <table width="10%" valign="top" border="1" cellspacing="0">
      <!--Phần mục (bảng 1)-->
      <tr>
        <td>
          <a href="trangchu.html" target="iframe_noidung"><font color="royal blue">Trang chủ</font></a>
        </td>
      </tr>
      <tr>
        <td>
          <a href="hoatdong.html" target="iframe_noidung"><font color="royal blue">Hoạt động</font></a>
        </td>
      </tr>
      <tr>
        <td>
          <a href="./thanhvienlop.html" target="iframe_noidung"><font color="royal blue"> Thành viên lớp</font></a>
        </td>
      </tr>
    </table>

    <!--Phần nội dung của mục (bảng 2)-->
    <table width="100%" height="1000px" border="0" cellspacing="0">
      <tr>
        <td width="10%" valign="top"></td>
        <td>
          <iframe src="gioithieu.html" name="iframe_noidung" width="100%" height="1000px" frameborder="0"></iframe>
        </td>
      </tr>
    </table>
    <hr />

    <!--Chân trang-->
    <center>
      <header>
        <font face="Times New Roman" size="3">
          <h2>Dễ dàng truy cập và theo dõi</h2>
          <p>
            Bạn đang ghé thăm kỉ yếu lớp 12A6 - Xin cảm ơn đã quan tâm kỉ yếu
            của lớp 12A6
          </p>
        </font>
      </header>
      <footer>
        <font size="3px">© Copyright, Lớp 12A6 2024 - 2025</font>
      </footer>
    </center>
  </body>
</html>
```

***

## thanhvienlop.html 

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>Thành viên lớp</title>
  </head>
  <body>
    <!--Tiêu đề bảng-->
    <table border="0" width="700" valign="top">
      <tr>
        <td colspan="2" align="center">
          <font face="Times New Roman" color="cornflowerblue" size="6px"><b>Thành viên lớp</b></font>
        </td>
      </tr>
    </table>
    <br>
    <!--Bảng thành viên lớp-->
    <table border="1" width="700" height="10" cellspacing="0">
      <tr>
        <th width="10%"><font color="cornflowerblue">STT</font></th>
        <th width="40%"><font color="cornflowerblue">Họ và tên</font></th>
        <th width="15%"><font color="cornflowerblue">Ngày sinh</font></th>
        <th width="20%"><font color="cornflowerblue">Chức vụ</font></th>
        <th width="15%"></th>
      </tr>
      <!--Thông tin 46 học sinh-->
      <tr align="center">
        <td><font color="cornflowerblue">1</font></td>
        <td><p align="left"><font color="cornflowerblue">Lê Huỳnh Duy Anh</font></p></td>
        <td><font color="cornflowerblue">25/06/2007</font></td>
        <td><font color="cornflowerblue">TNXK</font></td>
        <td><a href="#"><font color="cornflowerblue">Xem chi tiết</font></a></td>
      </tr>
      <tr align="center">
        <td>2</td>
        <td><p align="left">Nguyễn Việt Anh</p></td>
        <td>29/07/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>3</td>
        <td><p align="left">Phạm Đào Quốc Anh</p></td>
        <td>20/05/2007</td>
        <td>TNXK</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>4</td>
        <td><p align="left">Lương Hồng Kim Bảo</p></td>
        <td>14/12/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>5</td>
        <td><p align="left">Ngô Quốc Bình</p></td>
        <td>17/11/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>6</td>
        <td><p align="left">Huỳnh Ngọc Lan Chi</p></td>
        <td>26/12/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiế</a>t</td>
      </tr>
      <tr align="center">
        <td>7</td>
        <td><p align="left">Nguyễn Ngọc Kiên Cường</p></td>
        <td>22/08/2007</td>
        <td>TNXK</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>8</td>
        <td><p align="left">Đỗ Nguyễn Ngọc Duy</p></td>
        <td>08/01/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>9</td>
        <td><p align="left">Lê Thị Ngọc Điệp</p></td>
        <td>29/12/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>10</td>
        <td><p align="left">Phan Hữu Đức</p></td>
        <td>29/03/2007</td>
        <td>Tổ trưởng tổ 1</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>11</td>
        <td><p align="left">Trịnh Ngọc Hải</p></td>
        <td>08/08/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>12</td>
        <td><p align="left">Nguyễn Lê Ngọc Hân</p></td>
        <td>07/09/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>13</td>
        <td><p align="left">Võ Huỳnh Ngọc Hân</p></td>
        <td>30/01/2007</td>
        <td>Sao đỏ</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>14</td>
        <td><p align="left">Châu Thị Kim Hoa</p></td>
        <td>02/06/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      <tr align="center">
          <td>15</td>
          <td><p align="left">Nguyễn Hoàng Huy</p></td>
          <td>28/09/2007</td>
          <td>Lớp phó lao động</td>
          <td><a href="#">Xem chi tiết</a></td>
      </tr>
      </tr>
      <tr align="center">
        <td>16</td>
        <td><p align="left">Nguyễn Phúc Gia Hưng</p></td>
        <td>02/08/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>17</td>
        <td><p align="left">Nguyễn Bách Khang</p></td>
        <td>22/07/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>18</td>
        <td><p align="left">Tạ Vũ Chí Khang</p></td>
        <td>28/08/2007</td>
        <td>Phó bí thư</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>19</td>
        <td><p align="left">Trần Minh Khang</p></td>
        <td>19/10/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>20</td>
        <td><p align="left">Nguyễn Thành Luân</p></td>
        <td>05/06/2007</td>
        <td>TNXK</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>21</td>
        <td><p align="left">Trương Xuân Ngọc Mai</p></td>
        <td>25/09/2007</td>
        <td>Sao đỏ</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>22</td>
        <td><p align="left">Nguyễn Lê Nam</p></td>
        <td>15/08/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>23</td>
        <td><p align="left">Mai Phương Ngân</p></td>
        <td>16/08/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>24</td>
        <td><p align="left">Nguyễn Tuyết Ngân</p></td>
        <td>20/12/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>25</td>
        <td><p align="left">Vũ Ngọc Thy Ngân</p></td>
        <td>05/07/2007</td>
        <td>Tổ trưởng tổ 2</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>26</td>
        <td><p align="left">Trần Thị Tuyết Nhung</p></td>
        <td>11/08/2007</td>
        <td>Tổ trưởng tổ 4</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>27</td>
        <td><p align="left">Cao Văn Phúc</p></td>
        <td>13/08/2007</td>
        <td>Lớp trưởng</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>28</td>
        <td><p align="left">Ngô Trần Anh Phúc</p></td>
        <td>04/10/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>29</td>
        <td><p align="left">Tôn Thất Minh Quân</p></td>
        <td>08/11/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>30</td>
        <td><p align="left">Phan Trần Ngọc Quý</p></td>
        <td>14/02/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>31</td>
        <td><p align="left">Mai Thúc Sinh</p></td>
        <td>16/08/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>32</td>
        <td><p align="left">Lê Đỗ Minh Tài</p></td>
        <td>22/04/2007</td>
        <td>TNXK</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>33</td>
        <td><p align="left">Đinh Nguyễn Minh Thơ</p></td>
        <td>13/10/2007</td>
        <td>TNXK</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>34</td>
        <td><p align="left">Nguyễn Huỳnh Ánh Thư</p></td>
        <td>16/07/2007</td>
        <td>Bí thư</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>35</td>
        <td><p align="left">Nguyễn Khánh Thy</p></td>
        <td>01/04/2007</td>
        <td>lớp phó học tập</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>36</td>
        <td><p align="left">Vũ Thủy Tiên</p></td>
        <td>24/12/2007</td>
        <td>Thủ quỹ</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>37</td>
        <td><p align="left">Đào Nguyễn Diệp Tiền</p></td>
        <td>14/05/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>38</td>
        <td><p align="left">Lê Minh Tiến</p></td>
        <td>30/11/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>39</td>
        <td><p align="left">Huỳnh Đặng Quỳnh Trang</p></td>
        <td>23/10/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>40</td>
        <td><p align="left">Phạm Minh Trang</p></td>
        <td>17/11/2007</td>
        <td>Tổ trưởng tổ 3</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>41</td>
        <td><p align="left">Trần Ngọc Thanh Trúc</p></td>
        <td>03/11/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>42</td>
        <td><p align="left">Lê Thành Trường</p></td>
        <td>25/02/2007</td>
        <td>TNXK</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>43</td>
        <td><p align="left">Nguyễn Quang Vịnh</p></td>
        <td>02/03/2007</td>
        <td>TNXK</td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>44</td>
        <td><p align="left">Nguyễn Thảo Vy</p></td>
        <td>13/08/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
        <td>45</td>
        <td><p align="left">Phan Thị Kim Yến</p></td>
        <td>10/03/2007</td>
        <td></td>
        <td><a href="#">Xem chi tiết</a></td>
      </tr>
      <tr align="center">
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

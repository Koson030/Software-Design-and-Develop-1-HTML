# ใบงานการทดลอง HTML

## การทดลองที่ 5: การสร้างตารางและรายการ
### วัตถุประสงค์
- เรียนรู้การสร้างตารางข้อมูล
- เรียนรู้การสร้างรายการแบบต่างๆ

### ขั้นตอนการทดลอง
1. สร้างไฟล์ tablelist.html ดังตัวอย่าง:
```html
<table border="1">
    <thead>
        <tr>
            <th>Header 1</th>
            <th>Header 2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Row 1, Cell 1</td>
            <td>Row 1, Cell 2</td>
        </tr>
        <tr>
            <td>Row 2, Cell 1</td>
            <td>Row 2, Cell 2</td>
        </tr>
    </tbody>
</table>
```

### คำอธิบายเพิ่มเติม
- `<table>` กำหนดขอบเขตของตาราง
- `<thead>` สำหรับส่วนหัวตาราง
- `<tbody>` สำหรับเนื้อหาตาราง
- `<tr>` แทนแถว
- `<th>` แทนเซลล์หัวตาราง
- `<td>` แทนเซลล์ข้อมูล

2. การสร้างรายการ โดยเพิ่มเติม Code ในไฟล์ tablelist.html :
```html
<ul>
    <li>Unordered item 1</li>
    <li>Unordered item 2</li>
</ul>
<ol>
    <li>Ordered item 1</li>
    <li>Ordered item 2</li>
</ol>

<dl>
    <dt>Term 1</dt>
    <dd>Definition 1</dd>
    <dt>Term 2</dt>
    <dd>Definition 2</dd>
</dl>
```

### คำอธิบายเพิ่มเติม
- `<ul>` สำหรับรายการแบบไม่เรียงลำดับ
- `<ol>` สำหรับรายการแบบเรียงลำดับ
- `<dl>` สำหรับรายการแบบคำจำกัดความ
- `<li>` แทนรายการแต่ละรายการ

### แบบฝึกหัด
1. สร้างตารางแสดงข้อมูลส่วนตัว
2. สร้างรายการเมนูอาหาร


```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ข้อมูลส่วนตัวและเมนูอาหาร</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            background-color: #f9f9f9;
        }
        table {
            width: 50%;
            margin: 20px auto;
            border-collapse: collapse;
            background-color: #ffffff;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        th, td {
            border: 1px solid #ddd;
            text-align: left;
            padding: 8px;
        }
        th {
            background-color: #4CAF50;
            color: white;
        }
        tr:nth-child(even) {
            background-color: #f2f2f2;
        }
        h2 {
            text-align: center;
            color: #333;
        }
    </style>
</head>
<body>
    <h2 style="text-align: center;">ข้อมูลส่วนตัว</h2>
    <table>
        <tr>
            <th>หัวข้อ</th>
            <th>รายละเอียด</th>
        </tr>
        <tr>
            <td>ชื่อ</td>
            <td>นายโกศล เพ็งพิพัฒน์</td>
        </tr>
        <tr>
            <td>อายุ</td>
            <td>19 ปี</td>
        </tr>
        <tr>
            <td>ที่อยู่</td>
            <td>118/7 หมู่ที่ 7 ตำบลสำโรงใต้ อำเภอพระประแดง จังหวัดสมุทรปราการ 10130</td>
        </tr>
        <tr>
            <td>เบอร์โทร</td>
            <td>065-238-6136</td>
        </tr>
        <tr>
            <td>อีเมล</td>
            <td>67030030@kmitl.ac.th</td>
        </tr>
    </table>
    <h2 style="text-align: center;">เมนูอาหาร</h2>
    <table>
        <tr>
            <th>ลำดับ</th>
            <th>ชื่อเมนู</th>
            <th>ประเภท</th>
            <th>ราคา (บาท)</th>
        </tr>
        <tr>
            <td>1</td>
            <td>Pizza Margherita</td>
            <td>อิตาลี</td>
            <td>250</td>
        </tr>
        <tr>
            <td>2</td>
            <td>Sushi Set</td>
            <td>ญี่ปุ่น</td>
            <td>400</td>
        </tr>
        <tr>
            <td>3</td>
            <td>Pad Thai</td>
            <td>ไทย</td>
            <td>80</td>
        </tr>
        <tr>
            <td>4</td>
            <td>Spaghetti Carbonara</td>
            <td>อิตาลี</td>
            <td>180</td>
        </tr>
        <tr>
            <td>5</td>
            <td>Tom Yum Goong</td>
            <td>ไทย</td>
            <td>150</td>
        </tr>
        <tr>
            <td>6</td>
            <td>Ramen</td>
            <td>ญี่ปุ่น</td>
            <td>120</td>
        </tr>
        <tr>
            <td>7</td>
            <td>Tacos</td>
            <td>เม็กซิโก</td>
            <td>100</td>
        </tr>
        <tr>
            <td>8</td>
            <td>Cheeseburger</td>
            <td>อเมริกัน</td>
            <td>150</td>
        </tr>
        <tr>
            <td>9</td>
            <td>Butter Chicken</td>
            <td>อินเดีย</td>
            <td>200</td>
        </tr>
        <tr>
            <td>10</td>
            <td>Crepes</td>
            <td>ฝรั่งเศส</td>
            <td>120</td>
        </tr>
    </table>
</body>
</html> 

```html

```
- ภาพผลลัพธ์:
[วางภาพ screenshot ที่นี่]
![image](https://github.com/user-attachments/assets/679af0d3-d809-46c2-b7cc-ff24257b38f7)


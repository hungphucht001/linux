## - Tìm hiểu về trình soạn thảo văn bản Vi trong Linux
```
shift + 4: di chuyển cuối câu
shift + 6, 0: di chuyển đầu câu
shift + g: di chuyên cuối file văn bản
gg: quay lại đầu file văn bản
w: tiến tới 1 từ
b: quay lại một từ
i: chuyển sang chế độ inster từ chế độ lệnh
Esc: để thoát chế độ Line
:q: thoát
:q!: bắt buộc thoát và không lưu
:wq: thoát và lưu file lại
:w: lưu
:w!: bắt buộc ghi file (Ghi đè)
4 dấu mũi trên: di chuyển lên xuống trái phải
j: di chuyển xuống 1 dòng
k: di chuyển lên 1 dòng
h hoặc Backspace: di chuyển sang trái 1 ký tự
l: di chuyển sang phải 1 ký tự
e: di chuyển con trỏ đến cuối từ hiện tại

```
```
dd: xóa dòng hiện tại
D: xóa dòng còn lại của dòng hiện tại
Nx: xóa n ký tự bắt đầu từ vị trí hiện tại
shift + 8: tìm sự xuất hiện tiếp theo của từ hiện tại.
DND: xóa N dòng
u: hoàn tác
yy: sao chép dòng hiện tại và đặt nó vào bộ nhớ đệm
yNy: sao chép N dòng và đặt vào bộ nhớ đệm
p: dán tại vị trí hiện tại dòng từ bộ nhớ đệm
O: bắt đầu một dòng mới trên dòng hiện tại, chèn văn bản ở đó; dừng lại khi dùng phím Escape.
o: bắt đầu một dòng mới bên dưới dòng hiện tại, chèn văn bản ở đó; dừng lại khi dùng phím Escape.
R: thay thế văn bản bắt đầu với vị trí hiện tại; dừng lại khi dùng phím Escape.

https://kb.pavietnam.vn/huong-dan-su-dung-lenh-vi-vim-tren-linux.html
```

## - Thực thi thành thạo các lệnh cơ bản về file-folder: di chuyển, liệt kê, cho biết thư mục hiện hành….


- Thư mục hiện hành
```
pwd
```


## - Tạo cây thư mục

```
mkdir -p cap1/cap2/cap3 cap1a/cap2a/cap3a
```

## - Tạo file rỗng và file có chứa nội dung

- Tạo file rỗng
```
touch filename.txt
```

- Tạo file có dữ liệu
```
echo "hello" > abc.txt
```

## - Thành thạo các lệnh thêm, xóa, sửa, tìm kiếm, copy, hiển thị nội dung, hiển thị thông tin của file-folder


Xóa file

- Sửa tên thư mục
```
mv cap1 cap3
```
- Hiển thị thông tin thư mục
```
ls -l cap1
```
- Tìm file - folder
```
find . -name a
```
- Hiển thị nội dung file
```
cat abc.txt
```

- Xóa thư mục có dữ liệu
```
rm -rf cap1
```
- Xóa thư mục rỗng
```
rm abc.txt
```
- Di chuyển thư mục
```
mv cap1/a cap2
```

Tạo thư mục
```
mkdir cap1
```
Liệt kê thư mục
```
ls
```


## - Thành thạo các lệnh nén, giải nén, gom, bung file-folder

- Nén file
```
gzip abc.txt
```
- Giải nén file
```
gunzip abc.txt.gz
```
- Nén thư mục
```
tar cvfz cap1.tar.gz cap1
```
- Giải nén thư mục
```
tar xvfz cap1.tar.gz
```
- Gom thư mục
```
tar -cvf abc.tar cap1 cap2
```
- Nén và gom
```
tar -zcvf abc.tar.gz cap1 cap2
```
- bung file
```
tar -xvf abc.tar
```
- Giải nén và bung
```
tar -zxvf abc.tar.gz
```
- Coppy file vào thư mục
```
cp cap1/abc.txt cap2
```
- Coppy thư mục vào thư mục
```
cp -r cap1 cap2
```
- Di chuyển thư mục
```
mv cap1 cap2
``` 

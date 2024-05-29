Git Reset

	⁃	Dùng để di chuyền repo về các commit trước đó, và XOÁ MỌI THAY ĐỔI SAU COMMIT ĐÓ

Bước 1: Tìm đến commit trước

![alt text](../img/img_reset_part1.gif)


Bước 2: Di chuyển repo quay lại bước đó

![alt text](../img/img_reset_part2.gif)


Git Reset tìm Commit trong Log
Bước 1:
	⁃	Tìm điểm muốn quay về, sử dụng log
	⁃	Tiếp đến, reset repo quay trở lại commit cụ thể, sử dụng:
git reset commithash ( commithash là 7 ký tự commit đầu mà đã log)
	⁃	Sau khi reset xong thì lịch sử commit của những commit sau đó sẽ mất

Ví dụ: reset repo về commit 9a9add8

![alt text](<../img/Screenshot 2024-05-29 at 10.58.49.png>)

Sau khi reset và check git log ( Nó đã xoá lịch sử commit của e56 và 524)

![alt text](<../img/Screenshot 2024-05-29 at 10.59.17.png>)

	◦	Việc thay đổi lịch sử của repo có thể nguy hiểm
	◦	Chỉ nên sử dụng trên repo local, tránh thực hiện vào repo remote


Git Undo Reset
	•	Mặc dù các commit không còn hiển thị trong nhật ký nữa nhưng nó vẫn không bị xóa khỏi Git.

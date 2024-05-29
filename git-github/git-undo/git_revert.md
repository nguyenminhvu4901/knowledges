Git Revert

- Là lệnh sử dụng khi muốn lấy commit trước đó và thêm nó làm commit mới, giữ nguyên log

Bước 1: Tìm số commit trước
￼
![alt text](../img/image.png)

Bước 2: Sử dụng nó để tạo 1 commit mới 

![alt text](../img/img_revert_part2.gif)


Các bước làm

B1: 
- Tìm điểm cần quay trở lại, sử dụng log
- Để tránh danh sách log dài, dùng thêm flag —oneline (Show mỗi commit trên mỗi dòng
    - Show ra 7 kí tự đầu tiên của commit hash
    - Sau đó là message của commit đó

Git Revert HEAD
- Để revert commit mới nhất, sử dụng revert AHEAD ( revert commit mới nhất, sau đó commit) 
- Có thể sử dụng flag —no-edit để skip thông báo commit
- Để revert đến các commit gần đây, sử dụng
git revert HEAD~x (x là số, 1 để quay về 1 lần, 2 là quay về 2 lần,…)

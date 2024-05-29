Git Amend

- Thường được sử dụng để sửa đổi commit gần đây nhất
- Nó kết hợp các thay đổi trong staging env với commit mới nhất, và tạo ra 1 commit mới
- Commit mới (Dùng amend) này thay thế hoàn toàn Commit mới nhất

* Chức năng: Chỉnh sửa commit gần nhất (commit mới nhất) thay vì tạo một commit mới.
* Mục đích: Sử dụng khi bạn muốn sửa đổi commit cuối cùng, chẳng hạn như thay đổi thông điệp commit hoặc thêm/xóa/chỉnh sửa các thay đổi trong commit đó.
* Kết quả: Thay thế commit cuối cùng bằng commit mới, có thể thay đổi nội dung hoặc thông điệp của commit đó.

Ví dụ: 
- Tạo 1 commit (commit hash là 07c)

![alt text](<../img/git commit -m Adding plines to reddme.png>)

- Lúc này log đã có commit này
￼
![alt text](<../img/Screenshot 2024-05-29 at 11.14.09.png>)

- Giờ muốn sửa lại thay đổi của commit mới nhất, sử dụng thêm flag —amend
￼
![alt text](<../img/git commit --amend -m Added lines to README.md.png>)

- Sau đó, commit sử dụng amend sẽ thay thế hoàn toàn commit mới nhất (07c -> eaa)
￼
![alt text](<../img/09f4ocd Updated index.html with a new line.png>)

- [ ] Việc thay đổi lịch sử của repo có thể nguy hiểm
- [ ] Chỉ nên sử dụng trên repo local, tránh thực hiện vào repo remote

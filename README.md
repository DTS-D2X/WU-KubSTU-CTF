# WU-KubSTU-CTF
**CapyAgro Crop Rescue**\n
ở bài này ta cần sửa nhiệt độ, độ ẩm phù hợp
<img width="1919" height="971" alt="image" src="https://github.com/user-attachments/assets/42c112d4-825c-4c55-a7bc-d0d44bccce0d" />

<img width="944" height="677" alt="image" src="https://github.com/user-attachments/assets/da0fd0c9-cfb7-492f-97bf-cffa9a86ed28" />
đọc file config thì thấy các endpoint
ta sử dụng OPTIONS kiểm tra các endpoint hỗ trợ method nào
trong quá trình làm mình khá lan man và tóm gọn thì bài này sẽ chỉ cần tập trung vào
/api/sector/{id} và /api/sector/{id}/adjust
<img width="546" height="289" alt="image" src="https://github.com/user-attachments/assets/d5e55d08-7e40-4cae-b91b-84b2f757b207" />
mình tiến hành truyền id vào các endpoint bên trên
<img width="1864" height="386" alt="image" src="https://github.com/user-attachments/assets/7122b013-c940-4647-8046-175138341648" />
ở endpoint /api/sector/{id} mình tiến hành GET để đọc thông tin json
<img width="1878" height="631" alt="image" src="https://github.com/user-attachments/assets/ff89bfc2-3c13-486d-8e05-26bfdbbc451a" />
ở endpoint /api/sector/{id}/adjust mình có thực hiện POST cùng với thông tin json trên với các chỉ số nhiệt độ, độ ẩm được thay đổi và đã được flag
<img width="1882" height="344" alt="image" src="https://github.com/user-attachments/assets/d3667dc0-a371-44fb-85ff-df536956a4cf" />
tất cả các endpoint mình tìm được đều sử dụng OPTIONS để kiểm tra hỗ trợ trước khi thực hành

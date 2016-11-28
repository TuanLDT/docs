
### Tạo ticket
Test: http://123.31.11.105:3003/api/1.0/create_ticket  
Production: http://saleticket.vietid.net/api/1.0/create_ticket

> Method: POST (form-data)  

#### Parameter

Field         | Type | Description |
------------- | -------------|----------|
secretkey  | String | key được cấp|
deal_id  | Int | ID của deal|
order_id  | String ||
customer_name  | String||
customer_phone  | String||
customer_email  | String||
check_in  | String | Thời gian khởi hành/ Thời gian nhận phòng||
check_out  | String | Thời gian trả phòng||
number_adults  | Int | Số người lớn||
number_children  | String | Mô tả về số trẻ em. Ex: 2 tuổi: 1, 4 tuổi: 2||
payment_state  | Int | Trạng thái thanh toán  0: Chưa thanh toán  1: Đã thanh toán  Default value: 0||
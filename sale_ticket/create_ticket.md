
## Tạo ticket
Test: http://123.31.11.105:3003/api/1.0/create_ticket  
Production: http://saleticket.vietid.net/api/1.0/create_ticket

> Method: POST (form-data)  

#### Parameter

Field         | Type | Description |
------------- | -------------|----------|
secretkey(*)  | String | key được cấp|
data(*)  | [object] | Mảng các object|

Object bao gồm các thông tin sau:

key         | Type | Description |
------------- | -------------|----------|
deal_id(*)  | int | id của deal|
order_ids(*)  | [String] | Mảng các order_id|
cs_id(*)  | int | id của customer support|
customer_name  | String||
customer_phone  | String||
customer_email  | String||
check_in  | Number | Thời gian khởi hành/ Thời gian nhận phòng. Dạng milisecond Ex: 1480323665867||
check_out  | Number | Thời gian trả phòng. Dạng milisecond.|
booking_info  | Json | Thông tin booking {quantity_room, room_type}|
number_adults  | Int | Số người lớn||
number_children  | String | Mô tả về số trẻ em. Ex: 2 tuổi: 1, 4 tuổi: 2||
payment_state  | Int | Trạng thái thanh toán  0: Chưa thanh toán  1: Đã thanh toán  Default value: 0||
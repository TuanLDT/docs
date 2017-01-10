
## Tạo ticket
Test: http://123.31.11.105:3003/api/1.0/call_state  
Production: http://saleticket.vietid.net/api/1.0/call_state

> Method: POST (form-data)  

#### Parameter

Field         | Type | Description |
------------- | -------------|----------|
secretkey(*)  | String | key được cấp|
data(*)  | string |Ở dạng JSON string bao gồm các thông tin bên dưới |

data bao gồm các thông tin sau:

key         | Type | Description |
------------- | -------------|----------|
call_id`(*)`  | string | Id cuộc gọi|
phone`(*)`  | [string] | Mảng các order_id|
timestamp`(*)`  | float | Dạng time milisecond|
state`(*)`  | string|Một trong các trạng thái `ringing`, `picking_up`, `stop`  |
cs_ext_phone`(*)`  | String|Số máy lẻ của customer support|

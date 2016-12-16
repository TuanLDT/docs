## Conversation - [SCChannel (client)](http://socketcluster.io/#!/docs/api-scsocket-client)
Sử dụng SCSchannel của socket cluster cho socketGW

```js
    var socket = socketGW.scSocket();
    var conversation_id = 100920;
	var conversation = scSocket.subscribe(100920);
	conversation.watch(function(data) {
	    /*{
        	"data":{
        		"response":{
        			"conversation_id":"100920",
        			"root_message_id":null,
        			"message_id":"126156",
        			"sender_uid":"1",
        			"type":"activity",
        			"content":"p"
        		}
        	}
        }*/
	}); 
	
```
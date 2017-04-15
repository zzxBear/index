#webSocket  简单应用

const http=require('http');

const io=require('socket.io');

let server=http.createServer();

server.listen(666);

let wsServer=io.listen(server);

let wsServer.on('connection',function(){
 sock.emit('tick','a')
})


###html代码

let sock=io.connect('ws://localhost:666');

sock.on('tick',function(n){
 console.log(n);
})

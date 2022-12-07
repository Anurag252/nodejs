readfilesync is blocking call till the contents of file are copied to memory. 
fs.readfileaync and writefileaync are async methods
corect way to read large files is fs.CreateReadStream
apart from byte stream object streams are also possible in node
5 base classes from stream interface
Readable
WriteAble
Duplex
Transform
Passthrough

each of these base class inherit from Eventemitter.

write to a stream till you get a false
read from a stream till you have a null

let readable = new stream.Readble({encoding, highwatermark, objectmode})

writeable stream
let readable = new stream.Writeable({encoding, highwatermark, objectmode})

Duplex has both streams

Transform streams has _read, _write and _transform methods

Passthrough streams is used for testing . They can assert that methods have been called

http.CreateServer is used to create a http server in node
http.get , post for making http calls

proxy and tunneling is very easy with node

proxy :- 

use response.pipe(socket)

tunneling :- 
handle "CONNECT" only and then pipe '

use OPENSSL to create a self signed cert
you can also use free ssl cert from startssl.com

https.CreateServer also takes an arguement as key and cert

url module
Querystring module
headers and cookies maps


6 types of files are there:-

ordinary files
directory
sockets
named pipes
device files
links


to open a named pipe use 
makefifo > namedpipe 
type something
cat > namedpipe 



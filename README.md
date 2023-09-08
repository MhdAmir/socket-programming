## Alur kerja "Client" Socket 
client socket dibuat dengan memanggil fungsi **socket()**, dan dikoneksikan ke sebuah remote address dengan memanggil fungsi **connect()**, dan setelah itu, akhirnya bisa mengambil data dengan memanggil **recv()** 


## Alur kerja "Server" Socket
di dalam "Server", kita butuh untuk membuat sebuah socket dengan memanggil fungsi **socket()**, setlah itu, kita butuh untuk **bind()** socket itu ke sebuah IP dan port kemudian dapat **listen()** untuk koneksi, dan akhirnya kemudian **accept** sebuah koneksi dan **send()** atau **recv()** data ke socket yang lain yang sudah terkoneksi.

```mermaid
Socket Process;
    Socket-->Bind;
    Bind-->Listen;
    Listen-->Accept;
```

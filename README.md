# Test-Shopee
Untuk menyelesaikan task 3 saya tidak dapat menggunakan app test yang diberikan dikarenakan app tersebut tidak bisa di edit sama sekali (Bukti saya lampirkan melalui email).
Oleh karena itu saya mencreate app dan dockerfilenya menggunakan editor lain yang ada di laptop saya.
Untuk menjalankan app tersebut menggunakan docker maka hal yang pertama kali perlu dilakukan yaitu melakukan instalasi docker.
Jika docker sudah diinstall maka jalankan Dockerfile untuk melakukan build imange dengan menjalankan perintah:
docker build -t my-java-app .

Kemudian compile app di dalam docker container:
docker run --rm -v "$PWD":/usr/src/myapp/ -w /usr/src/myapp openjdk:7 app.java

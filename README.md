## 라즈베리 파이 개발 환경

1. 고정 ip 할당
    ```
    $ cd /etc
    $ sudo vi dhcpcd.conf
    ```
    * 다음 코드 추가
    ```
    interface eth0
        static ip_address= **.**.***.***
        static routers= **.**.***.1
        static domain_name_servers=***.***.***.**
        static netmask=255.255.255.0
    ```

1. GPIO library wilingpi
    1. gpio version: 2.44
    1. 라이브러리 다운 : [library download](https://git.drogon.net/?p=wiringPi;a=summary)
    ```
    $ tar xfz wiringPi-96344ff.tar.gz
    $ cd wiringPi-96344ff/
    $ ./build
    ```
    

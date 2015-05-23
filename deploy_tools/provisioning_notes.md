신규 사이트 프로비저닝
=========================

## 필요 패키지

* Nginx
* Python 3
* Git
* pip
* virtualenv

Ubuntu에서 실행 방법 예:

    $ sudo apt-get install nginx git python3 python3-pip

    $ sudo pip3 install virtualenv


## Nginx 가상 호스트 설정

* nginx.tempate.conf 참고
* SITENAME 부분을 도메인 주소로 수정.
* user 부분을 사용할 사용자로 수정.

## Upstart Job

* gunicorn-upstart.template.conf 참고
* SITENAME 부분을 도메인 주소로 수정.
* user 부분을 사용할 사용자로 수정.


## 폴더 구조:
사용자 계정의 홈폴더가 /home/user 라고 가정.

/home/user
- sites
    - SITENAME
        - database
        - source
        - static
        - virtualenv



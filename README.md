# pythonCGI

pythonCGI를 이용해 Dynamic 웹페이지 만들기  

### 1. 이 레파지토리를 다운받고 압축을 푼 다음 cmd에서 해당 폴더로 이동함  
* 폴더 이동 방법은 알고 있다고 가정  
```
cd pythonCGI-master
```

### 2. 아래 명령어로 웹서버를 실행함  
* python이 컴퓨터에 글로벌 옵션으로 설치되어 있어야 함  
```python
$ python -m http.server --cgi
```

### 3. 브라우저를 열고 아래 주소로 접속함  
#### a. form으로 입력을 받아 해당 명령을 실행하는 방법  
* form-pythonCGI 연동 실행 : http://127.0.0.1:8000/  
  - index.html - cgi-bin/cgi_test.py  

#### b. 공통적인 부분을 하나의 index.py파일로 실행하고, 사용자의 반응에 따라 바뀌는 부분은 해당 파일을 불러와서 붙여서 보여주는 방법  
* fileLoad-pythonCGI 실행 : http://127.0.0.1:8000/cgi-bin/index.py  
  - cgi-bin/index.py - cgi-bin/data/HTML  
  - cgi-bin/index.py - cgi-bin/data/CSS  
  - cgi-bin/index.py - cgi-bin/data/JavaSctipt  

### * pythonCGI의 형태로 작성된 웹페이지의 py 파일은 cgi-bin폴더 안에 있을 때만 동작함  

[참조 사이트 링크](https://dzone.com/articles/python-simple-http-server-with-cgi-scripts-enabled)  

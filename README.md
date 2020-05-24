# pythonCGI

pythonCGI를 이용해 Dynamic 웹페이지 만들기  
[참조 사이트 링크](https://dzone.com/articles/python-simple-http-server-with-cgi-scripts-enabled)  

### 이 레파지토리를 다운받고 압축을 푼 다음 해당 폴더로 이동함  
```
cd pythonCGI-master
```

### 아래 명령어로 웹서버를 실행함  
```python
$ python -m http.server --cgi
```

### 브라우저를 열고 아래 주소로 접속함  
form-pythonCGI 연동 실행 : http://127.0.0.1:8000/  
* index.html - cgi-bin/cgi_test.py  

fileLoad-pythonCGI 실행 : http://127.0.0.1:8000/cgi-bin/index.py  
* cgi-bin/index.py - cgi-bin/data/HTML  
* cgi-bin/index.py - cgi-bin/data/CSS  
* cgi-bin/index.py - cgi-bin/data/JavaSctipt  

### pythonCGI의 형태로 작성된 웹페이지의 py 파일은 cgi-bin폴더 안에 있을 때만 동작함  


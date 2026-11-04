## 1단계. 터미널 기본 조작

### ① 현재 위치 확인 (pwd)
```bash
$ pwd
C:/Users/wldn3089811/test2
```

### ② 목록 확인 - 숨김 포함 (ls -a)
```bash
$ ls -a
./  ../  .git/  .gitignore  README.md
```

###  ③ 폴더 이동 (cd)
```bash
$ mkdir practice
$ cd practice
$ pwd
C:/Users/wldn3089811/test2/practice
```

### ④ 빈 파일 생성 (touch)
```bash
$ touch test.txt
$ ls
test.txt
```

### ⑤ 파일 복사 (cp)
```bash
$ cp test.txt copy.txt
$ ls
copy.txt  test.txt
```

### ⑥ 이름 변경 (mv)
```bash
$ mv copy.txt renamed.txt
$ ls
renamed.txt  test.txt
```

### ⑦ 파일 내용 확인 (cat)
```bash
$ echo "hello codyssey" > test.txt
$ cat test.txt
hello codyssey
```

### ⑧ 삭제 (rm)
```bash
$ rm renamed.txt
$ ls
test.txt
```

## 2단계 권한 변경

### ① 권한 확인
```bash
$ ls -l
total 4
drwxr-xr-x 1 wldn3089811 1049089   0 Nov  4 15:51 practice/
-rw-r--r-- 1 wldn3089811 1049089 825 Nov  4 15:54 README.md
```
### ② 권한 변경
```bash
$ chmod 400 README.md
```
### ③ 변경 후 확인 
```bash
$ ls -l
total 4
drwxr-xr-x 1 wldn3089811 1049089   0 Nov  4 15:51 practice/
-r--r--r-- 1 wldn3089811 1049089 825 Nov  4 15:54 README.md
```
### ④ 원상복구 
```bash
$ chmod 644 README.MD
$ ls -l
total 4
drwxr-xr-x 1 wldn3089811 1049089   0 Nov  4 15:51 practice/
-rw-r--r-- 1 wldn3089811 1049089 825 Nov  4 15:54 README.md
```

## 3단계 Docker 설치 점검

### ① 버전 확인
```bash
$ docker --version
Docker version 29.9.2, build a82e528
```

### ② 데몬 동작 확인
```bash
$ docker info
Client:
 Version:    29.9.2
 Context:    desktop-linux
 Server Version: 29.9.2
 Containers: 0 (Running 0 / Paused 0 / Stopped 0)
 Images: 0
 Storage Driver: overlayfs
 Operating System: Docker Desktop
 OSType: linux
 Architecture: x86_64
 CPUs: 24
 Total Memory: 15.25GiB
 Kernel Version: 6.18.54.1-microsoft-standard-WSL2 (WSL2)
 ```

 ## 4단계 Docker 기본 운영
```bash
$ docker images
                                                                  i Info →   U  In Use
IMAGE   ID             DISK USAGE   CONTENT SIZE   EXTRA
$ docker ps -a
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
$ docker stats
- docker stats : 실시간 리소스 모니터링 화면 정상 출력 확인
  (현재 실행 중인 컨테이너가 없어 측정 대상 없음, Ctrl+C로 종료)
```

## 5단계 컨테이너 실행 실습

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
```bash
$ ls -l
total 4
drwxr-xr-x 1 wldn3089811 1049089   0 Nov  4 15:51 practice/
-rw-r--r-- 1 wldn3089811 1049089 825 Nov  4 15:54 README.md
$ chmod 400 README.md
$ ls -l
total 4
drwxr-xr-x 1 wldn3089811 1049089   0 Nov  4 15:51 practice/
-r--r--r-- 1 wldn3089811 1049089 825 Nov  4 15:54 README.md
$ chmod 644 README.MD
$ ls -l
total 4
drwxr-xr-x 1 wldn3089811 1049089   0 Nov  4 15:51 practice/
-rw-r--r-- 1 wldn3089811 1049089 825 Nov  4 15:54 README.md
```

## 3단계 Docker 설치 점검


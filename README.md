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
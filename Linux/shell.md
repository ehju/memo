
## 자주 쓰는 shell 명령어 정리 

### awk

awk  -F, '{ print $1,$2 }' ./file.txt


###  문자열 치환

$ grep "targetfrom" * -rl | xargs sed -i 's/targetfrom/targetto/g'


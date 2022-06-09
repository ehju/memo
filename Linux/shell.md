
## 자주 쓰는 shell 명령어 정리 

### awk

텍스트 입력을 패턴에 따라 처리

awk  -F, '{ print $1,$2 }' ./file.txt


### sed

텍스트 파일을 편집

기본적으로 기존 파일 변경하지 않음, -i 옵션 추가시 변경



### xargs

xargs [OPTIONS] [COMMAND [initial-arguments]]

전달된 문자열을 인수로 사용하는 명령을 실행


###  문자열 치환

$ grep "targetfrom" * -rl | xargs sed -i 's/targetfrom/targetto/g'


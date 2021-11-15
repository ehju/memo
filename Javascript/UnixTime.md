# unix time
 시간을 나타내는 방식.

1970년 1월 1일 00:00:00 협정 세계시(UTC) 부터의 경과 시간을 초로 환산하여 정수로 나타낸 것 (출처 : 위키백과 )


 ### javascript에서 unix timestamp parsing

```javascript
function Unix_timestamp(t){
    const date = new Date(t*1000);
    const year = date.getFullYear();
    const month = "0" + (date.getMonth()+1);
    const day = "0" + date.getDate();
    const hour = "0" + date.getHours();
    const minute = "0" + date.getMinutes();
    const second = "0" + date.getSeconds();
    return year + "/" + month.substr(-2) + "/" + day.substr(-2) + " " + hour.substr(-2) + ":" + minute.substr(-2) + ":" + second.substr(-2);
}
```
=> 결과 

"2021/11/15 12:00:15"


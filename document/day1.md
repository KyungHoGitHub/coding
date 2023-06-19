# Day1 

## golang 
<img width="1070" alt="스크린샷 2023-06-20 오전 1 40 09" src="https://github.com/KyungHoGitHub/coding/assets/119731100/49a5a6dc-0d9d-4147-b5db-de0cc4984952">
프로그래머스의 문제를 참조하였습니다

```
func solution(arr []int, delete_list []int) []int {
 var ret []int //ret 빈 배열을 생성
    for _, item := range arr { //arr 배열의 길이 만큼 순회
        if !Contain(delete_list, item) {
            ret = append(ret, item)
        }
    }
    return ret
}

func Contain(arr []int, value int) bool {
    for _, item := range arr {
        if item == value {
            return true
        }
    }
    return false
}
```

## javaScript
<img width="888" alt="스크린샷 2023-06-20 오전 1 52 53" src="https://github.com/KyungHoGitHub/coding/assets/119731100/28ea0ce3-4bdf-4fbd-bcf7-4d0bbab8da3d">

```
function solution(s) {
    var answer = '';
    for (let i = 0; i < s.length; i++) {
      if (i === 0 || s[i-1] === " ") {
        answer += s[i].toUpperCase();
      } else {
        answer += s[i].toLowerCase();
      }
    }
    return answer;
}
```

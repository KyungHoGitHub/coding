# Day1 

## golang 
<img width="1070" alt="스크린샷 2023-06-20 오전 1 40 09" src="https://github.com/KyungHoGitHub/coding/assets/119731100/49a5a6dc-0d9d-4147-b5db-de0cc4984952">
프로그래머스의 문제를 참조하였습니다

```
func solution(arr []int, delete_list []int) []int {
 var ret []int //ret 빈 배열을 생성
    for _, item := range arr { //arr 배열의 길이 만큼 순회
        if !Contain(delete_list, item) {  // Contain 함수에 매개변수 delet_list 배열 , item
            ret = append(ret, item)       // ret [] 빈 배열에 조건문에 false경우 값을 append
        }
    }
    return ret
}

func Contain(arr []int, value int) bool { //Contain 포함 함수 생성
    for _, item := range arr {            // 매개변수 arr 길이만큼 순회
        if item == value {                // arr 의 item 과 매개변수 value 값이 같으면 true를 반환
            return true  
        }
    }
    return false
}
```
✏️range

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

---
layout: post
title: "Divide and Conquer"
date: 2022-03-16 15:35:04 +0900
categories: jekyll update
---

# 분할정복 알고리즘

> 정의 : 분할정복 알고리즘은 문제를 나눌 수 없을 때까지 나누어서 각각을 풀면서 다시 합병하여 문제의 답을 얻는 알고리즘이다.

- # 분할정복의 설계
  1. Divide : 원래 문제가 분할하여 비슷한 유형의 더 작은 하위 문제로 분할이 가능할 때 까지 나눈다.
  2. Conquer : 각 하위 문제를 재귀적으로 해결한다. 하위 문제의 규모가 나눌 수 없는 단위가 되면 탈출 조건을 설정하고 해결한다.
  3. Combine : conquer(2번)한 문제들을 통합하여 원래 문제의 답을 얻어 해결한다.

> Divide를 잘 설계하는것이 중요 >> 잘 나누면 그만큼 Conquer단계에서 편해진다.

<br>
<br>
<br>
<br>

# 분할정복의 장단점

- 장점: 코드가 직관적이다 (상위-하위로 직선형이기 때문에)

* 단점: 오버헤드 및 오버플로우가 발생할 수 있다.

<br>
<br>
<br>
<br>

# 합병 정렬

> 하나의 list를 두개로 분할하고 각각 분할된 리스트를 정렬한 후 다시 합치는 것.

<br>
<br>
<br>
<br>

### 합병정렬 with Javascript

- mergeSort(arr) : 나누어 주는 함수
- merge(left,right) : 나누어 준걸 정렬해서 새로운 배열을 만들어 줌

<br>
<br>
<br>
<br>

### mergeSort(arr)

함수의 조건

> list의 length가 1이면 더이상 쪼갤 수 없다, 즉 length>=2 일때까지 계속해서 반으로 쪼갠다.

```
const mergeSort = ()=>{
    if(array.length==1){
        return array;
        // 길이가 1이면 그대로 리턴
    }
    else if(array.length>=2){

    }
}
```

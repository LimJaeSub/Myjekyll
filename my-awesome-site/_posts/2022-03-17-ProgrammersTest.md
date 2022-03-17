---
layout: post
title: "ProgrammersTest"
date: 2022-03-17 16:52:46 +0900
categories: Coding Test
---

# Level 1

#### 완주하지 못한 선수

> 정답코드

```
function solution(participant, completion) {
    // participant : 참가자(배열)
    // completeion : 참가자(배열)
    participant.sort();
    completion.sort();
    for(var i=0;i<participant.length;i++){
        if(participant[i]!=completion[i]){
            return participant[i];
        }
    }
}

```

> 효율성 문제

```
function solution(p,c){
    p.sort();
    c.sort();
    for(var i=0;i<p.length;i++){
        for(var j=0;j<c.length;j++){
            if(p[i]==c[j]){
                p[i]=0;
                c[j]=0;
                break;
            }
        }
    }
    for(var i=0;p.length;i++){
        if(p[i]!==0){
            return p[i];
        }
    }
}
```

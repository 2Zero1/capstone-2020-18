# Feature : 투두리스트의 공부계획을 완료처리한다

As 유저

I 투두리스트에 있는 요소를 완료 처리 하면 오늘 복습 리스트로 옮기길 원한다.

So that 나는 내가 오늘 Todolist에서 완료 했던 계획들을 복습 리스트에서 볼 수 있다.

Scenario : 하나의 공부 계획이 완료된다.

    Given 공부 계획이 주어지고

    When 그것을 완료 처리할때

    then 투두리스트 안에 있는 공부 계획은 지워지고, 복습 리스트에서 볼 수 있다.

Scenario : 등록되지 않은 공부계획을 완료 처리 할때 공부계획을 완료처리 하는것을 실패한다.

    Given 등록되지 않은 공부 계획이 주어지고
    
    When 그것을 완료 처리 처리할때

    then 잘못된 접근이라고 알린다.

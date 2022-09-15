### 피보나치 수열이란?
 
 수학에서 피보나치 수(영어: Fibonacci numbers)는 첫째 및 둘째 항이 1이며 그 뒤의 모든 항은 바로 앞 두 항의 합인 수열이다.

### 피보나치 역사
피사의 레오나르도로 널리 알려진 레오나르도 피보나치가 1202년 토끼의 번식을 언급하면서 이 수에 대하여 연구했다. 하지만, 피보나치가 최초로 연구한 것은 아니고 인도의 수학자가 최초란 기록이 남아있다. 기원전 450년 핑갈라가 쓴 책에서 최초로 이 패턴이 언급되었고 이후 인도의 수학자들이 이 수에 대하여 연구한 흔적들이 발견되었다.

### 피보나치 알고리즘
```shell
unsigned int fibonacci_iter(unsigned int n) {

    if (n <= 1) return n; // n이 1보다 작을 때는 해당 값을 그대로 반환한다.
    else {

        int result = 0;
        int iterA = 0, iterB = 1;

        for (int i = 2; i <= n; i++) {

            result = iterA + iterB;
            iterA = iterB;
            iterB = result;

        } // n항의 값을 구한다.

        return result;

    }

}
```

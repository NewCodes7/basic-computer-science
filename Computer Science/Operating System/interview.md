# 운영체제 면접 질문 & 답변

## 🎁 Tip

- 토글을 열기 전에 **실제 면접처럼 '답변'하는** 연습을 합시다!

- 시간이 부족하다면 **'핵심 키워드'** 위주로 떠올려 봅시다!

- 온전히 답변하지 못한 질문이 있다면, **'관련 자료'를** 살펴봅시다!

## 📚 빈출 질문 리스트

<details>
<summary>메모리 계층에 대해서 설명해주세요.</summary>

### 👨🏻‍💻 **답변**

``` 
메모리 계층은 레지스터, 캐시, 주기억장치, 보조기억장치로 구성되어 있습니다. 
레지스터는 CPU 안에 있는 메모리로 휘발성이며 속도가 가장 빠르고 기억 용량이 가장 낮습니다. 
캐시는 CPU 안에 있는 메모리로 대표적으로 L1, L2 캐시가 있으며 휘발성이고 속도가 빠르며 기억 용량이 낮습니다. 
주기억장치는 RAM을 가리키며 휘발성이며 속도와 기억 용량이 보통입니다.
보조기억장치로는 HDD, SSD를 일컬으며 비휘발성이며 속도가 낮고 기억 용량이 높습니다. 
```

### 🎯 **핵심 키워드**

```
 ‘레지스터, 캐시, 주기억장치(RAM), 보조기억장치(HDD, SSD)’ + ‘휘발성, 속도, 기억 용량’
```

### 📔 **관련 자료**

- [2. 메모리](2.%20메모리.md)

</details>

<details>
<summary>가상메모리는 무엇이며, MMU는 무엇인지 설명해주세요..</summary>

### 👨🏻‍💻 **답변**

``` 
가상메모리는 RAM의 크기를 실제보다 크게 확장하는 기술입니다. 이를 통해 프로세스 전체가 메모리 내에 올라오지 않더라도 실행이 가능하도록 합니다. 이를 통해 더 많은 프로그램이 동시에 실행될 수 있고, 프로그램들 간의 메모리 사용이 효율적으로 관리될 수 있습니다. 
MMU는 CPU와 메모리 사이에 위치하며 가상 주소를 실제 메모리 주소로 변환해주는 장치입니다. 
```

### 🎯 **핵심 키워드**

```
확장, 가상 주소, 실제 주소, 변환
```

### 📔 **관련 자료**

- [2. 메모리](2.%20메모리.md)

</details>

<details>
<summary>프로세스와 스레드 둘의 차이에 대해 설명해주세요.</summary>

### 👨🏻‍💻 **답변**

``` 
프로세스는 메인 메모리(주기억장치)에 적재되어 실행되는 프로그램의 인스턴스를 의미하며, 운영체제로부터 자원을 할당받은 작업의 단위를 의미합니다. 반면, 스레드는 한 프로세스 내의 실행 흐름의 단위를 의미합니다. 

프로세스는 프로세스마다 최소 하나의 스레드를 보유하고 있으며, 각각 별도의 주소공간을 독립적으로 할당받게 됩니다.
반면 스레드는 스택만 공간을 따로 할당받고 나머지 힙, 데이터, 코드 영역에서는 공간과 자원을 공유하며 사용하게 됩니다.
```

### 🎯 **핵심 키워드**

```
단위, 독립, 공유
```

### 📔 **관련 자료**

- [3. 프로세스와 스레드](3.%20프로세스와%20스레드.md)

</details>

<details>
<summary>선점(preemption)과 비선점(non-preemption)이 무엇인지 설명해주세요.</summary>

### 👨🏻‍💻 **답변**

``` 
선점 방식은 현재 사용하고 있는 프로세스를 알고리즘에 의해 중단시키고 다른 프로세스에 CPU 소유권을 할당하는 방식입니다. 반면, 비선점 방식은 프로세스가 스스로 CPU 소유권을 포기하는 방식이며, 강제로 프로세스를 중지하지 않습니다. 그렇기에 현재 실행되고 있는 프로세스의 CPU 사용이 끝날 때까지 기다려야 합니다.
```

### 🎯 **핵심 키워드**

```
소유권, 중단
```

### 📔 **관련 자료**

- [4. CPU 스케줄링 알고리즘](4.%20CPU%20스케줄링%20알고리즘.md)

</details>

<details>
<summary> 웹 브라우저의 캐시의 종류와 각각의 캐시를 간략히 설명해주세요. </summary>

### 👨🏻‍💻 **답변**

```
웹 브라우저의 대표적인 캐시로는 쿠키, 로컬 스토리지, 세션 스토리지가 있습니다.
쿠키는 만료기한이 있는 키-값 저장소이며 4KB까지 데이터를 저장할 수 있고 만료기한을 정할 수 있습니다.
로컬 스토리지는 만료기한이 없는 키-값 저장소이며 최대 10MB까지 저장할 수 있고 도메인 단위로 저장 및 생성됩니다.
마지막으로 세션 스토리지는 만료기한이 없는 키-값 저장소이며 최대 5MB까지 저장할 수 있고 탭 단위로 생성됩니다.
추가로 로컬 스토리지와 세션 스토리지는 클라이언트에서만 수정 가능합니다.
```

### 🎯 **핵심 키워드**

```
쿠키, 로컬 스토리지, 세션 스토리지, 만료기한
```

### 📔 **관련 자료**

- [2. 메모리](2.%20메모리.md)

</details>

<details>
<summary> 페이지와 프레임의 차이를 설명해주세요. </summary>

### 👨🏻‍💻 **답변**

```
페이지는 가상 메모리를 사용하는 최소 크기 단위를 뜻하고 프레임은 실제 메모리를 사용하는 최소 크기 단위를 뜻합니다.
페이지와 프레임 모두 최소 크기 단위라는 점은 같지만, 가상 메모리에서의 단위인지 실제 메모리에서의 단위인지에 차이가 있습니다.
```

### 🎯 **핵심 키워드**

```
가상 메모리, 실제 메모리, 단위
```

### 📔 **관련 자료**

- [2. 메모리](2.%20메모리.md)

</details>

<details>
<summary> 메모리 할당 알고리즘 중 first fit, best fit, worst fit 각각에 대해 설명해주세요. </summary>

### 👨🏻‍💻 **답변**

```
first fit은 최초적합으로도 불리며 위쪽이나 아래쪽부터 시작하여 홀을 찾으면 메모리를 바로 할당하는 알고리즘 입니다.
best fit은 최적적합으로도 불리며 프로세스의 크기 이상인 공간 중 가장 작은 홀부터 메모리를 할당하는 알고리즘 입니다.
마지막으로 worst fit은 최악적합으로도 불리며 프로세스의 크기와 가장 많이 차이가 나는 홀에 메모리를 할당하는 알고리즘 입니다.
```

### 🎯 **핵심 키워드**

```
최초적합, 최적적합, 최악적합
```

### 📔 **관련 자료**

- [2. 메모리](2.%20메모리.md)

</details>

<details>
<summary> 외부 단편화와 내부 단편화에 대해 설명해주세요. </summary>

### 👨🏻‍💻 **답변**

```
외부 단편화는 메모리를 나는 크기보다 프로그램이 커서 들어가지 못하는 공간이 많이 발생하는 현상을 말합니다. 이는 메모리 배치에 따라 발생하는 문제입니다.
반대로 내부 단편화는 메모리를 나눈 크기보다 프로그램이 작아서 내부에 사용 불가능한 공간이 많이 발생하는 현상을 말합니다.
```

### 🎯 **핵심 키워드**

```
메모리, 프로그램 크기
```

### 📔 **관련 자료**

- [2. 메모리](2.%20메모리.md)

</details>

<details>
<summary> 컨텍스트 스위칭이 무엇인지 간략히 설명해주세요. </summary>

### 👨🏻‍💻 **답변**

```
하나의 프로세스가 CPU를 사용 중인 상태에서 다른 프로세스가 CPU를 사용하도록 하기 위해, PCB를 교환하는 과정을 말합니다.
컨텍스트 스위칭이 일어나면 유휴시간 (idle time) 및 캐시미스 등의 비용이 발생하게 됩니다.
```

### 🎯 **핵심 키워드**

```
PCB 교환, 유휴시간, 캐시미스
```

### 📔 **관련 자료**

- [3. 프로세스와 스레드](3.%20프로세스와%20스레드.md)

</details>

<details>
<summary>멀티 스레드의 장단점을 설명해주세요.</summary>

### 👨🏻‍💻 **답변**

``` 
멀티 스레드를 통해 하나의 실행 흐름인 프로세스를 여러 개의 실행 흐름으로 만들 수 있습니다. 스레드는 자원을 공유하기 때문에, 프로세스의 처리 능력 향상과 자원의 소모가 줄어드는 것을 기대할 수 있다는 장점이 있습니다.  
하지만 하나의 스레드에 문제가 생길 경우 다른 스레드에도 영향을 끼쳐 프로세스에 문제가 생길 수 있다는 단점이 있습니다.
```

### 🎯 **핵심 키워드**

```
자원 공유, 프로세스
```

### 📔 **관련 자료**

- [3. 프로세스와 스레드](3.%20프로세스와%20스레드.md)
- [운영체제 기술면접](https://imbf.github.io/interview/2020/11/26/NAVER-Interview-Preparation-1.html)

</details>

<details>

<summary>멀티 스레드와 멀티 프로세스의 차이를 설명해주세요.</summary>

### 👨🏻‍💻 **답변**

``` 
멀티프로세싱은 여러 개의 프로세스를 통해 동시에 두 가지 이상의 일을 수행하는 것을 말합니다.
이를 통해 하나 이상의 일을 병렬로 처리할 수 있으며
특정 프로세스의 메모리, 프로세스 중 일부에 문제가 발생하더라도 다른 프로세스를 이용해 처리할 수 있어 신뢰성이 높다는 강점이 있습니다.

멀티 스레딩은 프로세스 내 작업을 여러 개의 스레드로 처리하는 기법을 말하며,
스레드끼리 서로 자원을 공유하기 때문에 효율성이 높습니다.
하지만 하나의 스레드에 문제가 생기면 프로세스에 영향을 줄 수 있다는 단점이 있습니다.

멀티프로세싱의 경우 프로세스끼리는 자원을 공유하지 않지만,
멀티스레딩의 경우에는 스레드끼리 같은 프로세스의 자원을 공유한다는 차이가 있습니다.
```

### 🎯 **핵심 키워드**

```
병렬 처리, 신뢰성, 효율성, 자원 공유
```

### 📔 **관련 자료**

- [3. 프로세스와 스레드](3.%20프로세스와%20스레드.md)
- [멀티 스레드와 멀티 프로세스](https://inpa.tistory.com/entry/%F0%9F%91%A9%E2%80%8D%F0%9F%92%BB-multi-process-multi-thread)
</details>

<details>
<summary>교착 상태란 무엇이고, 이를 해결하는 방법을 설명해주세요.</summary>

### 👨🏻‍💻 **답변**

``` 
두 개 이상의 프로세스가 서로가 가진 자원을 기다리며 중단된 상태로 데드락 이라고도 합니다.
교착 상태는 상호 배제, 점유와 대기, 비선점, 환형 대기의 4가지 조건을 만족할 때 발생합니다. 
이를 해결하기 위해서는 4가지 방법이 존재합니다. 애초에 자원을 할당할 때 교착 상태의 조건을 만족시키지 않게 함으로써 교착 상태를 방지하는 예방과, 교착상태가 발생할 가능성이 있는 자원 할당은 하지 않는 회피 방식, 그리고 교착상태가 발생 할 수 있도록 놔 두고 교착상태가 발생 할 경우 찾아내어 고치는 탐지 및 회복 방식이 있고, 현대 운영체제는 이러한 교착 상태가 드물게 일어나고 고치는 비용이 더 크다는 점에서 사용자가 직접 작업을 종료하는 방식을 채택했습니다.
```

### 🎯 **핵심 키워드**

```
예방, 회피, 탐지 및 회복, 사용자 종료
```

### 📔 **관련 자료**

- [3. 프로세스와 스레드](3.%20프로세스와%20스레드.md)

</details>

<details>

<summary>페이지 교체 알고리즘 두 가지를 말씀해주세요.</summary>

### 👨🏻‍💻 **답변**

```
페이지 교체 알고리즘에는
메모리에 가장 먼저 적재된 페이지를 교체하는 FIFO와
참조가 가장 오래된 페이지를 교체하는 LRU가 있습니다.
FIFO의 경우는 단순하지만, 프로그램 실행 내내 사용될 페이지는 먼저 적재되었다고 해서 교체되면 안되기 때문에
성능 측면에서 좋지 않다는 문제점이 있습니다.
LRU의 경우는 가장 오래된 페이지라는 것을 파악하기 위해 각 페이지마다 계수기, 스택을 두어야 하는 문제점이 있습니다.
```

### 🎯 **핵심 키워드**

```
메모리, 페이지, 참조
```

### 📔 **관련 자료**

- [2. 메모리](2.%20메모리.md)

</details>

<details>

<summary>PCB에 대해 설명해주세요.</summary>

### 👨🏻‍💻 **답변**

```
PCB는 프로세스 제어 블록이라고도 하며, 운영체제에서 프로세스에 대한 메타데이터를 저장한 데이터를 말합니다.
프로세스가 생성되면 운영체제는 해당 PCB를 생성하는데, 프로세스 스케줄링 상태, 프로세스 ID, 레지스터 값 등으로 이루어져 있습니다.
이는 프로세스의 중요한 정보를 포함하고 있기 때문에 일반 사용자가 접근하지 못하도록 커널 스택의 가장 앞부분에서 관리됩니다.
```

### 🎯 **핵심 키워드**

```
프로세스, 메타데이터, 커널 스택
```

### 📔 **관련 자료**

- [3. 프로세스와 스레드](3.%20프로세스와%20스레드.md)

</details>

<details>

<summary>임계 영역 문제를 해결하기 위한 세 가지 조건을 말씀해주세요.</summary>

### 👨🏻‍💻 **답변**

```
임계 영역을 해결하기 위한 조건으로는
한 프로세스가 임계 영역에 들어갔을 때 다른 프로세스는 들어갈 수 없는 상호 배제와
특정 프로세스가 영원히 임계 영역에 들어가지 못하면 안되는 한정 대기,
그리고 만약 어떠한 프로세스도 임계 영역을 사용하지 않는다면 임계 영역 외부의 어떠한 프로세스도 들어갈 수 있는 융통성이 있습니다.
```

### 🎯 **핵심 키워드**

```
상호 배제, 한정 대기, 융통성
```

### 📔 **관련 자료**

- [3. 프로세스와 스레드](3.%20프로세스와%20스레드.md)

</details>

<details>

<summary>CPU 스케줄링 알고리즘은 무엇인가요? 예시도 알려주세요.
</summary>

### 👨🏻‍💻 **답변**

```
CPU 스케줄링 알고리즘은 프로세스에서 해야 하는 일을 스레드 단위로 배치하는 알고리즘을 의미합니다. 
프로그램이 실행될 때 어떤 프로그램에게 CPU 소유권을 줄 것인지 결정합니다. 
```

### 🎯 **핵심 키워드**

```
배치, 프로세스, 스레드, CPU 소유권
```

### 📔 **관련 자료**

- [4. CPU 스케줄링 알고리즘](4.%20CPU%20스케줄링%20알고리즘.md)

</details>
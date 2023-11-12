# 삽입 정렬(Insertion Srot)

## 요약
### 시간 복잡도 : O(n^2)

<ul>
<li>선택한 요소를 그보다 더 앞쪽의 알맞은 위치에 삽입하는 작업을 반복하는 정렬 알고리즘</li>
<li>정렬되지 않은 데이터가 있을 때 정렬되지 않은 첫 번째 요소를 정렬된 부분의 알맞은 위치에 삽입</li>
<li>정렬이 많이 이루어진 경우 효율적으로 사용 가능</li>
<li>정렬에 안정적이고 단순해서 구현이 쉬우나 시간 복잡도가 비효율적임</li>
</ul>

## 삽입 정렬(Insertion Srot)이란
삽입 정렬이란 선택한 요소를 그보다 더 앞쪽의 알맞은 위치에 삽입하는 작업을 반복하는 정렬 알고리즘이다.
<br>
정렬되지 않은 데이터가 있을 때 정렬되지 않은 첫 번째 요소를 정렬된 부분의 알맞은 위치에 삽입하는 개념이다.
<br>
<br>
<img src="https://user-images.githubusercontent.com/87363461/201469759-47b0b434-e526-475d-a91a-9b4d995608ee.JPG" width="250" height="70">
<br>
<br>
위와 같은 정렬되지 않은 배열이 있다고 가정한다. 삽입 정렬은 2번째 요소부터 선택하여 진행한다.
<br>
이때 4는 6보다 앞쪽에 위치해야 하므로, 6보다 앞쪽인 첫 번째에 삽이하고, 6을 오른쪽으로 민다.
<br>
<br>
<img src="https://user-images.githubusercontent.com/87363461/201469884-64c49c8f-1009-4eb4-956c-853c711af94d.JPG" width="250" height="70">
<br>
<br>
다음에 3번째 요소 1을 선택해 앞쪽에 삽입한다. 그 이후 일련의 과정이 계속 반복된다.
<br>
즉, 아직 정렬되지 않은 부분의 첫 번째 요소를 정렬된 부분의 알맞은 위치에 삽입한다.
<br>
<br>
<img src="https://user-images.githubusercontent.com/87363461/201469947-de401da3-2552-4e72-b35c-3378c5d0bd84.JPG" width="600" height="400">
<br>
<br>
정렬된 구역, 정렬되지 않은 2가지 구역으로 나누고, 정렬되지 않은 요소의 첫 번째부터 정렬된 요소의 구역으로 정렬되는 것을 볼 수 있다.
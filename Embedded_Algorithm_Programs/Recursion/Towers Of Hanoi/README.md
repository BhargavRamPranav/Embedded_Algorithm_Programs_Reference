# 하노이의 탑

### 요약
<ul>
<li>큰 원반이 아래에서 차례로 위치할 수 있고, 최소한의 횟수로 마지막 기둥으로 원반을 옮기는 문제</li>
<li>가장 큰 원반을 제외하고 나머지 원반을 그룹으로 묶어 문제 해결에 접근</li>
<li>그룹은 원반 개수의 N - 1</li>
</ul>

## 하노이의 탑(Towers Of Hanoi)이란
하뇌의 탑은 작은 원반이 위에, 큰 원반이 아래에 위치할 수 있도록 원반을 3개의 기둥 사이에서 옮기는 문제이다.
<br>
모든 원반는 크기가 다르고 처음에는 모든 원반이 이 규칙에 맞게 첫 번째 기둥에 쌓여 있다.
<br>
이 상태에서 모든 원반을 세 번째 기둥으로 최소한의 횟수로 옮기는 문제이며, 원반은 1개씩만, 큰 원반을 작은 원반위에 쌓을 수 없다.
<br>
<br>
<img src="https://user-images.githubusercontent.com/87363461/201454325-e694a37b-5078-4847-bfce-b34841a69a45.JPG" width="600" height="500">
<br>
<br>
문제를 해결하기 위해 가장 큰 원반을 제외하고, 나머지 원반을 그룹으로 묶어 접근해야 한다.
<br>
그리고 총 3단계로 접근하여 문제를 해결한다.
<ol>
<li>그룹을 시작 기둥에서 중간 기둥으로</li>
<li>원반 3을 시작 기둥에서 목표 기둥으로</li>
<li>그룹을 중간 기둥에서 목표 기둥으로</li>
</ol>
<img src="https://user-images.githubusercontent.com/87363461/201457357-a38085ff-7fdf-4803-ab84-93c5aa90fa7b.JPG" width="400" height="400">
<br>
<br>
이 경우로 접근하면 원반 N개일 때도 동일하게 적용할 수 있다. 원반이 N개일 때 가장 큰 원반을 제외, N - 1개를 그룹으로 묶는다.

## 문제 풀이
<ol>
<li>바닥 원반을 제외한 그룹(원반[1] ~ 원반[no - 1])을 시작 기둥에서 중간 기둥으로 옮김</li>
<li>바닥 원반 no를 시작 기둥에서 목표 기둥으로 옮김</li>
<li>바닥 원반을 제외한 그룹(원반[1] ~ 원반[no - 1])을 중간 기둥에서 목표 기둥으로 옮김</li>
</ol>

<img src="https://user-images.githubusercontent.com/87363461/201457580-b807b203-c177-4410-97d8-891ffedf7f4f.JPG" width="600" height="400">
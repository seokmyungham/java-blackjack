# java-blackjack

블랙잭 미션 저장소

## 기능 요구 사항

### 게임

- [x] 딜러와 플레이어 중 카드의 합이 21 또는 21에 가장 가까운 쪽이 승리한다.
- [x]  게임을 시작하면 플레이어는 두 장의 카드를 지급 받는다.
    - [x] 이후 플레이어와 딜러의 카드를 출력한다.
    - [x] 단, 딜러의 카드는 하나만 출력한다.
- [ ] 플레이어는 게임을 시작할 때 원하는 금액을 배팅한다.
- [x] 플레이어는 카드의 숫자 합이 21을 초과하지 않는다면 카드를 원하는 만큼 다시 뽑을 수 있다.
    - [x] 새로 받을 때 마다 해당 플레이어의 카드를 출력한다.
- [x] 플레이어가 카드를 다 받으면 딜러의 카드를 확인한다.
- [x] 딜러의 카드 합이 17 이상이 될 때 까지 카드를 받는다.
- [ ] 플레이어의 게임 결과로부터 수익을 계산한다.
    - [ ] 블랙잭으로 승리 할 경우 배팅 금액의 1.5배를 딜러로부터 받는다.
    - [ ] 무승부인 경우 플레이어는 베팅한 금액을 돌려받는다.
    - [ ] 승리할 경우 베팅 금액만큼 받는다.
    - [ ] 패배할 경우 배팅 금액을 모두 잃는다.
- [ ] 딜러와 플레이어의 카드, 결과와 최종 수익 결과를 출력한다.

### 카드

- [x] 클로버, 스페이드, 하트, 다이아몬드 모양을 가진다.
- [x] 카드는 2부터 10까지의 숫자와 Ace, King, Queen, Jack으로 이루어져 있다.
- [x] King, Queen, Jack은 10으로 계산한다.
- [x] ACE는 1 또는 11로 계산할 수 있다.

### 딜러, 플레이어 공통

- [x] 최소 1글자, 최대 5글자의 이름을 가진다.
- [x] ACE 카드를 가지는 경우, 일단 11로 계산한 뒤, 합이 21을 초과하면 1로 계산한다.
- [x] 현재 가진 카드 숫자의 합을 기준으로 카드를 더 받을 수 있는지 결정한다.
    - [x] 딜러는 숫자의 합이 16 이하이면 카드를 더 받을 수 있다.
    - [x] 플레이어는 숫자의 합이 21 이하이면 카드를 더 받을 수 있다.

### 플레이어

- [x] 플레이어의 이름은 중복될 수 없다.
- [x] 플레이어는 최소 2명부터 최대 8명까지 가능하다.
- [ ] 딜러의 점수를 입력받아 승,무,패를 결정한다.
    - [ ] (블랙잭) 처음 두 장의 카드 합이 21일 경우 블랙잭.
    - [ ] (무승부) 딜러와 플레이어가 동시에 블랙잭인 경우.
    - [ ] (무승부) 플레이어의 점수가 21 이하이고, 딜러와 동점인 경우.
    - [ ] (승리) 플레이어의 점수가 21 이하이고, 딜러의 점수가 21을 초과하는 경우.
    - [ ] (승리) 플레이어와 딜러의 점수가 모두 21 이하이고, 딜러의 점수보다 큰 경우.
    - [ ] (패배) 플레이어의 점수가 21을 초과하면 딜러의 점수와 무관.
    - [ ] (패배) 플레이어와 딜러의 점수가 모두 21 이하이고, 딜러의 점수보다 작은 경우.

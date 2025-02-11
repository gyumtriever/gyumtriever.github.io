---
title: "3D Zombie Survival Horror Project"
categories: BlackWall
excerpt: "stay-still"
---

# 크리처
{: .notice--warning}

## 크리처1
{: .notice--success}

- 크리처가 전투 상태일 때 주변의(플레이어의) 라이트를 2초 간격마다 0.5초씩 작동하지 않게 만듦(암전)

## 크리처2
{: .notice--success}

- 지능이 있는 인간형 좀비, 플레이어를 뒤에서 천천히 다가와 암살하려하고 들키면 도망가 위치를 숨기는 패턴

## 크리처3
{: .notice--success}

- 기본적으로 제압 불가능하며, 신체에 있는 모든 약점 포인트를 파괴해야 제압가능(정점에 약점 객체를 하위객체로)
- (보류 사유 : 난이도 문제)약점 포인트를 모두 파괴하고나면 그로기 상태가 되며 가까이 다가가 근접 마무리 공격을 해야 제압할 수 있음, 마무리를 못하면 일정 시간 뒤 재생됨

## 크리처3
{: .notice--success}

- 빛에 약한 크리처, 플래시 라이트로 스턴 가능(밤에는 그 이상의 저지 불가능으로?)

## 크리처4
{: .notice--success}

- 플레이어를 한번에 즉사시키는 크리처, 크리처도 한번의 타격에 즉사(밤에는 공격할 때 카운터로만 즉사하도록?)

## 크리처5
{: .notice--success}

- 예민한 크리처, 플레이어의 완전 작은 행동에도 반응하며 견제 상태일 때 움직이거나 공격할 경우 빠른 속도로 쫒아옴, 이 때 공격력과 방어력이 높은 편임. 견제 상태가 아닐 때 약점을 공격하면 즉사하는 크리처

## 크리처6
{: .notice--success}

- 일렁이는 반투명 상태의 크리처, 화상을 입혀 실체를 드러내게 할 수 있음

## 크리처7
{: .notice--success}

- 시력이 없는 크리처, 작은 소리에 큰 행동 패턴을 보이며 소리를 내지 않아도 플레이어 쪽을 바라보는 등 공포감을 줌

## 크리처8
{: .notice--success}

- 트랩을 사용하는 크리처, 점액같은 흔적을 남기는 등 플레이어가 상호작용 했을 때 죽을때까지 쫒아오는 크리처

## 크리처9
{: .notice--success}

- 모습이 보이지 않다가 근처에가면 보이거나 일렁이는 등 힌트를 주며 플레이어를 멈추게하는 크리처

## 크리처10
{: .notice--success}

- 불빛에 민감한 크리처, 플레이어의 라이트를 포함한 주변 조명을 깜빡거리게 하다가 작동 불가능하게 만듦, 불빛을 보면 달려들음

## 크리처11
{: .notice--success}

- 주변에 가스를 내뿜는 크리처, 가스는 플레이어에게 데미지를 주고 기침을 유도해 사운드를 유발, 해당 크리처를 죽일 경우 크리처에 가스존이 유지됨

## 크리처12
{: .notice--success}

- 해당 크리처에게 발각될 경우 소리를 질러 소음을 유발하고 플레이어에게 어지러움을 유발하는 카메라 워크가 진행되어 조준을 방해함

# 동물
{: .notice--warning}

- 플레이어 발견 시 소리를 내 놀래키거나 크리처가 반응하게 끔 만들고, 가죽/고기 등의 아이템을 루트하거나, 크리처가 아닌 위험할 수 있는 동물 타입의 적의 컨셉으로 맵 마다 다른 동물 타입이 있음

# 상태이상
{: .notice--warning}

## 감염
{: .notice--success}

- 일정 기간내에 완전히 치료하지 못하면 사망함(변이)
- 완전 치료 아이템이 있으며 기간을 늦춰주는 아이템도 존재

# 시스템
{: .notice--warning}

## 시간
{: .notice--success}

- 낮, 밤이 있으며 낮에 강한 좀비, 밤에 강한 좀비가 있음(밤에만 시력이 보이는 등)

## 날씨
{: .notice--success}

- 날씨 시스템은 플레이어와 괴물 모두에게 영향을 미침
  + 안개 : 플레이어 시야 방해(실외), 시각에 의존하는 괴물의 능력 현저히 떨어짐(실외)
  + 호우 : 플레이어 사운드 방해(실외), 소리에 의존하는 괴물의 지각 반경이 매우 떨어짐(실외)
  + 일식 : 플레이어 시야 매우 방해로 인해 나이트 비전 강제화(실외), 시각에 의존하는 괴물이 무방비가 됨
  + 레드문 : 모든 좀비가 강화되거나 특별한 능력이 생김
  + 황사 : 플레이어 시야 방해(실외), 스테미너 감소 속도 증가(실외)

## 방해 요소
{: .notice--success}

- 맵에 밟거나 지나가면 사운드를 발생시켜 좀비에게 들키게 만드는 장치 존재(유리조각 등)

- 뛰다가 밟으면 넘어지는 프롭 존재(적당한 크기의 돌 등)

## 그리드 인벤토리
{: .notice--success}

- 인벤토리를 그리드 형식으로 만들어 정리하는 재미를 주게 함, 가방(인벤토리) 아이템의 등급에 따라(랜덤적으로) 중간중간 막힌 그리드를 구성해 정리 재미를 더 높임, 장착한 아이템은 E 표시로 두어 인벤토리에 그대로 그리드를 차지함

- 엄청 작은 부피의 아이템은 사용하는 칸 마다 MAX 값을 두어 중복으로 보유할 수 있음

- 수리 같은 시스템을 통해 막힌 그리드를 사용 가능한 그리드로 만들 수 있음

## 바디캠 뷰
{: .notice--success}

- Hand 애니메이션을 바디캠 느낌으로 현실감을 극대화
- 걷거나 뛸 때 카메라 흔들림이 있고 흔들림의 특정 포인트에 맞춰 발소리가 재생
- 총기류 반동의 힘, 근접 무기 공격 방향에 따라 카메라 반동(부메랑)이 있음

## 수면
{: .notice--success}

- 해당 맵에서 숙면을 취할 수 있음, 맵의 몬스터를 모두 제거하지 않을 시 확률적으로 패널티(습격)이 있을 수 있음

## 부상 시스템
{: .notice--success}

- 부상 당했을 시 걷거나 뛰는 모션의 카메라 워크가 다리가 절뚝거리는 등의 연출

## 퍼즐
{: .notice--success}

- 락픽으로 문을 딸 때 간단한 퍼즐이 나오는 등 압박감과 손맛을 느끼게 해주는 장치

## 특수아이템
{: .notice--success}

- 특정 아이템(가스 마스크 등)이 있어야 갈 수 있는 지역이 있음

## 환경 사운드
{: .notice--success}

- 잔잔한 분위기에 몰입감을 높여줄 환경 사운드가 중요

# 레벨(난이도)
{: .notice--warning}

- 게임의 난이도는 기본적으로 도전할 수 있도록 조금 어려운 편(잠입 위주)에 속하고, 그 이상의 난이도는 맵의 난이도에 따라 하이리스크 하이리턴의 형태(시티 A구역, B구역 등)
  + 방문한 곳은 기상이변 등의 이유로 쿨타임을 두기(다른 맵으로 이동할 땐 거리에 따라 패널티가 있음 -> 허기 감소 등)
- 잠입 플레이를 유도하고 전투(난전)는 소모품(탄약)이 매우 모자라 최대한 피하도록 설정
  + 맵 중간중간 앉아들어가 숨는 포인트도 있음
- 시작 시 현재 캐릭터의 특성이나 아이템을 선택할 수 있음(유저가 직접 난이도 조절)
  + 인벤토리 증가/감소, 피격시 즉사, 앉아 이동 시 속도 증가 등 난이도를 자체적으로 조절할 수 있게하거나 잠입 특화/전투 특화로 더 유저가 원하는 방향으로 할 수 있음(유저 편의성도 고려)
  + 다른 생존자의 유품의 컨셉으로 가이드 북을 가지고 시작할 수 있고 적에 대한 정보를 글로만 표현해 유추(추리)할 수 있게 유도(가이드 북은 인벤토리를 차지함)
- 세이브 슬롯을 3개 정도 만들어 1슬롯당 1캐릭터가 차지하는 형태, 죽게되면 바로 슬롯이 초기화됨
- 각 맵(구역) 마다 얻을 수 있는 아이템의 종류가 다름
- (보류)날씨에 따라 실외, 실내에 등장하는 크리처가 다름
- 1일차(게임 초반)에는 상대가 쉬운 크리처만 적게 배치해 파밍을 많이 하게 끔 유도, 일차가 높아질수록 잠입&전략 플레이를 하도록 어려운 크리처도 배치하고 크리처의 수도 점차 많아지도록 설정
- UI는 최소한으로(탄약은 플레이어가 직접 세도록), 장착한 무기와 소모품등의 퀵슬롯UI는 바꿀 때만 등장하고 러프하게 비활성화
  + 낮은 HP는 화면 스크린 UI등으로 표현(흑백, 시야가 늘어지는듯한 연출 등)
- 기본적으로 크리처가 플레이어의 일정범위(5m) 이내 일 경우 천천히 다가오며 공격을 준비하는 등의 모션을 취하고 일정범위(5m) 밖일 경우 거리를 빠르게 좁히는 모션 등을 통해 압박감을 유도
- 크리처 개체 수, 밀집 지역, 일반 크리처와 특수 크리처를 적절히 분배해야 함
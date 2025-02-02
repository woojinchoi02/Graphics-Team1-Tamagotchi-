# Graphics-Team1-Tamagotchi

### 사용법
1. SFML라이브러리를 다운로드합니다.
2. SFML폴더의 bin 안에 있는 파일을 모두 복사한 뒤, C 드라이브 -> Windows -> System32 폴더에 넣어줍니다.
3. visual studio에서 Tamagotchi를 실행시켜 줍니다.
4. 프로젝트 속성 C/C++(일반) 추가 포함 디렉터리에서 SFML폴더의 include 폴더를 선택합니다.
5. 프로젝트 속성 링커(일반) 추가 라이브러리 디렉터리에서 SFML폴더의 lib 폴더를 선택합니다.
6. 프로젝트 속성 링커(입력) 추가 종속성에서 아래의 코드를 추가해 줍니다.
   
                        sfml-main-d.lib
                        sfml-graphics-d.lib
                        sfml-window-d.lib
                        sfml-system-d.lib
                        sfml-audio-d.lib
7. SDL2.dll파일을 프로젝트 X64 Debug파일에 넣어줍니다.
---------
### 프로그램 설명
저희 조는 다마고치 게임을 만들어 보았습니다. 다마고치의 주요 기능을 구현하고 다마고치 속 미니게임도 만들어보았습니다.

--------
#### 프로그램 실행 
프로그램 시작 시 총 3마리의 포켓몬 중 한 마리가 랜덤으로 선택됩니다.

![캡처](https://github.com/woojinchoi02/Graphics-Team1-Tamagotchi/assets/162526228/0bf29758-0517-4627-8581-f850b55a4a38)
![111](https://github.com/woojinchoi02/Graphics-Team1-Tamagotchi/assets/162526228/67457b9a-aa32-43e4-8574-096a12cdf485)
![캡처123](https://github.com/woojinchoi02/Graphics-Team1-Tamagotchi/assets/162526228/cf748d00-0bcb-48a2-8651-1de8aad67064)

시간이 지나거나 놀아주기, 청소 등을 하면 청결도, 배고픔, 행복도, 경험치가 오르고 내려갑니다.

![기본로직](https://github.com/woojinchoi02/Graphics-Team1-Tamagotchi/assets/162526228/927c255a-4751-4309-a3f3-d326c9149b50)

일정 레벨에 도달 시 포켓몬이 진화합니다.

![진화](https://github.com/woojinchoi02/Graphics-Team1-Tamagotchi/assets/162526228/59fa740d-d7dd-400d-b186-de0e87320352)

우측 상단 미니게임 버튼을 통해 두 가지의 미니게임을 즐길 수 있으며 경험치도 획득합니다.

게임1 : 블록깨기게임

![게임1](https://github.com/woojinchoi02/Graphics-Team1-Tamagotchi/assets/162526228/f24d1230-c169-4f7a-89e8-674cf352f4ad)

게임2 : 슈팅게임

![게임2](https://github.com/woojinchoi02/Graphics-Team1-Tamagotchi/assets/162526228/1a83e135-32b4-4238-af54-ae025d67cdeb)


플레이 시 각 버튼을 누를 때 효과음이 나도록 구현했습니다.

https://github.com/woojinchoi02/Graphics-Team1-Tamagotchi/assets/162526228/ace4a2cf-d10b-4fa9-90a4-9007d519829a

------
##### 조원
20210809 김현욱, 20210823 이준서, 20210819 우상범, 20210831 최우진
------
### 소감
20210809 김현욱 : 슈팅게임과 블록깨기를 만들면서 게임 개발의 다양한 측면을 경험할 수 있었습니다. SFML을 이용하여 그래픽 요소를 다루고, 이벤트 처리와 게임 로직을 구현하는 과정에서 프로그래밍 능력이 향상되었습니다. 또한, 게임의 성공과 실패를 판단하고 적절한 리소스를 관리하는 것이 중요함을 배웠습니다. 앞으로 더 많은 기능을 추가하고 개선하여 더욱 흥미로운 게임을 만들고 싶습니다.

20210823 이준서 : 혼자서 하면 오래 걸릴 법한 프로젝트였는데 4명이서 분업해서 로직 구현하는 사람, 매핑하는 사람, 등등 나눠서  해서 시간이 많이 단축되었고, 각자 특화된 분야에 일을 맡아서 어렵지만 그나마 수월하게 수행해냈습니다.  이전에 했던 블록깨기 게임과, 슈팅게임을 클래스로 하여 미니게임을 구현하는 등 게임 내에서도 작은 게임을 만드는 곳에서 오류가 많이 나고 고생을 했습니다. SFML을 이용하여 이미지를 매핑시키고, 완벽하지는 않으나 원하는 방향으로 구현하는 것이 생각보다 크게 어렵지 않았고, 흥미를 느꼈습니다.

20210819 우상범 : 게임 개발은 늘 도전적이지만, SFML을 사용하면서 게임 개발에 대한 흥미와 재미를 느꼈어요. 특히, 다마고치 게임과 미니게임을 만들면서 사용자 경험을 디자인하고 구현하는 과정에서의 즐거움은 무엇과도 비교할 수 없었어요. SFML을 사용하면서 저의 프로그래밍 스킬도 향상되었어요. 그 과정에서 많은 오류와 문제를 마주쳤지만, 그것들을 해결해나가는 과정에서 배우는 것이 많았어요. 또한, SFML을 사용하면서 게임의 그래픽, 사운드, 사용자 입력 처리 등 다양한 측면에서의 개발을 경험할 수 있었는데, 이것이 제가 게임 개발에 대해 더 넓은 시야를 갖게 되게 해주었어요. 색다른 경험있었으며 즐거웠습니다.

20210831 최우진 : 익숙하지 않은 C++와 SFML을 사용하는 것이 이번 과제의 가장 힘들었던 점이었습니다. 많은 자료조사가 있었고, 팀원들과 많은 의사소통을 통해 이를 해결해 나갈 수 있었던 것 같습니다. 이번 과제는 어려웠지만 게임을 만들어 나가는 것에서 재미를 느낄 수 있는 기회가 되었고, 다음에도 이러한 게임을 조금 더 완성도 있게 만들어 출시해 보고 싶다는 생각도 하였습니다. 또한 팀장으로서 팀원을 지휘하면서 정말 많은 것을 배운 것 같습니다. 팀원들 간의 협력과 의사소통이 프로젝트의 효율성과 성공에 큰 영향을 미친다는 것을 알 수 있었고 저에겐 하나도 없는 것 같던 리더십도 조금은 있지 않았나 생각해 보는 계기가 된 것 같습니다. 


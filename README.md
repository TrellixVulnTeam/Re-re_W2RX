# 자연어를 활용한 영상검색 어플리케이션

졸업 작품 결과를 위한 프로젝트를 진행했기 떄문에, 현재로서는 다시 정리하기가 어려워서, 발표자료의 내용을 정리해서 업로드하였습니다.


<br>

## 1. 배경

사람은 글자보다 인상적인 이미지를 잘 기억합니다. 어떤 인상적인 동영상을 봤다면, 우리는 그 동영상의 제목을 기억하지 않고, 그 장면을 더 잘 기억합니다. 다시 찾으려고 할 때, 정확한 제목일 기억하려고 노력할 떄도 있지만, 도저히 기억나지 않으면 장면과 연관있는 단어로 검색을 한 경험이 있을 것입니다. 그래서 저희는 이 문제를 딥러닝을 활용해서 해결해보고자 했습니다.

![배경](/assets/background.png)


<br>


## 2. Deep Learning

지금도 딥러닝은 영상처리와 자연어 처리에 많은 영향을 끼치고 있는데, 당시 저희는 img2txt 모델이 개발되었기 때문에 이를 활용해서 문제를 풀고자 했습니다.

![Deep Learning](/assets/deep_learning.png)


<br>


## 3. 목표

모든 동영상에서 해결하는 건 너무 큰 문제라고 생각되서, YouTube 사용자가 지금까지 봤던 영상을 기준으로 작업을 진행했습니다. YouTube의 영상을 받고, 모든 프레임에 대해 문장을 추출했습니다.

그리고 사용자가 찾고자하는 장면을 입력하면, 추출된 문자열들과 비교해서 가장 유사한 동영상을 출력하도록 했습니다.

![목표](/assets/goal.png)


<br>


## 4. 시스템 구성도

![시스템 구성도](/assets/plan.png)


<br>


## 5. 시연 영상

![시연 영상](/assets/demo.png)

- Image caption 생성 과정: [링크](https://youtu.be/XYXqH3uqZp0)
    1. 사용자의 쿠키를 통해 history 정보 수집
    2. 사용자가 시청한 영상 다운로드 및 프레임 분할
    3. 각 프레임별 caption 생성 후 데이터베이스 저장
- 문장 입력을 통한 영상 검색: [링크](https://youtu.be/gn1H9k9F7PM)
    1. 찾고자하는 장면의 문장 입력
    2. 데이터베이스에 저장된 문자들과 유사도를 비교하여 관련 영상 출력


<br>


## 6. 기대 효과

![기대 효과](/assets/benefit.png)


<br>


## 7. 참고 문헌

![참고 문헌](/assets/references.png)
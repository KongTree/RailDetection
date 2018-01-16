# RailDetection
딥러닝

**개요**

`
매번 철로 위의 상태를 확인 할 수가 없다. 그래서 이러한 상태 확인을 위해 인공지능과 드론을 활용하여 철로 위 상황 확인을 대신하는 것을 만든다.
`

**사용기술**

`
LabelImage, MobileNet, Python
`

**설 명**

`
이미지파일을 학습하기 전 라벨이미지(LabelImage) 오픈 소스를 사용하여 각 이미지 마다 Detect 할 범위를 지정하여 디텍트 좌표를 뽑아내 XML파일에 정리한다.

디텍트 좌표 XML 파일과 학습할 이미지를 같이 사용해 MobileNet으로 학습시킨다.

학습이 완료된 데이터를 가지고 테스트 진행
`

**과정**

`
<추가예정>
`

**결과**

`
테스트를 진행할 때에는 동일한 사진으로 진행하지 않고 새로운 이미지로 테스트, 정확도는 약 98~99%의 정확도를 보여준다.
`

**문제점 및 개선**

`
MobileNet을 사용하지않고 학습을 진행 했을 때에는 GPU버전의 텐서플로우를 사용하지않고 학습을 진행해서 매우 느린 학습속도를 보여줌, MobileNet을 사용하니 어느정도 눈에 띄는 학습 속도를 보여줌.

일일히 학습 시킬 이미지의 디텍트 좌표를 뽑아내야하는 반복적인 작업을 해야함

한국 내에서 드론을 올려 철로 위 사진을 구할 곳이 많지 않음.(중국인 유학생 선배 덕분에 중국의 철로 사진을 구할 수 있었음.)
`

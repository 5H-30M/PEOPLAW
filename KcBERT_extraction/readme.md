## 1. 기술 소개
판례 데이터셋에서 QA모델을 통해 핵심 사실을 추출하는 기술을 구현한다. 여기에서 질의응답모델을 통해 판례의 주요사실을 추출하는 방식으로 진행할 예정이기때문에, KoBERT모델과 KorSQuAD 데이터셋을 활용한다. 핵심 사실을 추출한 후, 피해자의 사례와 유사한 판례를 찾기 위해 유사도 검사를 진행한다. 여기에서는 코사인 유사도, BERT를 사용한다.
<br>
## 2. 실행환경
testing을 위한 실행환경은 구글 colab을 활용하여 기술검증을 진행합니다. 기본적으로 런타임을 GPU로 변경한 후 코드를 차례로 실행하는 방식으로 실행합니다. 
<br>
## 3. 실행방법
![image](https://user-images.githubusercontent.com/66730012/206725986-9cb041a3-5bdc-425c-aabc-ec547ebad6fb.png)
1. 반드시 https://colab.research.google.com/?hl=ko로 들어가서 github에서 파일 불러오기 항목을 누릅니다. 

![image](https://user-images.githubusercontent.com/66730012/206726407-d19280f9-0d83-4a9b-88e1-4215e771474b.png)
2. github링크에 
https://github.com/5H-30M/PEOPLAW.gitKcBERT_extraction/kcbert.ipynb를 복사 붙여넣기 하면 해당 파일을 실행할 수 있습니다. 

3. colab의 런타임을 GPU로 바꾸어주세요.
4. 차례대로 코드를 실행합니다.
5. '예시' 전까지의 코드를 실행한 후,
6. 가장 마지막 부분에 실행코드에 원하는 context와 질문을 입력하고 엔터를 눌러주세요.
###주의사항
Optimizer을 통해 모델을 학습시키는 시간이 조금 오래걸릴 수 있습니다

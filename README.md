
1. baseline :
    - 대회의 규정상 수정이 불가한 파일들을 모아둔 폴더입니다.
    - detect.py, east_dataset.py, loss.py, model.py 가 포함되어 있습니다.
2. train.py
    - Main 실행 파일입니다. WanDB 접속 등 다양한 custom option을 제공하며, 다른 코드의 내용을 적절하게 불러와 사용합니다.
    - 이 파일을 실행하기 위해서는 '../data' 경로에 train dataset이 위치해야 합니다.
3. dataset.py : dataset에 다양한 EDA 기법을 적용시키는 script file 입니다.
4. archive : 이전 기수(6기)에서 1위를 기록했던 팀의 solution입니다.
4. 'train.py'를 실행하기 위해서는 아래의 tree 구조가 필요합니다.


```
📦.GitHub
 ┣ 📂.git
 ┣ 📂.github
 ┣ 📂baseline / ~
 ┣ 📂pths
 ┃ ┗ 📜vgg16_bn-6c64b313.pth
 ┣ 📂tools / ~ : 아직 사용할 필요 없는 내용들입니다.
 ┣ 📂utils / ~
 ┣ 📜.gitignore
 ┣ 📜README.md
 ┣ 📜dataset.py : 전체적인 전처리 과정을 수행하는 파일입니다.
 ┣ 📜deteval.py
 ┣ 📜inference.py : checkpoint를 불러옵니다.
 ┣ 📜metrics.py
 ┣ 📜requirements.txt
 ┣ 📜train.py : main 실행 파일입니다.
 ┗ 📜utils.py
```

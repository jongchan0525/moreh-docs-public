# Get Reference Model Code

(개요)
HAC 환경에서는 간단한 명령어 한줄로 다양한 Reference Model(이하 RM) Code를 얻으실수가 있습니다.

실행 방법은 다음과 같습니다.

```shell
get-reference-model resnet
```

위와 같은 명령어 실행 시 ResNet에 대한 RM Code 설치 파일을 다운로드 받게 되며, 동시에 해당 설치 파일을 실행시켜 실행환경을 세팅해줍니다. 명령어 실행 완료시 모델명에 따른 폴더가 생성이 되며 해당 폴더로 들어가 아래 명령어로 바로 모델을 실행(학습) 시킬 수가 있습니다.

```shell
python train.py
```

어떤 모델 코드들이 제공하는지 궁금하시다면 아래와 같은 명령어로 제공가능한 모델 목록을 보실수가 있습니다.

```shell
get-reference-model -h
```

만일, 모델 설치 파일에 대해서 수정 사항이 필요할경우엔 아래와 같이 `--download-only` 옵션을 추가하여 모델 설치 파일만 다운로드 받으실수도 있습니다. 해당 옵션을 추가하고 실행하면 실행경로에 `install_MODEL_NAME.sh` 파일이 생성됩니다.

```shell
get-reference-model --download-only resnet
```
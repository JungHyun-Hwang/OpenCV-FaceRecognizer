# OpenCV-FaceRecognizer
OpenCV를 이용한 얼굴인식 및 모자이크 처리

다음과 같은 간단한 **얼굴인식 및 모자이크 처리**를 **OpenCV**를 이용하여 만들어봅니다.

<p align="center">
  <img src="https://github.com/devetude/OpenCV-FaceRecognizer/blob/master/images/play.gif?raw=true" width="500"/>
</p>

# 프로젝트를 시작하기 전에...
본 프로젝트는 **Microsoft Visual Studio Community 2013** IDE를 사용하였습니다.<br>
프로젝트의 형태는 **Win64 Console Application**이며 프로젝트 파일을 생성하는 부분의 설명은 생략하겠습니다.<br>
(아래의 내용들은 개개인의 PC의 OpenCV 설치 위치에 따라 상이합니다.)<br>

## 1. OpenCV 프로그래밍을 위해서는 다음과 같은 **라이브러리**가 우선 포함되어야 합니다.<br>
**Linker -> General -> Additional Library Directories**에 **OpenCV lib 디렉토리**를 추가해줍니다.

<p align="center">
  <img src="https://github.com/devetude/OpenCV-FaceRecognizer/blob/master/images/additional_library_directories.png?raw=true" width="500"/>
</p>

## 2. 다음으로 **의존성 추가**가 필요합니다.<br>
**Linker -> Input -> Additional Dependencies**에 **OpenCV 의존성 lib 파일**을 추가해줍니다.

<p align="center">
  <img src="https://github.com/devetude/OpenCV-FaceRecognizer/blob/master/images/additional_depandencies.png?raw=true" width="500"/>
</p>

## 3. 다음으로 **디렉토리 추가**가 필요합니다.<br>
**C/C++ -> General -> Additional Include Directories**에 **OpenCV include 디렉토리**를 추가해줍니다.

<p align="center">
  <img src="https://github.com/devetude/OpenCV-FaceRecognizer/blob/master/images/additional_include_directories.png?raw=true" width="500"/>
</p>

## 4. 본 프로젝트에선 OpenCV 64bit 버젼을 사용했습니다.<br>
따라서, 아래와 같이 **Configure Manager -> Platform -> New -> x64**로 변경해줍니다.

<p align="center">
  <img src="https://github.com/devetude/OpenCV-FaceRecognizer/blob/master/images/configure_manager.png?raw=true" width="500"/>
</p>

## 5. 마지막으로 소스코드의 OpenCV 얼굴인식 패턴 xml 파일의 경로를 설정해줍니다.<br>
```c++
#define FACE_CLASSIFIER_PATH "[OpenCV 설치경로]\\sources\\data\\haarcascades\\haarcascade_frontalface_default.xml"
```

# 라이센스
본 프로젝트는 Apache 2.0 License를 따릅니다. http://www.apache.org/licenses/LICENSE-2.0

# 문의사항
기타 문의사항이 있으실 경우 아래의 **문의 수단**으로 연락해주세요.
> **문의 수단:**
> - 메일 : **devetude@naver.com** 또는 **devetude@gmail.com**
> - github : **https://github.com/devetude/OpenCV-FaceRecognizer/issues**

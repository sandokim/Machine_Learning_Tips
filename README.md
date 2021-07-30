# 꼭 알아야하는 분류성능평가지표

Precision, Recall

[참고사이트](https://sumniya.tistory.com/26)

# 실습 환경설정에 대한 유용한 정보들, 프로그램 용어를 정리합니다
---
### **가상환경(Virtual Environments)이란 자신이 원하는 Python 환경을 구축하기 위해 필요한 모듈만 담아 놓는 바구니라고 생각하면 됩니다.**

즉 Python Virtual Envs처럼 각 가상환경(virtualenv1, 2, 3…)은 독립적으로 관리됩니다. 

**각 모듈은 다른 모듈에 대한 의존성(dependency)이 다르기 때문에 마구잡이로 설치하다보면 이유 모를 충돌이 날 수도 있습니다.**

따라서 각 프로젝트 별로 별개의 가상환경을 만들어놓고 사용하는 것이 정신 건강에 좋습니다.

다시 정리하면 가상환경을 사용하는 이유는, 같은 모듈을 사용한다고 하더라도 다른 버전을 필요로 한다거나, 

Python 프로그램을 실행하기 위한 최소한의 환경을 마련하고자 할 때나, 

GitHub 등의 저장소나 네트워크와 연계하고자 할 때 등으로 매우 다양합니다.

Python에서 가상환경을 만드는 방법은 크게 2가지로 virtualenv와 conda를 사용합니다.

conda는 anaconda 환경에서의 명령어입니다.

---

# Data Augmentation
The transformations used by [35, 43, 32] include shifting, rotating and

scaling images, as well as augmenting grey values. One transformation cited in each of the three

papers is the application of a random deformation field. This random deformation field is applied to

the image at the beginning of each training iteration. Hence, in every epoch, the network is training

on a different version of the original data set.

---

### **아나콘다 설치시 유의사항**

아나콘다를 설치하면 아나콘다에 포함된 데이터 분석 라이브러리와 가장 잘 호환되는 버전의 파이썬도 함께 설치됩니다.

파이썬이 중복 설치되면 프로그램 실행 도중 오류가 발생할 수 있으니 기존의 파이썬을 꼭 삭제하고 다음 설치 과정을 진행하세요.

---

### **파이썬 패키지 관리자 - pip**

pip는 파이썬 라이브러리(패키지)를 관리해 주는 관리자 프로그램입니다.

아나콘다를 설치하면 실습에 필요한 대부분의 파이썬 라이브러리가 설치됩니다.

추가로 라이브러리를 더 설치할 경우 pip를 꼭 사용할 줄 알아야 합니다.

---

### **라이브러리(패키지)**

프로그래밍 분야에서는 필요한 기능을 미리 작성하여 모아둔 것을 라이브러리하고 부르는데 파이썬에서는 이를 패키지라고 합니다.

두 용어의 뜻에는 큰 차이가 없습니다.

---

numpy는 CPU에서만 연산이 가능하고 pytorch와 tensorflow는 CPU는 물론 GPU로 데이터를 옮겨서 연산이 가능합니다.

---

numpy.dim은 **dimension을 한 차원 증가시킨다음 concatenate한다는 점**에서 concatenation과 차이가 있습니다.

numpy.dim은 실제로 2개의 numpy array를 각각 reshape한 뒤에 concatenate하는 것과 같은 연산입니다.

# 🎮 게임 수학 예제 따라해보기

C++ 기반의 **게임 수학 교재 예제 코드**를 따라 작성하고 직접 실행해보는 학습용 프로젝트입니다.

</br>원본 링크: https://github.com/onlybooks/gamemath
---

## ✅ 실행 전 필수 설정
> ⚠️ **CMake 버전 문제로 인한 프로젝트 생성 오류 해결**
### 🔍 문제점  
교재에서 제공하는 `.bat` 파일  
- `CMake-VS-16-2019.bat`  
- `CMake-VS-17-2022.bat`  
을 그대로 실행하면 **Visual Studio 프로젝트 파일이 제대로 생성되지 않는 문제**가 발생합니다.  
Why? </br>`CMakeLists.txt`에 명시된 **최소 CMake 버전이 너무 낮기 때문**에 해당 설명대로 실행하면 설명에 있는 Project파일이 제대로 생성되지 않아서
교재내 예제코드들을 볼 수 없습니다.

### 🔧 해결 방법
`cmake_minimum_required(VERSION 3.1)`  → `cmake_minimum_required(VERSION 3.5)` 
</br>로 변경해야 합니다.

### ✏️ 수정 대상 파일 목록 (총 5개)

| 경로 | 설명 |
|------|------|
| `CMakeLists.txt` | 루트 디렉토리의 메인 설정 파일 |
| `Source/Player/CMakeLists.txt` | Player 모듈 |
| `Source/Runtime/Engine/CMakeLists.txt` | Engine 모듈 |
| `Source/Runtime/Math/CMakeLists.txt` | Math 모듈 |
| `Source/Runtime/Renderer/CMakeLists.txt` | Renderer 모듈 |

---

## 📘 학습 목표

- CMake를 사용한 C++ 프로젝트 구성법 학습  
- 수학 이론(벡터, 행렬, 회전 등)의 실습 적용  
- 예제를 통한 수학 시각화 및 개념 이해  

---

## 🛠️ 개발 및 실행 환경

- OS: Windows 10 이상  
- IDE: Visual Studio 2019 또는 2022  
- CMake: **3.5 이상**

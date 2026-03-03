# 📸 Analogue Film Camera App (도담도담)

> **"디지털 사진에 아날로그의 온기를 더하다"** > CameraX와 이미지 처리 알고리즘을 활용한 안드로이드 필름 카메라 애플리케이션

---

## 🛠 Tech Stack
- **Language:** Kotlin
- **Framework:** Android Jetpack (CameraX, Lifecycle)
- **Image Processing:** ColorMatrix, Canvas API
- **Architecture:** MVVM (예정)

---

## ✨ Key Features

### 1. Real-time Analogue Filter
- **Custom ColorMatrix:** 단순한 필터가 아닌, 픽셀 단위의 RGB 값 조정을 통해 정교한 아날로그 색감을 구현했습니다.
- **Granular Texture:** 이미지 오버레이 기술을 활용하여 필름 특유의 노이즈와 질감을 추가했습니다.

### 2. CameraX Integration
- 저지연(Low-latency) 프리뷰와 고화질 사진 캡처를 위해 Google의 최신 CameraX 라이브러리를 적용했습니다.
- 하드웨어 제어(Focus, Exposure)를 통해 실제 수동 카메라와 유사한 사용자 경험을 제공합니다.

---

## 🚀 Troubleshooting & Tech Challenge

### 💡 구글 플레이 스토어 심사 거절 대응
- **Issue:** 알파 배포 심사 중 '사용자 인증 정보 누락'으로 인한 반려(Rejection) 발생.
- **Solution:** 심사위원을 위한 테스트 계정을 제공하고, 앱 진입 시의 예외 처리를 강화하여 성공적으로 **Alpha 단계 배포 및 테스트**를 완료했습니다.

### 💡 이미지 처리 성능 최적화
- 실시간 필터 적용 시 발생하는 프레임 드랍을 해결하기 위해 이미지 분석 알고리즘을 최적화하여 저사양 기기에서도 부드러운 미리보기를 지원합니다.

---

## 📂 Project Structure
- `app/src/main/java/`: 핵심 Kotlin 로직 (Camera 제어 및 필터 알고리즘)
- `app/src/main/res/`: 앱 UI 레이아웃 및 디자인 리소스

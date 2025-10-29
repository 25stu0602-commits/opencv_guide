# opencv_guide
# OpenCV(오픈씨브이) — 간단 요약

고등학생용 깃허브 README용 간단 정리입니다. OpenCV는 컴퓨터 비전(이미지/비디오 처리) 라이브러리로, 실시간 처리와 풍부한 기능을 제공합니다.

---

## 한눈에 보는 핵심

| 영역 | 설명 | 대표 함수/모듈 |
|---|---:|---|
| 입력/출력 | 이미지/영상 읽기·쓰기, 카메라 캡처 | `cv2.imread`, `cv2.imwrite`, `cv2.VideoCapture` |
| 전처리 | 색변환, 필터, 리사이즈, 이진화 등 | `cv2.cvtColor`, `cv2.GaussianBlur`, `cv2.resize`, `cv2.threshold` |
| 특성 검출/매칭 | 에지, 코너, 서술자(ORB, SIFT 등) | `cv2.Canny`, `cv2.goodFeaturesToTrack`, `cv2.ORB_create()` |
| 윤곽선/형태 | 객체의 외곽선 검출과 모멘트 | `cv2.findContours`, `cv2.drawContours`, `cv2.contourArea` |
| 변환 | 기하학적 변환(이동, 회전, 투영) | `cv2.warpAffine`, `cv2.getPerspectiveTransform` |
| 객체 인식 | 얼굴, 사람, 물체 검출(딥러닝 포함) | `cv2.CascadeClassifier`, DNN 모듈 (`cv2.dnn`) |
| 동영상 처리 | 프레임 단위 처리, 비디오 저장 | `cv2.VideoWriter`, 루프에서 프레임 처리 |

---

## 설치

```bash
# Python용 (권장)
pip install opencv-python        # 핵심 패키지
pip install opencv-python-headless  # GUI 없음(서버용)
# 추가(추가 기능): opencv-contrib-python
pip install opencv-contrib-python

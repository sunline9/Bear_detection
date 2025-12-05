🐻 Wild Bear Detection System with YOLOv7

📋 프로젝트 개요 (Project Overview)

이 프로젝트는 YOLOv7 객체 탐지 알고리즘을 활용하여 야생 곰의 출몰을 실시간으로 탐지하는 시스템입니다.
NPU가 탑재된 엣지(Edge) 디바이스에서 구동되도록 설계되어, 통신이 원활하지 않은 산간 지역에서도 독립적인 감시와 경보가 가능합니다.

🚩 개발 배경 (Background)

국외 사례 (일본): 최근 일본에서는 야생 곰의 개체 수 증가와 서식지 파괴로 인해 도심 및 민가 피해가 급증하고 있습니다.

국내 현황 (한국): 대한민국 또한 반달가슴곰 복원 사업으로 개체 수가 늘어남에 따라, 등산객 조우 및 농가 피해 예방을 위한 선제적 관리가 필요해졌습니다.

기술적 필요성: 광대한 산간 지역의 CCTV 영상을 모두 중앙 서버로 전송하는 것은 네트워크 대역폭 및 비용 문제가 발생합니다. 따라서 현장(Edge)에서 즉시 판단할 수 있는 시스템이 필요합니다.

💡 핵심 기능 (Key Features)

실시간 객체 탐지: YOLOv7 모델을 사용하여 높은 정확도와 빠른 속도로 곰(Bear)을 탐지합니다.

Edge Computing 최적화: NPU가 탑재된 소규모 장비(Jetson Nano, Xavier 등)에서도 원활하게 작동하도록 경량화 및 최적화를 수행합니다.

자동 경보 시스템: 곰이 탐지되는 즉시 바운딩 박스(Bounding Box)를 표시하고, 로그를 기록하거나 경고 신호를 보낼 수 있습니다.

🛠️ 기술 스택 (Tech Stack)

Language: Python

Framework: PyTorch

Model: YOLOv7 tiny

Data Source: AI Hub 야생동물 데이터, Custom Crawling Data

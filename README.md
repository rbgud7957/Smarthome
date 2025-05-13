💡 프로젝트 개요
본 프로젝트는 Arduino UNO Board와 다양한 센서, 액추에이터를 활용하여 스마트홈 모형을 제작하고,
주요 기능으로 자동 전등 제어, 인체 감지, 스마트 주차장, 자동 경보 시스템 등을 구현하였습니다.

이 중 저는 코드 총괄과 스마트 주차장 시스템을 담당하여 아래와 같은 기능을 구현했습니다.

🗂 주요 기능 목록
기능 번호	기능명	설명
1	스위치로 실내 전등 제어	버튼을 통해 내부 전등 ON/OFF
2	현관 인체 감지 자동 전등	사람이 감지되면 현관등 자동 점등
3	스마트 주차장 (담당)	차량 감지 및 주차 상태 표시
4	경보 시스템	부동 센서로 침입 감지 시 경고음 발생
5	조도 자동 전등 제어	실외 조도에 따라 전등 자동 점등

🚗 스마트 주차장 시스템 (담당 기능)
✅ 기능 목표
초음파 센서를 이용하여 주차장에 차량 유무를 감지

주차장 진입 시 LED를 통해 주차 가능/불가 상태 표시

LCD를 통해 실시간 주차장 상태 표시

⚙️ 구현 내용
초음파 센서 설치

주차장 입구에 초음파 센서를 배치

일정 거리 이내에 차량이 접근하면 감지

LED 상태 표시

차량이 주차장에 들어오면 적색 LED 점등 (만차)

차량이 빠지면 녹색 LED 점등 (주차 가능)

LCD 실시간 표시

LCD에 "주차 가능", "만차" 상태를 표시

차량 이동에 따른 상태 자동 갱신

📦 구성
<table> <tr> <th>스위치 전등</th> <th>인체 감지 전등</th> </tr> <tr> <td align="center"> <img src="https://github.com/user-attachments/assets/5944980c-5e14-4b11-8f6f-0fa4766debf4" width="300"/><br> 스위치로 ON/OFF가 가능한 전등<br> 사용자가 직접 스위치를 눌러<br> 전등의 점등과 소등을 제어 </td> <td align="center"> <img src="https://github.com/user-attachments/assets/a15eebe3-1769-4e0e-9584-6862a2533c16" width="300"/><br> 인체 감지 시 자동으로 불이 들어오는 전등<br> 사람이 접근하면 PIR 센서를 통해<br> LED 자동 점등 </td> </tr> </table> <table> <tr> <th>스마트 주차장</th> <th>빛 감지 커튼</th> </tr> <tr> <td align="center"> <img src="https://github.com/user-attachments/assets/d5ad2cab-eb33-481a-973e-403accf99621" width="300"/><br> 차량이 들어오면 피에조 스피커로<br> 경고음이 울리고 LED 점등<br> 초음파 센서를 이용하여 차량 감지 </td> <td align="center"> <img src="https://github.com/user-attachments/assets/7414a265-4efe-425f-b6c5-c4c9fdaa7ec4" width="300"/><br> 빛이 들어오면 서보모터를 이용해<br> 자동으로 닫히는 커튼<br> 빛 감지 센서와 서보모터 제어 </td> </tr> </table> <table> <tr> <th>보일러 자동 제어</th> </tr> <tr> <td align="center"> <img src="https://github.com/user-attachments/assets/96877c1a-49c3-4fac-945b-eb84b9e99c6c" width="300"/><br> 실내 온도에 따라 자동으로<br> 보일러를 켜고 끄는 기능<br> 온도 센서를 활용해 스마트한 난방 구현 </td> </tr> </table>

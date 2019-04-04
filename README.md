# DE1-SoC

 <FPGA 기반 재설정 가능한 비휘발성 메모리 에뮬레이터>
   -
 
- Quartus Prime 17.1 사용
- AXI 버스 인터페이스를 기반으로 FPGA와 HPS의 통신을 위한 회로 합성
- VHDL을 사용하여 구현한 FSM(Finite State Machine)으로 데이터 처리
  - read / write : 읽기 및 쓰기 신호로, FPGA의 On-chip RAM에 접근
  - writedata : HPS로부터 받은 데이터
  - waitrequest : 설정한 비휘발성 메모리에 맞는 시간만큼 지연시키기위해 HPS에 요청
  - readdata : On-chip RAM으로부터 읽은 데이터를 HPS로 전송
  


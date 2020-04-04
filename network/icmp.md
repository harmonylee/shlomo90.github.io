<link rel="stylesheet" type="text/css" media="all" href="https://shlomo90.github.io/homepage.css" />

# ICMP

## 목적지 도달 실패 에러

ICMPv4 통신이 관리용으로 금지됨(코드 13)과 ICMPv6 목적지가 관리용으로 금지됨

ICMPv4 와 ICMPv6 에서 목적지 도달 불가 메세지들은 '관리용으로 금지함'이 목적지와의 통신을 방해한다는 것을
표시한다. 이것은 전형적인 방화벽의 소산이다. 방화벽은 라우터에 설정된 운영 정책을 위배하는 트래픽을 의도적으로
버리고, ICMP 오류를 보낸다. 대부분의 경우 트래픽을 버려지는 특별한 정책이 있다는 사실이 광고되지 않아야하므로,
들어오는 패킷을 조용히 버리거나, 혹은 다른 약간 ICMP 오류를 생성해 이런 메시지들의 생성을 무효화 하는 것이 가능하다

### ref.

- TCP/IP Illustrated, Volume 1 
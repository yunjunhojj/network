# 네트워크 계층 (Network Layer)

네트워크 계층은 OSI 7계층 모델의 세 번째 계층으로, 다양한 네트워크 간의 데이터 전송을 담당합니다. 이 계층의 주요 기능과 프로토콜에 대해 자세히 살펴보겠습니다.

## 주요 기능

1. **경로 결정 (Routing)**

   - 네트워크 계층의 가장 중요한 기능 중 하나는 데이터 패킷이 출발지에서 목적지까지 최적의 경로를 찾는 것입니다.
   - 라우터는 경로를 결정하는 장비로, 다양한 라우팅 알고리즘을 사용하여 네트워크 내의 경로를 선택합니다.

2. **패킷 전달 (Packet Forwarding)**

   - 네트워크 계층은 데이터 패킷을 한 네트워크에서 다른 네트워크로 전달합니다.
   - 패킷이 목적지까지 도달할 때까지 여러 라우터를 통해 전달됩니다.

3. **논리적 주소 할당 (Logical Addressing)**

   - 네트워크 계층은 각 장치에 논리적 주소(IP 주소)를 할당하여 네트워크에서의 위치를 지정합니다.
   - IP 주소는 네트워크 식별자와 호스트 식별자로 구성됩니다.

4. **혼잡 제어 (Congestion Control)**
   - 네트워크 내 트래픽이 과도하게 증가할 경우, 네트워크 성능을 유지하기 위해 혼잡 제어 메커니즘을 사용합니다.

## 주요 프로토콜

1. **IP (Internet Protocol)**

   - IP는 네트워크 계층의 주요 프로토콜로, 데이터를 패킷으로 나누어 전송하고 목적지 IP 주소로 전달합니다.
   - IPv4와 IPv6가 주요 버전으로 사용됩니다.

2. **ICMP (Internet Control Message Protocol)**

   - ICMP는 네트워크 진단 및 오류 보고에 사용됩니다.
   - 예를 들어, `ping` 명령어는 ICMP 에코 요청 메시지를 사용하여 네트워크 상태를 확인합니다.

3. **IGMP (Internet Group Management Protocol)**
   - IGMP는 멀티캐스트 그룹 관리를 위해 사용됩니다.
   - 멀티캐스트는 한 송신자가 여러 수신자에게 데이터를 전송할 때 사용됩니다.

## 데이터 전송 과정

1. **패킷 생성**

   - 전송 계층에서 생성된 세그먼트에 IP 헤더를 추가하여 패킷을 생성합니다.

2. **주소 지정**

   - 패킷의 IP 헤더에는 출발지 IP 주소와 목적지 IP 주소가 포함됩니다.

3. **라우팅 및 전달**

   - 라우터는 목적지 IP 주소를 기반으로 최적의 경로를 찾아 패킷을 전달합니다.
   - 각 라우터는 패킷을 다음 라우터로 전달하며, 최종적으로 목적지 네트워크에 도달합니다.

4. **패킷 수신 및 처리**
   - 목적지 네트워크에 도달한 패킷은 해당 호스트의 네트워크 계층에서 수신되고, 상위 계층으로 전달됩니다.

## 네트워크 계층의 장비

1. **라우터 (Router)**

   - 라우터는 네트워크 계층에서 가장 중요한 장비로, 다양한 네트워크 간의 데이터 패킷을 전달하고 경로를 결정합니다.

2. **방화벽 (Firewall)**
   - 방화벽은 네트워크 트래픽을 모니터링하고, 보안 정책에 따라 데이터를 차단하거나 허용하는 장비입니다.

## 결론

네트워크 계층은 데이터 패킷의 전달과 경로 설정을 통해 다양한 네트워크 간의 통신을 가능하게 합니다. IP, ICMP, IGMP 등의 프로토콜을 통해 논리적 주소 할당, 라우팅, 혼잡 제어 등의 기능을 수행합니다. 네트워크 계층은 라우터와 같은 장비를 통해 구현되며, 네트워크의 효율적이고 안전한 운영을 지원합니다.

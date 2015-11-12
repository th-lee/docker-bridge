# docker-bridge
Connect a docker container to a local network


도커 컨테이너(container)와 물리적 서버(docker-engine)를 동일 네트워크 Layer에 구성 함으로 
container와 docker-engine간 port-mapping을 하지 않고 
임의의 client도 container를 하나의 서버로 인식하게 함을 목적으로 합니다.

이 구성은 동일한 배포판을 수십 수백의 다수 client에 배포하여 테스트할때 적절한 구성이 될수 있으며 
변경된 container의 서비스(Web, SSH, DB, etc...)를 commit 전에 테스트 할수 있는 잇점이 있습니다.

# Environment

+ Host OS : Ubunutu 14.04LTS
+ Host IP : 10.0.1.35/32
+ Docker-Engine Ver : 1.9.0
+ Container IP Range (Max #30) : 10.0.1.32/27 (10.0.1.32~10.0.1.63)
+ 

+ container의 gateway는 Host(10.0.1.35/32)가 된다.
+ 




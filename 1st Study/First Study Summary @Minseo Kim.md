# Section 1 Summary @Minseo Kim

Created: 2024년 11월 15일 오전 11:46
Person: Minseo Kim
Section: Section 1, Section 2, Section 3
Tags: Start

### **🧼 Section Summary**

**📍 Section [1]: Getting Started**

- **주요 개념**
    
    트래픽 변화 대응
    
    온프레미스의 한계
    
    클라우드 장점 - 온디멘드 리소스 프로비저닝
    
- **학습 내용 요약**
    
    쇼핑몰 같은 어플은 특정 시간대에만 사람이 많아짐
    
    갑작스러운 증가를 어떻게 감당할 것인지
    
    온프레미스로 가동하면 이와 같은 문제 발생
    
    → 클라우드가 해결책!
    
    온디멘드 리소스 프리비저닝
    
    얼마만큼 돈이 들지 미리 예상할 필요 없음
    
    클라우드는 쓴 만큼 내면 됨
    
    GCP, AZURE, AWS 삼대 Cloud 서비스
    
    [https://cloud.google.com/?hl=ko](https://cloud.google.com/?hl=ko)
    

### **📒 Notes and Key Takeaways**

### **🧼 Section Summary**

**📍 Section 2 : Google Cloud Regions and Zones**

- **주요 개념**

- **학습 내용 요약**
    
    리전과 존
    
    데이터 센터가 여러개여야 세계의 사람들이 활용 가능
    
    두 지역에 동일한 데이터 센터로 해결
    
    세계 전체에 데이터 센터 설치는 어려움
    
    구글은 리전이 20개 있음
    
    리전 안에 존이 존재 
    
    최소 3개
    

### **📒 Notes and Key Takeaways**

### **🧼 Section Summary**

**📍 Section 3 : Google Compute Engine for Associate Cloud Engineer**

- **주요 개념**

- **학습 내용 요약**
    
    컴퓨트 엔진
    
    앱을 빌드할때
    
    클라우드는 가상 서버에서 앱을 배포함
    
    구글 컴퓨트 엔진은 GCP에서 가상 컴퓨터를 프로비전하고 관리하는 서비스
    
    가상 인스턴스 컴퓨터 만들 수 있음
    
    Vm 인스턴스 생성 및 연결
    
    라이프사이클 체크
    
    머신 패밀리안에 다양한 머신 타입
    
    메모리, ssd 등 다양한 타입 선택 가능
    
    CPU, Memory, disk
    
    IMAGE
    
    퍼블릭 이미지 - 구글이 주는
    
    커스텀 이미지 - 내가 만드는
    
    ```bash
    sudo su
    apt update 
    apt install apache2
    ls /var/www/html
    echo "Hello World!"
    echo "Hello World!" > /var/www/html/index.html
    echo $(hostname)
    echo $(hostname -i)
    echo "Hello World from $(hostname)"
    echo "Hello World from $(hostname) $(hostname -i)"
    echo "Hello world from $(hostname) $(hostname -i)" > /var/www/html/index.html
    sudo service apache2 start
    ```
    
    퍼블릭 아이피 - 인터넷 주소
    
    프라이빗 아이피 - 회사 네트워크 내부
    
    vm 인스턴스가 끊기면 외부 아이피는 사라짐
    

### **📒 Notes and Key Takeaways**

https://www.in28minutes.com/google-cloud-updates#exploring-external-ip-addresses
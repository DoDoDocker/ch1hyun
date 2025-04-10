# 섹션 4 - 이미지 레지스트리

---

## 이미지 레지스트리란

<aside>
💡

Docker Hub

도커 이미지를 저장하는 저장소

</aside>

### 제공하는 기능

1. 이미지 공유 (업로드/다운로드)
2. 이미지 검색
3. 이미지 버전 관리
    1. 특정 버전 다운로드 가능
4. 보안
5. 파이프라인

### 이미지 로드 과정

1. docker run
2. 로컬 레지스트리에서 이미지를 찾음
3. 원격 레지스트리에서 이미지를 찾음
4. 로컬 레지스트리로 이미지 다운로드
5. 컨테이너 실행

### 접근 가능 네트워크에 따른 레지스트리 분류

퍼블릭 레지스트리 : 모든 네트워크에서 접근 가능

프라이빗 레지스트리 : 특정 네트워크에서만 접근 가능

‼️ 도커 허브는 퍼블릭 레지스트리이기 때문에 보안상 위험할 수 있다.

![image.png](./section4-images/image.png)

1. 서버에 레지스트리를 설치할 수 있다.
    1. HARBOR
    2. docker
2. 퍼블릭 클라우드 서비스를 사용할 수 있다.
    1. Amazon ECR
    2. Azure Container Registry

## 이미지명 규칙

<aside>
💡

레지스트리주소/프로젝트명/이미지명:이미지태그

레지스트리주소 기본 값 : docker.io

프로젝트명(계정명) 기본 값 : library

이미지태그 기본 값 : latest

</aside>
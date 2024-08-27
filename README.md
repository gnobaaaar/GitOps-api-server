# 테라폼으로 EKS 인프라 구축과 GitOps CICD 파이프라인을 통한 API 서버 배포
## :open_file_folder: 프로젝트 소개
AWS 관리형 쿠버네티스 서비스 EKS를 사용하여
GitOps 기반 파이프라인 API 서비스 배포
</br>
</br>

## :open_file_folder: 구성도
<img width="1058" alt="스크린샷 2022-07-30 오후 6 02 10" src="https://previews.123rf.com/images/aquir/aquir1906/aquir190606651/125693673-%EC%98%88%EC%8B%9C-%EC%8A%A4%ED%83%AC%ED%94%84-%EC%98%88-%EC%82%AC%EA%B0%81%ED%98%95-%EA%B7%B8%EB%9F%B0-%EC%A7%80-%EA%B8%B0%ED%98%B8%EC%9E%85%EB%8B%88%EB%8B%A4-%EC%98%88%EC%8B%9C.jpg">
</br>

## :open_file_folder: 주요 기능
1. IaC
</br>Terraform : AWS의 관리형 쿠버네티스인 EKS를 구축

2. api server
</br>2.1 Python + FastAPI 기반 api server 생성
</br>2.2 api server 도커 컨테이너화

3. GitOps CI/CD
</br>3.1 CI : 컨테이너 빌드 후 도커 컨테이너 ECR 업로드
</br>3.2 CD : argoCD를 통해 명시된 이미지 태그에 해당하는 ECR 이미지로 쿠버네티스 서비스 앱 배포
</br>

## :open_file_folder: 적용 기술
### - Terraform
클라우드 리소스를 일관되고 반복 가능한 방식으로 프로비저닝하며, 인프라 상태를 코드로 관리하고, 변경사항을 자동으로 적용
### - AWS (EKS) &nbsp;
AWS의 관리형 Kubernetes 서비스인 EKS를 사용하여 클라우드에서 확장성과 안정성이 뛰어난 컨테이너화된 애플리케이션을 운영
### - GitOps (GitAction + ArgoCD) &nbsp;
GitHub Actions를 통해 CI/CD 파이프라인을 자동화하고, ArgoCD를 사용하여 Kubernetes 클러스터에 지속적으로 안전하게 배포
### - Python + FastApi &nbsp;
Python은 범용성과 확장성이 뛰어난 프로그래밍 언어이고, FastAPI는 고성능 API를 신속하게 개발
### - Docker and Kubernetes
### - Kustomize
Kustomize를 통해 Kubernetes 매니페스트 파일을 템플릿화 하지 않고도 설정의 변형을 관리
### - AWS CLI
### - Linux
</br>

## :open_file_folder: 결과물
캡처화면
</br>
</br>
</br>


## :open_file_folder: 프로젝트 레포지토리
</br>1. terraform EKS : https://github.com/gnobaaaar/eks-terraform-module
</br>2. GitOps (gitaction + argoCD) : https://github.com/gnobaaaar/GitOps-api-server
</br>3. k8s manifest (Kustomize) : https://github.com/gnobaaaar/k8s-manifest-repo
</br>
</br>
</br>

### Contributors
<table>
  <tr>
    <td align="center"><a href="https://github.com/Song121099"><img src="https://avatars.githubusercontent.com/u/70850937?v=4" width="100px;" alt=""/><br /><sub><b>Song121099</b></sub></a><br/></td>
    <td align="center"><a href="https://github.com/gnobaaaar"><img src="https://avatars.githubusercontent.com/u/65750746?v=4" width="100px;" alt=""/><br /><sub><b>gnobaaar</b></sub></a><br/></td>
  </tr>
  </table>

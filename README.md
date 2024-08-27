# 💻 테라폼으로 EKS 인프라 구축하고 api 서버 GitOps CICD 파이프라인 배포

## :open_file_folder: 구성도
<img width="1058" alt="스크린샷 2022-07-30 오후 6 02 10" src="https://user-images.githubusercontent.com/65750746/181903494-c3bf810b-151f-449f-bf0f-e6346a150449.png">


## :open_file_folder: 주요 기능
1. IaC
</br>Terraform : AWS의 관리형 쿠버네티스인 EKS를 구축

2. api server
</br>2.1 python 기반 api server 생성
</br>2.2 api server 도커 컨테이너화

3. GitOps CICD
</br>3.1 CI : 빌드 후 도커 컨테이너 ECR 배포
</br>3.2 CD : argoCD를 통해 명시된 이미지 태그에 해당하는 컨테이너로 쿠버네티스 배포

## :open_file_folder: 적용 기술
### - Terraform <img width="25" height="25" alt="5" src="https://user-images.githubusercontent.com/65750746/181904360-2c2e2806-57dd-4f73-a1d5-af4d06117ad0.png">
<br>

### - AWS (EKS) &nbsp; <img width="25" height="25" alt="5" src="https://user-images.githubusercontent.com/65750746/181905171-7c4fe95d-230e-42b1-a30b-6d3e95959249.png">

### - GitOps (GitAction + ArgoCD) &nbsp; <img width="100" height="35" alt="15" src="https://user-images.githubusercontent.com/70850937/185784787-7f7d6189-3ee5-4861-9c8a-99b6749aa128.png">

### - Python + FastApi <img width="30" height="30" alt="5" src="https://user-images.githubusercontent.com/70850937/185784932-a68229fb-c4c4-4ce7-a126-f0f81c5e1ce1.png">



## :open_file_folder: 결과물 
- 결과 캡처 화면
<img width="1171" alt="스크린샷 2022-07-30 오후 6 38 00" src="-">


### Contributors
<table>
  <tr>
    <td align="center"><a href="https://github.com/Song121099"><img src="https://avatars.githubusercontent.com/u/70850937?v=4" width="100px;" alt=""/><br /><sub><b>Song121099</b></sub></a><br/></td>
    <td align="center"><a href="https://github.com/gnobaaaar"><img src="https://avatars.githubusercontent.com/u/65750746?v=4" width="100px;" alt=""/><br /><sub><b>gnobaaar</b></sub></a><br/></td>
  </tr>
  </table>

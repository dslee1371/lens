# lens

##Lens 설치 및 인증 설정 안내
 
1. 렌즈를 다운로드 후 설치합니다.
- kubernetes lens
- https://github.com/lensapp/lens/releases/tag/v3.5.1
 
2. aws cli 설치 후 access key와 secret access key 설정 합니다.
```
aws cli
AWS CLI 설치 - AWS Command Line Interface
eks 에서 iam 권한을 받기 위해 설치 합니다. (필수)
```

3. Aws 인증 설정
```
$ aws configure
AWS Access Key ID [None]:
AWS Secret Access Key [None]: 
Default region name [None]: ap-northeast-2
Default output format [None]: json
```

4. 초콜릿 설치 ( 파워쉘 커맨드 사용 안내)
```
- 설치 전 powershell을 관리자 권한으로 실행 후 아래 커맨드를 입력합니다.
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
3-1 aws-iam-authenticator 파워셀으로 
aws-iam-authenticator 설치 - Amazon EKS
```

5. 렌즈 시작
- .kube/config 설정 - copy and paste

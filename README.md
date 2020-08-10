# TEAMATE





## 1. generating crypto-config directory, genesis.block, channel and anchor peer transactions

cd network

./generate.sh

## 2. starting the network, create channel and join 

./start.sh

# -chaincode

## 3. chaincode install, instsantiate and test(invoke, query, invoke)

./cc_tea.sh instantiate v1.0

# -prototype

cd ../prototype

## 4. nodejs module install

npm install

## 5. certification works

node enrollAdmin.js

node registerUser.js

## 6. server start

node server.js

## 7. open web browser and connect to localhost:8080

### prototype 사이트맵 구조

![Untitled Diagram](https://user-images.githubusercontent.com/44858733/89749936-ce8e3600-db04-11ea-9fdb-5edc3ed91bb1.png)

### -web_template

#### 1. teamate/network 로 이동

```powershell
cd network
```

#### 2. ./teardown.sh 실행을 통해 container 제거

```powershell
./teardown.sh
```

#### 3.  ./ start.sh 실행을 통한network 실행

```powershell
./start.sh
```

#### 4. ./cc_tea.sh 실행을 통한 체인코드 실행

```powershell
./cc_tea.sh
```

#### 5.  web_template로 이동후 npm을 이용한 라이브러리 설치

```powershell
cd .. && cd web_template && npm install
```

#### 6. enrollAdmin.js 실행을 통한 admin등록

web_template 폴던 안에 wallet 폴더가 존재하면 삭제후 다음과 같은 명령어 실행

```powershell
node enrollAdmin.js
```

#### 7. resisterUser.js 실해을 통한 User 생성

```powershell
node resisterUser.js
```

#### 8.  서버 실행전 mongodb를 사용하길 원한다면 따라하기

server.js 를 열어서 mongoose connection 부분의 몽고db 주소를 내 몽고db에 connection의 주소를 복사 붙여넣기로 바꿔준다.



#### 9.  web_template 

![Untitled Diagram (2)](https://user-images.githubusercontent.com/44858733/89754031-45332f80-db15-11ea-946f-a1d686370d5d.png)

![ezgif com-video-to-gif](https://user-images.githubusercontent.com/44858733/89754691-d3101a00-db17-11ea-9d54-00dd044ed774.gif)

#### 10. web_template 시나리오 보드

![Untitled Diagram (3)](https://user-images.githubusercontent.com/44858733/89756279-f7bac080-db1c-11ea-91c1-ce00bae02c9d.png)

![Untitled Diagram (1)](https://user-images.githubusercontent.com/44858733/89758731-70bd1680-db23-11ea-8893-2fc634257b1a.png)

#### 11.  web_template UML



![Untitled Diagram (4)](https://user-images.githubusercontent.com/44858733/89758551-0c01bc00-db23-11ea-9c3f-79e3941431b3.png)

#### 12. Architecture 

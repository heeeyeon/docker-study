# 1. 기본 이미지 선택
FROM node:18

# 2. 작업 디렉토리 설정
WORKDIR /app

# 3. 종속성 정보 복사 및 설치 // 개발환경에서는 주로 컨테이너 실행 후 터미널에 접속하여 npm install을 실행
COPY package*.json ./
RUN npm install

# 4. 애플리케이션 소스 복사
COPY . .

# 5. 포트 노출
EXPOSE 3000

# 6. 컨테이너 시작 명령
CMD ["npm", "start"]

# lib

개발하는데 필요한 라이브러리 저장소


styled-components: https://www.styled-components.com/  
open-color: https://yeun.github.io/open-color/  
moment: https://momentjs.com/  
numeral: http://numeraljs.com/  
js-cookie: https://github.com/js-cookie/js-cookie  
lodash: https://lodash.com/  

yarn  
npm  
SQLgate  
channel.io  
jenkins.io  
nodemailer  
icon8  
elastic(엘라스틱)  
구글폰트  

npx  
pm2  
docker  

react-router: https://github.com/ReactTraining/react-router  
redux: [https://github.com/reduxjs/redux/blob/master/README.md, https://deminoth.github.io/redux/]  
redux-saga: https://github.com/redux-saga/redux-saga  


[docker]  
FROM : 베이스 이미지  
RUN : 실행 커맨드 라인  
ENV : 설정할 환경변수  
CMD : 데몬으로 실행할 명령어  
VOLUME : 호스트와 컨테이너의 디렉터리 공유  
COPY : 호스트에서 가져올 디렉터리 또는 파일  
EXPOSE : 노출할 포트 설정  

[pm2 - ecosystem.config.js 설정]  
name : pm2 에서 관리하는 이름입니다.  
script : 앱을 구동할 경로 입니다. 보통 app.js 나 express 로 만드셨다면 bin/www 가 되겠지요  
watch : 파일이 변경되면 자동으로 재시작 하겠다는 의미입니다. 개발시에 유용합니다.  
ignore_watch : 배열안에 있는 리스트는 watch 대상에서 무시하겠다는 의미입니다. 로그파일이나 데이터 폴더등의 경로 혹은 이름이 될것입니다.  
exec_mode : 클러스터 모드로 구동합니다  
instances : 클러스터로 구동될시 몇개까지 구동할것인지 선택합니다.(0 : cpu갯수)  
merge_logs : 클러스터로 구동할시 로그를 한파일에 기록합니다.  
log_date_format : 로그에 출력될 날짜와 시간값의 형식입니다.  
error_file : 에러 파일 위치  
out_file : 기본 출력 로그 위치  

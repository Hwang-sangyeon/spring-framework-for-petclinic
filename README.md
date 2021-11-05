# tomcat-petclinic
tomcat-petclinic

# 소스 컴파일 방법
root@master:/etc# vi /etc/environment
JAVA_HOME="/usr/lib/jvm/java-8-openjdk-amd64"

java -version으로 자바경로가 정상적으로 1.8로 잡혔는지 확인하고 다음 단계로 넘어가자!

$ sudo update-java-alternatives -s /usr/lib/jvm/java-1.8.0-openjdk-amd64
$ sudo update-java-alternatives -s /usr/lib/jvm/java-1.11.0-openjdk-amd64


# 소스 빌드
mvn clean package -Dmaven.test.skip=true -P MySQL

..빌드 후에 target 디렉토리에 petclinic.war 파일이 생성된다.
##

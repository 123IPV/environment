linuxͬʱ��װ64��86λjdk

1������JDKĿ¼
   mkdir /usr/java/x64
   mkdir /usr/java/x86

2���ϴ�JDK��װ��
   /usr/java/x64/jdk-6u45-linux-x64.bin 
   /usr/java/x86/jdk-6u45-linux-i586.bin

3����Ȩִ��
   chmod u+x jdk-6u45-linux-x64.bin 
   chmod u+x jdk-6u45-linux-i586.bin

4����װ
   ./jdk-6u45-linux-x64.bin 
   ./jdk-6u45-linux-i586.bin

5������ϵͳ��������
   vi /etc/profile

   ĩβ���
   export JAVA_HOME=/usr/java/x64/jdk1.6.0_45
   #export JAVA_HOME=/usr/java/x86/jdk1.6.0_45
   export CLASSPATH=.:${JAVA_HOME}/lib:${JAVA_HOME}/jre/lib  
   export PATH=${JAVA_HOME}/bin:$PATH

6������������
   ln -s /usr/java/x64/jdk1.6.0_45/bin/java  /usr/bin/java
   ln -s /usr/java/x64/jdk1.6.0_45/bin/javac  /usr/bin/javac
   ln -s /usr/java/x86/jdk1.6.0_45/bin/java  /usr/bin/java86
   ln -s /usr/java/x86/jdk1.6.0_45/bin/javac  /usr/bin/javac86

7���鿴�汾
   java -version
   java86 -version

# Kibana Install
	
## Kibana Download/Unzip

	wget https://artifacts.elastic.co/downloads/kibana/kibana-6.7.2-linux-x86_64.tar.gz
	tar -zxvf kibana-6.7.2-linux-x86_64.tar.gz

## Kibana Start
  
  	cd kibana-6.7.2-linux-x86_64/config
	vi kibana.yml
	server.host: 0.0.0.0
	
	cd ..
  	bin/kibana &
  
## Kibana Check
  
  	ps -ef | grep kibana
  	netstat -na | grep LISTEN | grep 5601
  	http://localhost:5601

## Kibana Stop
  
  	ps 명령어로 PID 확인.
  	kill -s kill PID	

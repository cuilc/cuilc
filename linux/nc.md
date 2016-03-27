
【nc】  
	$ nc -l -v -w 30 192.168.1.20 1234 -l < conf/zoo_sample.cfg   
Connection from 192.168.1.20 port 1234 [tcp/search-agent] accepted

	$ nc -v -w 2 192.168.1.20 1234 > nc.log

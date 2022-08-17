---
title: Matar serviço do windows
layout: post
---

![Matar Serviço do Windows]({{site.baseurl}}/assets/images/posts_img/matar-servico-windows.jpg)
*Foto de [SHVETS](https://instagram.com/sh.vets) production no Pexels*


É de conhecimento geral como matar/encerrar/finalizar um processo que estiver “travado” no Windows.
Usamos muito o gerenciador de tarefas Ctrl+Shift+Esc ou Ctrl+Alt+del. 
Essa forma resolve boa parte das coisas que ficam congeladas no Windows.
A coisa fica mais complicada quando o programa que está travado é um serviço, daqueles que ficam no services.msc.


sc queryex servicename 


taskkill /f /pid [PID] 

sc queryex Sankhya_Om_WILDFLY_TESTE 

taskkill /f /pid 9999 

 

$ netstat -a -n -o | findstr :8080 

TCP    127.0.0.1:8080         0.0.0.0:0              LISTENING       9332 

$ taskkill.exe /F /pid 9332  

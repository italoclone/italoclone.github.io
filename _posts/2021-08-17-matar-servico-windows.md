---
title: Matar serviço do Windows via terminal
layout: post
---

![Matar Serviço do Windows](/assets/images/posts_img/matar-servico-windows.jpg)
_Foto de [SHVETS](https://instagram.com/sh.vets) production no Pexels_

É de conhecimento geral como matar/encerrar/finalizar um processo que estiver “travado” no Windows.
Usamos muito o gerenciador de tarefas Ctrl+Shift+Esc ou Ctrl+Alt+del.
Essa forma resolve boa parte das coisas que ficam congeladas no Windows.
A coisa fica mais complicada quando o programa que está travado é um serviço, daqueles que ficam no services.msc.

```powershell
sc queryex [servicename]

taskkill /f /pid [PID]
```

Exemplo

```powershell
sc queryex Sankhya_Om_WILDFLY_TESTE

taskkill /f /pid 9999
```

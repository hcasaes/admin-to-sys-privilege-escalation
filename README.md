# admin-to-sys-privilege-escalation
Esta é uma técnica de escalonamento de privilégios muito simples, do administrador para o sistema. Esta é a mesma técnica que o PSExec usa.

1) Verifique todos os processos em busca de token do sistema.<br>
2) Copie o token do sistema.<br>
3) Ajuste o token atual.<br>
4) Inicie o processo como Sistema.<br>
5) Reverter para si mesmo.<br>
_________________________________________
PSExec é uma ferramenta de linha de comando que permite aos usuários executar comandos remotamente em outros computadores. É um utilitário Windows gratuito e de código aberto desenvolvido pela SysInternals, uma empresa de software que foi adquirida pela Microsoft em 2006.

O PSExec pode ser usado para uma variedade de tarefas, incluindo:

Executar scripts remotamente
Executar tarefas administrativas remotamente
Executar diagnósticos remotos
O PSExec é uma ferramenta poderosa que pode ser usada para automatizar tarefas e gerenciar computadores remotamente. No entanto, é importante usá-lo com cautela, pois pode ser usado para fins maliciosos.

Para usar o PSExec, você precisa instalar o utilitário no computador local e no computador remoto. Depois de instalado, você pode usar o seguinte comando para executar um comando remotamente:

psexec \\computername command
Onde:

\\computername é o nome do computador remoto
command é o comando que você deseja executar
Por exemplo, o seguinte comando executará o comando dir no computador remoto chamado server1:

psexec \\server1 dir
O PSExec também pode ser usado para executar comandos com privilégios elevados. Para fazer isso, você pode usar o seguinte comando:

psexec \\computername -s command
Onde:

-s é a opção que especifica que o comando deve ser executado com privilégios elevados
Por exemplo, o seguinte comando executará o comando shutdown /r /t 0 no computador remoto chamado server1 com privilégios elevados:

psexec \\server1 -s shutdown /r /t 0
O PSExec é uma ferramenta útil que pode ser usada para automatizar tarefas e gerenciar computadores remotamente. No entanto, é importante usá-lo com cautela, pois pode ser usado para fins maliciosos.

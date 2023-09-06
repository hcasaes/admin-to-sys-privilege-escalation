# admin-to-sys-privilege-escalation
Esta é uma técnica de escalonamento de privilégios muito simples, do administrador para o sistema. Esta é a mesma técnica que o PSExec usa.

1) Verifique todos os processos em busca de token do sistema.<br>
2) Copie o token do sistema.<br>
3) Ajuste o token atual.<br>
4) Inicie o processo como Sistema.<br>
5) Reverter para si mesmo.<br>

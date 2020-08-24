# backup-mkauth-telegram
Enviar backup do mk-auth no telegram

Altere a linha token e user de acordo com os dados do seu bot

1 - Coloque o arquivo enviaBkp dentro da pasta: /opt/mk-auth/scripts/

2 - Dê permissões de execução: chmod -R 777 /opt/mk-auth/scripts/enviaBkp

3 - Crie uma rotina de execução na crontab: echo "30 06 * * * root bash /opt/mk-auth/scripts/enviaBkp &" >> /etc/crontab
Obs: a rotina a cima está configurada para rodar todos os dias as 06:30 da manhã.

4 - Após executar todos os passos a cima, devemos dar um reload na crontab: /etc/init.d/cron restart && sleep 4 &&  /etc/init.d/cron reload


#######################################################################
# DESENVOLVIDO POR: MATHEUS CARVALHO                                  #
# PROIBIDO A COMERCIALIZAÇÃO SEM AUTORIZAÇÃO PREVIA DO DESENVOLVEDOR. #
# E-MAIL: matheuscarvalho@bsd.com.br WEBSITE: matheuscarvalho.com.br  #
#######################################################################

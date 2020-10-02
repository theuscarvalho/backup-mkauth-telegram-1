# backup-mkauth-telegram
Enviar backup do mk-auth no telegram

Altere a linha token e user de acordo com os dados do seu bot

<br>1 - Coloque o arquivo enviaBkp dentro da pasta:</br>
<p><b>/opt/mk-auth/scripts/</b></p>

<br>2 - Dê permissões de execução: </br>
<p><b>chmod -R 777 /opt/mk-auth/scripts/enviaBkp</b></p>

<br>3 - Crie uma rotina de execução na crontab:</br>
<p><b>echo "30 06 * * * root bash /opt/mk-auth/scripts/enviaBkp &" >> /etc/crontab</b></p>


<br>Obs: a rotina a cima está configurada para rodar todos os dias as 06:30 da manhã.</br>


4 - Após executar todos os passos a cima, devemos dar um reload na crontab: <b>/etc/init.d/cron restart && sleep 4 &&  /etc/init.d/cron reload</b>


#######################################################################

  DESENVOLVIDO POR: MATHEUS CARVALHO                                  
  PROIBIDO A COMERCIALIZAÇÃO SEM AUTORIZAÇÃO PRÉVIA DO DESENVOLVEDOR. 
  E-MAIL: matheuscarvalho@bsd.com.br WEBSITE: matheuscarvalho.com.br  
  
#######################################################################

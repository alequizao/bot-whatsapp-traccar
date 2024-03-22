# bot-whatsapp


Em traccar.xml você deve adicionar:

    <entry key='notificator.types'>web,sms</entry>
    <entry key='notificator.sms.manager.class'>org.traccar.sms.HttpSmsClient</entry>
    <entry key='sms.http.url'>http://localhost:8080/enviar</entry>
    <entry key='sms.http.template'>
      {"destino": "{phone}","mensagem": "{message}"}
    </entry>
    <entry key='status.timeout'>60</entry>
    


Instalação:

git clone https://github.com/alequizao/bot-whatsapp-traccar
cd bot-whatsapp-traccar
npm install --force --save && npm start

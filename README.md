# icons_OneSignal

Se sua aplicação do intel XDK está tendo problemas para receber os ícones das notificações do OneSignal nos dispositivos Android, aqui a solução!

1.	Edite os ícones localizado nas pastas com o ícone do seu app, antes de adicionar o plugin.

2.	Adicione o plugin personalizado para inserir os ícones em sua aplicação!

3.	Abra o seu projeto em Gerenciador de plugin importe plugin e selecione a pasta com os seus ícones modificados!

4.	Feito isso aguarde o carregamento, e faça a Build da sua aplicação! Depois disso ele irá pegar os ícones automaticamente! 

5.	Caso não pegue automaticamente os ícones você pode chama-los através do resurso Drawable: ic_stat_onesignal_default 

Para mais informações sobre como personalizar o seu plugin:
https://documentation.onesignal.com/docs/customize-notification-icons


Você pode adicionar ícones customizados com Drawable!
No arquivo plugin.xml, você pode adicionar as resource necessárias!

 resource-file src="drawable-hdpi/ic_stat_onesignal_default.png" target="res/drawable-hdpi/ic_stat_onesignal_default.png"
    
    
# Crie novos plugins
   
  Você pode criar novos plugins para mover arquivos para dentro da pasta do android utilizando esse exemplo!

  
  
<plugin xmlns="http://apache.org/cordova/ns/plugins/1.0" id="icones-onesignal-plugin" version="1.0.0"> 

    <name>Adding icones to OneSignal push notification</name> 
    <description>Adicione seus icones OneSignal - By Victor Marques</description> 
    <license>MIT</license> 

    <engines> 
        <engine name="cordova" version=">=3.0.0" /> 
    </engines>  

    <!-- android --> 
    <platform name="android">

        <resource-file src="drawable-hdpi/ic_stat_onesignal_default.png" target="res/drawable-hdpi/ic_stat_onesignal_default.png" />
        <resource-file src="drawable-xhdpi/ic_stat_onesignal_default.png" target="res/drawable-xhdpi/ic_stat_onesignal_default.png" />
        <resource-file src="drawable-xxhdpi/ic_stat_onesignal_default.png" target="res/drawable-xxhdpi/ic_stat_onesignal_default.png" />
        <resource-file src="drawable-xxxhdpi/ic_stat_onesignal_default.png" target="res/drawable-xxxhdpi/ic_stat_onesignal_default.png" />
    
    </platform>  
    
</plugin>
  
  
  Ele é muito util para mover arquivos que você não consegue para a raiz do seu projeto, com isso você consegue mover qualquer arquivo para dentro dos diretorios que o ItelXDK não permite!
  
  Acesso finalmente para a famosa pasta RES! :D, você pode customisar os icones do plugin Splashscreen dentre outros!
  
  https://cordova.apache.org/docs/en/latest/reference/cordova-plugin-splashscreen/index.html
  
  
  

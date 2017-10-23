# ProxyBot
The proxy just got smarter  
Price: 0.015 BTC  
<br />
# Join the telegram group
If you have questions after reading the readme
### Main Channel
https://t.me/joinchat/FWYlMkKK-mkrSuj836ehug

|Channel Language   | Channel link                                  |
|-------------------|-----------------------------------------------|
|German Channel     | https://t.me/joinchat/FDBA_g1yD6Iw-k46ysvYzA  |
|Potuguese Channel  | https://t.me/joinchat/EzzWHAyih4JoEMk0XBiezA  |
|Russian Channel    | https://t.me/joinchat/DreUUw-n-aGoi2LunoJTFA  |



# Check out the wiki
https://github.com/taniman/proxy-bot/wiki/ProxyBot  

# How to run
Download the latest released jar file  
https://github.com/taniman/proxy-bot/releases  

1. Make sure you have java 8 installed on your system
2. Unzip proxybot.zip file  
3. Fill your apiKeys and secrets in application.properties  
4. set server.botMode = true in application.properties
5. Open a terminal or command prompt and type  
6. java -jar ProxyBot.jar -XX:+UseConcMarkSweepGC -Xmx256m -Xms256m  
   * On OSX or some linux versions you might need to sudo su and then run the java -jar command.  
7. If you did everything correctly the application will start without giving you any error messages  

### On windows
Open a web browser and go to  
http://localhost:8081/checkSetup/

### On a Linux VPS
curl http://localhost:8081/checkSetupLinux/  

All rows should say 'Looking good!'  
If this is not the case, than you have an error in your application.properties  


# Running in the background
Use the provided pm2 json file.<br />
If you have pm2 installed just use this command.<br />
pm2 start pm2-ProxyBot.json <br />
pm2 save <br />
This will make sure that pm2 will automatically start the proxy when pm2 reloads. <br />
<br />
To see the proxy log you could do. <br />
pm2 log 'id' <-- this is the id pm2 gave your proxy

# Setup telegram so the proxy can send you telegram messages
1. Talk to @BotFather   
1.1. NOT to be confused with TheBotFather channel!!!  
1.2 Once there type "/newbot" to create a bot. Answer the questions by typing answers and pressing enter.  

2. Start a chat to your bot's name (for ex. @MyProxyBot) and press start button

3. Start another chat with https://telegram.me/get_id_bot This bot will reveal your Chat ID

4. Edit application.properties and set
    - telegram.botToken = "your bot token"
    - telegram.chatId = "your chat id"
    - restart the bot

5. Go to http://localhost:8081/settings/telegramTestMessage to test your telegram setup. You will receive a message if the setup is correct.

# Authorized resellers on telegram
  - @Elroy (DEV)
  - @Anderson_drsub (Portuguese)
  - @Moondust2010 (German)
  - @AkaDeCaoS (Spanish)
  - @T1M3C (Russian)

# Warning
Please use the proxy on a VPS or machine that you do not use normally. <br />
Once you change the host file the poloniex.com website will not work properly anymore. <br />
<br />


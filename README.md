![Akatsuki](https://telegra.ph/file/66c17e679a90c1caf555b.jpg)
# Pain Robot 
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/6141417ceaf84545bab6bd671503df51)](https://app.codacy.com/gh/TeamNexusTG/PainAkatsukiRobot?utm_source=github.com&utm_medium=referral&utm_content=TeamNexusTG/PainRobot&utm_campaign=Badge_Grade_Settings)  [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/TeamNexusTG/PainRobot/graphs/commit-activity) [![GPLv3 license](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://perso.crans.org/besson/LICENSE.html) [![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com) [![Updates channel!](https://img.shields.io/badge/Join%20Channel-!-red)](https://t.me/PainRobotUpdates)


A modular Telegram Python bot running on python3 with a sqlalchemy database and an entirely themed persona to make Pain suitable for Anime and Manga group chats. 

Can be found on telegram as [PainRobot](https://t.me/PainAkatsukiRobot).

The Support group can be reached out to at [Akatsuki Organization](https://t.me/PainRobotSupport), where you can ask for help about [PainRobot](https://t.me/PainAkatsukiRobot), discover/request new features, report bugs, and stay in the loop whenever a new update is available. 

News channel as at [PainRobot Updates](https://t.me/PainRobotUpdates) 

## How to setup/deploy.

### Read these notes carefully before proceeding 
 - Edit any mentions of @PainRobotSupport to your own support chat
 - Your code must be open source and a link to your fork's repository must be there in the start reply of the bot [See this](https://github.com/AnimeKaizoku/SaitamaRobot/blob/shiken/SaitamaRobot/__main__.py#L25)
 - Lastly, if you are found to run this repo without the code being open sourced or the repository link not mentioned in the bot, we will push a gban for you in our network because of being in violation of the license, you are free to be a dick and not respect the open source code (we do not mind) but we will not be having you around our chats
 - This repo does not come with technical support, so DO NOT come to us asking help about deploy/console errors

<details>
  <summary> Steps to deploy on Railway! </summary>

```
Fill in all the details, Deploy!
Now send the bot /start, If it doesn't respond go to https://dashboard.heroku.com/apps/(app-name)/settings and remove webhook and port.
```

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template?template=https%3A%2F%2Fgithub.com%2FPAINBOI2008%2FPainRobot&plugins=postgresql&envs=TOKEN%2CAPI_ID%2CAPI_HASH%2CSQLALCHEMY_DATABASE_URI%2COWNER_ID%2COWNER_USERNAME%2CSUPPORT_CHAT%2CEVENT_LOGS%2CJOIN_LOGGER%2CCASH_API_KEY%2CTIME_API_KEY%2CDEV_USERS%2Csw_api%2CSTRICT_GBAN%2CDRAGONS%2CDEMONS%2CTIGERS%2CWOLVES%2CNo_LOAD%2CBL_CHATS%2CALLOW_EXCL%2CENV%2CDONATION_LINK%2CDEL_CMDS%2CBAN_STICKER%2CWALL_API%2CREM_BG_API_KEY&optionalEnvs=SQLALCHEMY_DATABASE_URI%2CEVENT_LOGS%2CJOIN_LOGGER%2CCASH_API_KEY%2CTIME_API_KEY%2CDEV_USERS%2Csw_api%2CDRAGONS%2CDEMONS%2CTIGERS%2CWOLVES%2CNo_LOAD%2CBL_CHATS%2CALLOW_EXCL%2CDONATION_LINK%2CWALL_API%2CREM_BG_API_KEY&TOKENDesc=Your+bot+token.+Get+one+from+https%3A%2F%2Ft.me%2FBotFather+.&API_IDDesc=Get+API_ID+from+my.telegram.org%2C+used+for+telethon+based+modules.&API_HASHDesc=Get+API_HASH+from+my.telegram.org%2C+used+for+telethon+based+modules.+&SQLALCHEMY_DATABASE_URIDesc=Your+postgres+sql+db.+Don%27t+add+this+ENV+if+you+dont+have+one.&OWNER_IDDesc=Owner%27s+User+ID+as+an+integer.++Used+by+the+bot+to+identify+the+owner.+&OWNER_USERNAMEDesc=Your+username+without+the+%27%40%27&SUPPORT_CHATDesc=Your+bot%27s+support+chat+username+without+the+%27%40%27&EVENT_LOGSDesc=Event+logs+channel+to+note+down+important+bot+level+events.+Let+it+be+%27123456798%27+if+you+don%27t+have+one.&JOIN_LOGGERDesc=A+channel+where+bot+will+print+who+added+it+to+what+group%2C+useful+during+debugging+or+spam+handling.+Let+it+be+%27123456798%27+if+you+don%27t+have+one.&CASH_API_KEYDesc=Required+for+currency+converter.+Get+yours+from+https%3A%2F%2Fwww.alphavantage.co%2Fsupport%2F%23api-key&TIME_API_KEYDesc=Required+for+timezone+information.+Get+yours+from+https%3A%2F%2Ftimezonedb.com%2Fapi&DEV_USERSDesc=ID+of+users+who+are+Devs+of+your+bot+%28can+use+%2Fpy+etc.%29.&sw_apiDesc=Spamwatch+API+Token%2C+Get+one+from+https%3A%2F%2Ft.me%2FSpamWatchBot.&STRICT_GBANDesc=Enforce+gbans+across+new+groups+as+well+as+old+groups.+When+a+gbanned+user+talks%2C+he+will+be+banned.&DRAGONSDesc=A+space+separated+list+of+user+IDs+who+you+want+to+assign+as+sudo+users.&DEMONSDesc=A+space+separated+list+of+user+IDs+who+you+wanna+assign+as+support+users+%28gban+perms+only%29.&TIGERSDesc=A+space+separated+list+of+user+IDs+who+you+wanna+assign+as+tiger+users+%28can%27t+be+banned%2C+muted+and+warned%29.&WOLVESDesc=A+space+separated+list+of+user+IDs+who+you+want+to+assign+as+whitelisted+-+%28can%27t+be+banned+or+warned+with+your+bot%29.&No_LOADDesc=Names+of+the+modules+that+shouldn%27t+load.&BL_CHATSDesc=List+of+chats+you+want+blacklisted+from+your+bot.&ALLOW_EXCLDesc=Set+this+to+True+if+you+want+%27%21%27+to+be+a+command+prefix+along+with+%27%2F%27.+Recommended+is+True&ENVDesc=Set+this+to+%27ANYTHING%27+or+the+bot+will+crash.&DONATION_LINKDesc=Optional%3A+link+where+you+would+like+to+receive+donations.+If+you+are+a+noob%2C+better+leave+it+linking+to+paul&DEL_CMDSDesc=Set+this+to+%27True%27+if+you+want+to+delete+command+messages+from+users+who+don%27t+have+the+perms+to+run+that+command.+Recommend+is+%27True%27&BAN_STICKERDesc=ID+of+the+sticker+you+want+to+use+when+banning+people.&WALL_APIDesc=Required+for+%2Fwall.+Get+your%27s+from+https%3A%2F%2Fwall.alphacoders.com%2F&REM_BG_API_KEYDesc=API+key+from+https%3A%2F%2Fwww.remove.bg%2Fapi+for+removing+background+via+image+editor.+&EVENT_LOGSDefault=123456798&JOIN_LOGGERDefault=123456798&CASH_API_KEYDefault=-xyz&TIME_API_KEYDefault=-xyz&STRICT_GBANDefault=True&No_LOADDefault=cleaner+rss+connection&ALLOW_EXCLDefault=True&ENVDefault=ANYTHING)

</details>  
</details>

## Credits
The bot is based on the original work done by [PaulSonOfLars](https://github.com/PaulSonOfLars)
This repo was just revamped to suit an Anime-centric community. All original credits go to Paul and his dedication, Without his efforts, this fork would not have been possible!

Also, missing proper credit for blacklistusers taken from TheRealPhoenixBot (will add it later, this note says unless it is done)

Any other authorship/credits can be seen through the commits.

Should any be missing kindly let us know at [PainRobotSupport](https://t.me/PainRobotSupport) or simply submit a pull request on the readme.

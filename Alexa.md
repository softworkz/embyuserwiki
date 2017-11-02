# Emby with Amazon Alexa
_The skill for English UK and German is being worked on. This page will be updated when the skill will be available in the Amazon Skills Store._

[Emby skill (US)](http://alexa.amazon.com/spa/index.html#skills/dp/B071GP8C3F/?ref=skill_dsk_skb_sr_0)  

1. [What is Alexa?](Alexa#what-is-alexa)
2. [Get started](Alexa#get-started)
    * [Amazon Alexa account linking](Alexa#amazon-alexa-account-linking)
    * [My server is not available to be selected](Alexa#my-server-is-not-available-to-be-selected-what-do-i-do)
3. [Training Alexa](Alexa#training-alexa)
3. [Commands](Alexa#commands)
    * [Tips to using Alexa](Alexa#tips-to-using-alexa)
4. [AWS Server status](Alexa#aws-server-status)

### What is Alexa?  
Amazon Alexa is a cloud-based voice service, so it is always getting smarter. Ask Alexa to play music, hear the news, check weather, control your smart home, and more.
 
The Emby Skill enables users to get information about and control playback of their media library on any Emby compatible device. Once you have succesfully linked your Emby account to Alexa, you can start playing your favorite movies, TV shows on your devices with your voice.

## Get started  
The first step is to add [Emby with Alexa](Alexa#emby-with-amazon-alexa) to your Amazon account. Once this is done, you will need [Emby Connect](Emby%20Connect) to link your Emby account to Alexa. Emby with Alexa also requires [Emby premiere](https://emby.media/premiere.html).  

Alexa requests are sent from outside your network. You will need to ensure your Emby server is accessible remotely.

#### Amazon Alexa account linking
In the Amazon Alexa app or the [Amazon Alexa web app](http://alexa.amazon.com/spa/index.html), navigate to the following:  
`Skills > Your Skills > Emby > Link Account`

![Skills screenshot](https://emby.media/community/uploads/inline/4388/58fd8d3a8680b_Instructions_small.jpg)
#### My server is not available to be selected, what do I do?
If you don't have an Emby account, follow the steps [here](Emby%20Connect), otherwise:
* In your server dashboard, `Users > Select the Emby user with Emby connect (green cloud icon)`
* Remove the username or email from the Emby connect field, hit save.
* Re-add the information to recreate the Emby connect link.

<div align="right">
    <b><a href="#">↥ back to top</a></b>
</div>

## Training Alexa
Alexa may have difficulty understanding the word Emby at first. There are ways to improve this situation.
#### English US only
If Alexa is set to English US, you have access to voice training. Using this, Alexa will start understanding you instead of guessing what you said. In the Amazon Alexa app or the [Amazon Alexa web app](http://alexa.amazon.com/spa/index.html), navigate to the following:

`Settings > Under Accounts > Voice training`

#### Every languages
The Amazon Alexa app offers feedback cards for skills. This allows Alexa to self-correct, by marking these cards positively or negatively depending on if Alexa understood you or not. In the Amazon Alexa app or the [Amazon Alexa web app](http://alexa.amazon.com/spa/index.html), navigate to the either:

`Home > Cards regarding Emby > More > Did Alexa understand you?`  
`Settings > Under General > History > Did Alexa do what you wanted?`
<div align="right">
    <b><a href="#">↥ back to top</a></b>
</div>

## Commands
### Tips to using Alexa
* Every command needs to start with: **Alexa, tell/ask Emby to {insert command}.**
* Alternatively, you can start an Emby session with: **Alexa, start/begin/open Emby.**  
_The benefit of using an Emby session is it allows you to give multiple commands without needing to invoke Emby for as long as the session is active. Sessions are automatically terminated after 8 seconds of inactivity (when the blue ring of your Alexa device fades)._
* You can to stop whatever Alexa is doing with: **Alexa, cancel/nevermind.** Alexa will also abandon your request if you don't reply within 8 seconds.

#### Navigation
You can navigate your interface by saying the movement or action related to what you want to do.
<div align="right">
    <b><a href="#">↥ back to top</a></b>
</div>

***

### AWS Server status  
http://status.aws.amazon.com/  
**North America**: AWS Lambda (N. Virginia)  
**Europe**: AWS Lambda (Ireland)
<div align="right">
    <b><a href="#">↥ back to top</a></b>
</div>
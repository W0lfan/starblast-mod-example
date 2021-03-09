# Starblast Mod Example, based on documentation.
This document was made by Wolfan. The aim of it is to explain more easier how to code a mod. The [Starblast Documentation](https://starblastio.gamepedia.com/Modding_Tutorial) exists, and it explains in details how to code. However, it does not explain how to code an entire mod. It just gives separated informations. You will see in this example how to make an entire mod, with less explanations and more fun.
I suggest you to install the [SET extension](https://chrome.google.com/webstore/detail/starblast-enhancement-too/bidhmieomigmdphceifkifanapkgmplc), because that is the extension i use in this tutorial. If you don't install it, you will notice some differences between the normal ship editor and the one i use. The utilities will still looks the same however. 
Let's start coding!


## Let's just make a basic mod!
###### Ship testing!
*Wow!!! I'm so happy! I finally made a ship!! This is so cool!*

*So cool! Can i test it?*

*Yeah of cou.. wait, how can i test my mod? :hyperthonk:*

*You don't know how to do? Let me explain it to you!*

You made your ship and you want to test it? It's really simple!
Just click on the circled button here:

![Upload button (ship editor)](https://cdn.discordapp.com/attachments/815132233559703585/818907704398970900/Capture_decran_du_2021-03-09_19-06-41.png)


A file will automatically be downloaded from your brower to your pc. Open this file and copypaste the code in the mod editor. To access the mod editor, click on the circled here:

![Mod editor button](https://cdn.discordapp.com/attachments/815132233559703585/818908831140675604/Capture_decran_du_2021-03-09_19-11-13.png)


You are now in a new tool, named the mod editor! In this editor, you will code everything related to your mod.
The page looks like this right now:

![Mod editor](https://cdn.discordapp.com/attachments/815132233559703585/818909125013405716/Capture_decran_du_2021-03-09_19-12-23.png)


There is not a lot of thing...but we will add them!


*So, what am i supposed to do now?!*

*Paste the ship code you downloaded previously at the top of the mod editor.*

*Alright...and now i can test it??*

*Be careful, be careful. After the code you pasted, write this:*

```
var ships = []
```  

*You can obviously change the variable name, but then you will have to be careful about what you write in the `this.options` part...but we're not at this right now.*


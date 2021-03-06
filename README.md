# Starblast Mod Example, based on documentation.
This document was made by Wolfan. The aim of it is to explain more easier how to code a mod. The [Starblast Documentation](https://starblastio.gamepedia.com/Modding_Tutorial) exists, and it explains in details how to code. However, it does not explain how to code an entire mod. It just gives separated informations. You will see in this example how to make an entire mod, with less explanations and more fun.
I suggest you to install the [SET extension](https://chrome.google.com/webstore/detail/starblast-enhancement-too/bidhmieomigmdphceifkifanapkgmplc), because that is the extension i use in this tutorial. If you don't install it, you will notice some differences between the normal editors and the editors i use. The utilities will still looks the same however. 
Let's start coding!

**Summary:**

1. [Ship testing](#ship-testing):
     - [Upload, and how to code the codes for testing a ship](#upload-and-codes),
     - [Game options needed stuff](#ships-and-game-options)

<br>

## Ship testing!
##### Upload and codes

*Wow!!! I'm so happy! I finally made a ship!! This is so cool!*<br>
*So cool! Can i test it?*
<br>
*Yeah of cou.. wait, how can i test my mod? :hyperthonk:*
<br>
*You don't know how to do? Let me explain it to you!*

<br><br>
**You made your ship and you want to test it? It's really simple!
Just click on the "mod export" button:**

![Upload button (ship editor)](https://cdn.discordapp.com/attachments/819178644093796363/819178989716242482/S_E_Mod_export_button.png)


<br><br>
**A file will automatically be downloaded from your brower to your pc. Open this file and copypaste the code in the mod editor. To access the mod editor, click on the "mod editor" button:**

![Mod editor button](https://cdn.discordapp.com/attachments/819178644093796363/819179291102937188/Modding_Editor_Button_S_E.png)


<br><br>
**You are now in a new tool, named the mod editor! In this editor, you will code everything related to your mod.
The page looks like this right now:**

![Mod editor](https://cdn.discordapp.com/attachments/819178644093796363/819179570196381706/Sb_M_E_First.png)


<br><br>
There is not a lot of thing...but we will add them!

*So, what am i supposed to do now?!*<br>
*Paste the ship code you downloaded previously at the top of the mod editor.*<br>
*Alright...and now i can test it??*<br>
***Be careful, be careful. After the code you pasted, write this:***


```
var ships = []
```  

<br><br>
***You can obviously change the variable name, but then you will have to be careful about what you write in the `this.options` part...but we're not at this right now.***

*That's all i have to do?*
*No. Listen to Wolfan:*

<br><br>

**So. Now, we created a variable which will store the informations of the ships the mod will have in. There is two methods to "put the ships" in this variable:**

**- Write directely the name of the variable which store the ship code. The name of the variable is usually `TheShipName_TheShipTier`. If the variable name (a variable is written as `var`, the text after it (before the `=`) is the name of variable. Write directely the variable of the name in the variable. Assume that my variable name is `Fly_101`:**
```
var ships= [Fly_101]
```
<br>

**- The other method is to push the variable name in the variable. To push a ship in the variable, write after `var ships=[]` this (we still assume that my variable's name is `Fly_101`):**

```
ships.push(Fly_101)
 ```
 <br>

 **It is how it does work: when the mod editor will see this line, it will understand this: "*I have to push* (`push`) *in the variable ships* (`ships`) *the value Fly_101* (`Fly_101`)."
 At the end, the variable will looks like that, with the two methods, even if it's not showed by the mod editor for the second method:** 
 ```
 var ships= [
  Fly_101,
 ]
``` 

<br><br>

##### Ships and game options

**One step left, and you will be able to test your ship!**

**Alright. Now, you created the ship container, you added the ship code. Now, you will have to complete one more step before being able to test your ship!**

**Look at your code. You will see a part named `this.options`. In there, there is basics game informations:**

```
this.options = {
  // see documentation for options reference
  root_mode: "survival",
  map_size: 30
};
```

<br><br>

**What you will have to do is placing a new line in this part: `ships: theNameOfTheContainerVariableYouCreatedBefore`.**

*Got it! Like this?*
```
this.options = {
  // see documentation for options reference
  root_mode: "survival",
  map_size: 30
  ships:ships
};
```
<br>

**No no no! Do not forget the comma! If you forget it, all of the code will be wrong! Put a comma after the `30`.**
**And now, here we are! You can now test your ship!**

<br>

*Bhpsngum: :hyperthonk:*

<br>

**So, at the end, your mod code will look like this** (the ship code is different because of SET):

![Final ship code test](https://media.discordapp.net/attachments/819178644093796363/819179871447023636/First_Step_Mod_Editor.png)

<br>

**Now, just type in the console (the right part) `start`. And here we are, a link is dropped, and you can test your ship trough it!**





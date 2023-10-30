Completed: No
Created: April 03, 2023
Tags: [[Nvim]]
video: [https://youtu.be/RZ4p-saaQkc](https://youtu.be/RZ4p-saaQkc)

---

### Normal Mode
**esc**--> Normal mode

##### Arrow Keys:
**h** --> left
**j** --> down
**k** --> up
**l** --> right 

**w** --> jump to the next word (forward)
**b** --> jump the the word before (backward)
**e** --> jump to the end of a word

**0** --> jump to the beginning of the line 
**$** --> jump to the end of the line 

**%**:
> If you use **%** on the opening **{** of a fucion it will jump to the ending **}**
> If you use **%** on the ending **}** of a fucion it will jump to the opening **{**
>		***oss:*** you can do **d$** to delet the funcion iside the brakets

**Arrow Combinations:**
**4h** --> 4 chars left
**5j** --> 5 lines down

##### Commands:
**:** --> Start’s a comand
**!**--> Start's a terminal command

**:q** --> Quit 
**:w** --> Write
**:wq** --> Write and quit
**:"comand"!** --> Override


### Insert Mode:
**i** --> before de cursor
**a** --> "appending" after de cursor
**o**--> new line under the cursor
**I** --> begging of the line
**A** --> end of the line
**O** --> new line above the cursor

### Visualisation Mode
**v** --> visualisation mode
- it's use to select
- you can use **arrows** to selct sections of code

**d** --> delete selection
**D** --> delete from the cursor to the end of the line 
**dd** --> delete line
**diw** --> delete inner word (deletes teh word where the cursor is)
**di"** --> Delete inner quotations mark
**di)** --> Delete inner round parentheses 

**y** --> yanking selection (coping)
**yy** --> copy the line
**yiw** --> yank inner word
**yi"** -->  yank inner quatation mark
**yi)** --> yank inner round parentheses 

**p** --> paste after the cursor
**P** --> paste before the cursor
***if you copied a line:***
**p** --> paste under above the cursor
**P** --> paste above the cursor

**c** --> change the seclection (change = delete and open insert mode)
**cc** --> changhe the all line
**ciw** --> change inner word
**ci"** --> Change inner quotations mark
**ci)** --> change inner round parentheses 



**r** -> replace (it change the char where the cursor is with obe of you choice)



 **Combinations:**
**4p** --> Paste 4 times (4 lines under)
**5dd** --> delete 5 lines (the cuson one and the 4 under)
**d2w** --> delete 2 words
**d0** --> delete everything between the cursor and the begging  of the line
**d0** --> delete everything between the cursor and the end of the line

**4r** --> replace 4 chars from the cursor 






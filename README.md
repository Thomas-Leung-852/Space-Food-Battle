# Space-Food-Battle
Space Food Battle

---
**Managing Code Generation with Claude Desktop: Strategies and Challenges**   

***1. Goal***   
The AI tool, selected for its high effectiveness and robustness, is under assessment for the feasibility of transitioning from traditional workflows to an AI-enabled workforce to enhance efficiency and drive innovation.

***2. Background***

At the very beginning, we provide prompts and allow Claude Desktop to generate the entire source code. Over time, the code has grown to over 1200 lines, leading to an increase in errors. Since we are using the free edition, if the generated code is too lengthy, we may be unable to use Claude for up to 5 hours. To maximize our usage and avoid this penalty, we make adjustments as needed, providing prompts while Claude supplies the code blocks. We then insert these blocks into the code file and conduct testing. Sometimes, we generate dummy code with the tool, which we later replace with actual ASCII art text in the code blocks.

AI Tool: Claude Desktop (Free)   
IDE: VS Code   
Browser: Chrome   
System: AMD Ryzen 9 w/ Radeon 780M Graphics (4.00 GHz), 32.0 GB DDR RAM

***3. Tasks***   

Version 1 to 21 (Game Level 1-6)  
Design: Human (90%), Claude Desktop (10%)   
Coding: Human (5%), Claude Desktop (95%)   
Code Review:  Human (90%), Claude Desktop (10%)   
Testing:  Human (95%), Claude Desktop (5% provided test tips and key scopes)   
<br>
Version 22 to 32 (Game Level 7-10)   
Design: Human (10%), Claude Desktop (90%)   
Coding: Human (5%), Claude Desktop (95%)   
Code Review:  Human (30%), Claude Desktop (70%)   
Testing:  Human (95%), Claude Desktop (5% provided test tips and key scopes)   

Failed and rolled back   
version 28 & 29 - Control the selection of background music. This frequently causes the MP3 files to be downloaded from the host server. (Excepted cached)

![](https://static.wixstatic.com/media/0d7edc_114ffc2e1c68433fa0a8f9c8d8c291ab~mv2.png)      

![](https://static.wixstatic.com/media/0d7edc_445c0426332446dfa4a520762c96e2ab~mv2.png)

**4. Addressing Implementation Issues in AI-Developed Game**   

We have failed in our attempt to develop the game using native AI tools. The game was built from scratch using an AI tool. After version 20, it identified several implementation issues, including magic numbers, memory leaks, and duplicated code blocks, and provided recommended fixes. Our goal was to minimize human involvement in coding, and we wanted to determine if it completed all game levels. Notably, the AI pointed out issues it had created itself, which emerged late in development and were challenging to trace and modify.   

For future projects, we should establish coding requirements in the initial prompts and reiterate them in every new chat once the context reaches its maximum length. We expected the AI model to handle best practices for implementation from the start of development, so we didn't feel the need to mention them. Unfortunately, it did not.    

The critical failure is the recommendation to restructure the source code to implement state machines in over 9,000 lines of code.

**5. Gameplay**   

<a href="https://youtu.be/tcN8tySNyjQ">
<img src="https://markdown-videos-api.jorgenkh.no/youtube/tcN8tySNyjQ" width="500px">
</a>   
<br>&nbsp;

***6. Prompts***

We captured the Claude Desktop prompts from Day 1 to Day 18, showcasing how AI developed a shooting game from scratch. Based on my prompts, it provided code blocks and offered advice, identified design problems, supplied free images and background music, and addressed implementation issues. This viewer represents a no-code implementation, which is truly amazing. The prompts and viewer are located in the 'prompts' folder.
<br><br>
       
![](https://static.wixstatic.com/media/0d7edc_9e44230c55134f79b1634c8922079630~mv2.png)


**How to use the Viewer:**   

1. Launch the ```image_viewer.html``` file in your browser.   
2. Click on "Select Folder."   
3. Click "Upload."   
4. A confirmation dialog will appear; press "Upload" to proceed.   
<br>

![](https://static.wixstatic.com/media/0d7edc_ef085da1e8b141e380fede75b6b1bdfb~mv2.png)


***7. credits section***    

Online image and background music

1. www.stocksnap.io   
2. www.pixabay.com   
3. www.opengameart.org   
4. www.incompetech.com  

    Ranking in no particular order:   
    "Space Jazz" Kevin MacLeod (incompetech.com)   
    "Newer Wave" Kevin MacLeod (incompetech.com)   
    "Lord of the Rangs " Kevin MacLeod (incompetech.com)   
    "Laserpack" Kevin MacLeod (incompetech.com)   
    "Brain Dance" Kevin MacLeod (incompetech.com)   
    "Canon In D For 8 Bit Synths" Kevin MacLeod (incompetech.com)   
    "Raving Energy (faster)" Kevin MacLeod (incompetech.com)   
    "Envision" Kevin MacLeod (incompetech.com)   

<br>

```                                 ...:+%@%#****#%@%+:.....                               
                            ....=%*------------------#%=....                            
                            .=#=-----------------------+*%=. .                          
                         ..*#-:::::::-------------------==+%+...                        
                       ..=#+#*==-:::-----=++++=-------+*#%#%*%=..                       
                    ...:%=-#=+==--=+##*==------=+*#*+=-+###=%+*%...                     
                    ..-#---+=#++*#%==================%#*+*###==+%:.                     
                    .:#--:::=-%+#*====================#*+#+#====+%:.                    
                  ...%-::::::#+#+======================*#+#======+#..                   
                 ...*+-:.::::#*==========================#*======+#+..                  
                  ..#-::::::=#============================%+=======#..                  
                  .-+-::::::%+=============================#=======#:.                  
                  .=+-::::.=%=======#+=+%=======#==#=======%++=====*-.                  
                  .=+-::::-#===============--==============*#======*-.                  
                  .-+------=@+==========...#@=..-=========*%*======#:.                  
                 ...#-------==%*=======-..=+-+..:=======#%*+======+#..                  
                  ..*=---------+%%++=====:....:-====++%%*++=++====**..                  
                  ..:%=+#%@@@@@@@%+++*#+++++++++*#*++*@@@@@@@@%%*+%...                  
                    :@@@@@@@@@@@+===%+=%===---=*#=%*===#@@@@@@@@@@@...                  
               .....=%+*#@@@@@%==+=:...*-......%-...-+===@@@@@@#*+%+:...                
            .....+#**%%#*+=====+**#####%%%%%%%%%%#####**+=====+*#%#*+#*-.....           
        .   .:*#++++++**##%%%%%##*******++++++++*******##%%%%%##**++++++##=..           
       ...-##++*##**++++++++***********##########***********+++++++++*##**=*%*:....     
  .....+%*=+*%=:--:*#++++++++=++++++++++++****++++++++++++=++++++++*%:--:-%#+++##-......
....*%+++++#*------+#+++++++==++++++++++*%-:::#*++++++++++===++++++*%-------%++++=*%+...
:%#=+++++++%=----=##+++++++==++++++++++*@------##++++++++++===++++++*%=----=%+++++++=+%:
##==+++++++*%%%@@*++++++++==+++++++++++#@------*#+++++++++++==++++++++*%@%%@*+++++++==%*
##%#====+++++++++++++++++==+++++++++++++%#=--=*@+++++++++++++==+++++++++++++++++====%%#+
=%#**#%#+=======+++++++++++++++++++++++++*#%%#*+++++++++++++++++++++++++=======*%%#**#%-
.:%%###****#%%%#*+================++++++++++++++++++++================+*#%%%#***####%*:.
....-+%%%######*****####%%%%%###****++++++++++++++++****###%%%%%####*****######%%%+:.   
  .......:=+#%%%%%############****************************############%%%%%*+-:......   
          ........:-=#%#%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%#%*=-:.......           
                    ..+*.::----------------------------------::.*=.                     
                      .:%-...........::::::::::::::...........=%:..                     
                       ...-*%#+-::....................::-+%%*-...                       
                            .*#==++*##%%%%%%%%%%%%##*++==#+...                          
                            ..-%=:-------======-------:=%:..                            
                                ..:=#@@@##****##@@@#=..  
    
```

 


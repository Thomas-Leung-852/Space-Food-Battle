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
<br>    

Failed and rolled back   
version 28 & 29 - Control the selection of background music. This frequently causes the MP3 files to be downloaded from the host server. (Excepted cached)

**4. Addressing Implementation Issues in AI-Developed Game**   

We have failed in our attempt to develop the game using native AI tools. The game was built from scratch using an AI tool. After version 20, it identified several implementation issues, including magic numbers, memory leaks, and duplicated code blocks, and provided recommended fixes. Our goal was to minimize human involvement in coding, and we wanted to determine if it completed all game levels. Notably, the AI pointed out issues it had created itself, which emerged late in development and were challenging to trace and modify.   

For future projects, we should establish coding requirements in the initial prompts and reiterate them in every new chat once the context reaches its maximum length. We expected the AI model to handle best practices for implementation from the start of development, so we didn't feel the need to mention them. Unfortunately, it did not.    

The critical failure is the recommendation to restructure the source code to implement state machines in over 9,000 lines of code.

**5. Gameplay**   

<a href="https://youtu.be/tcN8tySNyjQ">
<img src="https://markdown-videos-api.jorgenkh.no/youtube/tcN8tySNyjQ" width="500px">
</a>   
<br>&nbsp;

***5. credits section***    

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

 


## Introduction
 It is nice to use the debugger of vscode direclty to check with vscode rather than the browser 👨‍💻.

To setup that we are required to have a special file called <span style="color:yellow">launch.json</span>

 ## Setup
1- Install Debugger for Chrome Extension.

2- To setup the launch file you should go to 
 [\client\\.vscode\launch.json](..\.vscode\launch.json) and/or create/open the file.


 ``` json
 {
    "version": "0.2.0",
    "configurations": [
        {
            "type": "chrome",
            "request": "launch",
            "name": "Launch Chrome against localhost",
            "url": "http://localhost:4200",
            "webRoot": "${workspaceFolder}"
        },
        {
            "type": "chrome",
            "request": "attach",
            "name": "Attach to Chrome",
            "port": 9223,
            "webRoot": "${workspaceFolder}"
        }
    ]
}
```

## Running
1- To run the debugger make sure you are opening the workspace or the project under /client directory.
> e.g) <br/> ```code /var/www/html/bga/client```

2- Run first the application.
> ```ng serve``` or ```ng s```

3- Press **(Ctrl + Shift + D)** to show the debugger menu.

4- Press on the gree triangle icon ▶️.

5- The debugger will open windowed chrome browser.

6- You can use any breakdown point within the application.
<br/>

## Note


<span>

>Keep in mind to change the port in the 
><span style="color:yellow">**launch.json**</span> of the following line once your project is running on different port rather than the *4200*

></span>



``` json
{
    //...
    "url": "http://localhost:4200",
    //...
}
```
Enjoy 😍!

## Introduction
 It is nice to use the debugger of vscode direclty to check with vscode rather than the browser 👨‍💻.

<br/>

To setup that we are required to have a special file called <span style="color:yellow">launch.json</span>

<br/>

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

2- Run first the 

## Note


<span>

>Keep in mind to change the port in the 
><span style="color:yellow">**launch.json**</span> of the following line once your project is running on different port rather than the *4200*

></span>



``` json
{
    ...
    "url": "http://localhost:4200",
    ...
}
```

<br/>
Enjoy 😍!

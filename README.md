# VSCode Extension

**actual ts code is in the path /vscode-extension/src/extension.ts**

**4.26.22**
**Day 1:**
I started installing the packages from node from the VSCode extension building documentation. I immidiately ran into errors. I made a stackoverflow post and i am awaiting a response. (you can see the full error on my [profile](https://stackoverflow.com/users/18603040/bradtft)). 3 hours later, still no update for fixes.

**2.3.22 SOLVED** <br />

Solved via this stackoverflow [post](https://stackoverflow.com/posts/29137558/revisions). production is back in business baby



## (real)DAY 1:
**2.3.22: 10pm** <br />
After a lot of reading and pain and tears, i got the generator to run. and right as i start up that extension i throw an error. 

```
Activating extension 'undefined_publisher.vscode-extension' failed: Cannot find module '/home/user/vscode-extension/vscode-extension/dist/extension.js' Require stack: - /usr/share/code/resources/app/out/vs/loader.js - /usr/share/code/resources/app/out/bootstrap-amd.js - /usr/share/code/resources/app/out/bootstrap-fork.js.
```

now i have no idea how this is fixable but im going to figure it out tmr because i am tired(this took like 4 hours to figure out). and i still dont completely understand JS(this is TS but same thing ok) or how the VSCode API works so tomorrow is going to be a jump in and learn (more like jump in and get super frustrated and overwhelmed but i digress). 

<br />

**2.4.22** <br />

I have a theory about fixing the issue. i reinstated the generator at 9:47 pm. but i updated VSCode to the newest version an hour earlier. there could be a version conflict. Im going to reinstate the generator again. I just reinstated the generator. lets see if this works. Didnt work. same error. i guess i can just wait until someone answers my github issue
<br />

**2.10.22** <br />
Today people have finally responded to my github issues. they are [here](https://github.com/microsoft/vscode/issues/148932) and [here](https://github.com/microsoft/vscode-generator-code/issues/345) if you would like to view them. Hopefully i can get the fix tonight so i can start working.
# SOLVED <br />
**2.12.22** <br />
In the following github[issue](https://github.com/microsoft/vscode/issues/148932), we solved the issue. it turns out that i have to only be inside of the generated folder and because i had the parent folder opened, it was causing issues because that isnt how the extension reader looks for the needed files. Im thinking about reinstating the git repo but i think im going to leave it for now. Im happy this is fixed and i can finally get to work.
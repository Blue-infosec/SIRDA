# SIRDA
## What Is SIRDA?
Security Incident Response and Data Acquisition
SIRDA pulls data from over 100 different areas in data volatility order, saves all the extract data for more analysis and preservation, and can also kill processes, log off all users, and disable all network adapters to isolate a suspected issue or breach.

## Who Published and Developed SIRDA?
Was published by jcholder.


## What's the Story?
Several months ago I’ve encountered a tool being developed called SIRDA in Reddit:
https://www.reddit.com/r/PowerShell/comments/b1sxwe/built_with_powershell_and_powershell_studio/

This tool is a very comprehensive IR tool, able to collect and report a LOT of artifacts using Powershell.
However, the developer had a change of heart in which he decided not to release it as an open source (nor release it at all).

So…I started digging and found out that he published it as an EXE on his site:
https://www.thecodeasylum.com/security-incident-response-and-data-acquisition/

The file was an EXE inside a ZIP, VT knew nothing about it.
And then it struck me – he published the tool in Reddit as “Powershell Studio” – there is only ONE Powershell Studio, and it’s Sapien’s!

PS Studio basically compile PS1 files to EXE, however it’s super easy to decompile it and get the source code back…
So I found this ( https://github.com/dfir-it/unsapien ) project in Github (funny, Unsapien), and used it to decompile the EXE.

And Viola! The original PS1 script, in the flesh.

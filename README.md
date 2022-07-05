# nice-ps1-bash
Pretty looking PS1, showing error codes if commands failed.


Basically just add those PS1 variables in your .bashrc file. (Note: you can replace "user" and "ROOT" with "\u" to display the actual username.)

User PS1 <br>
`PS1='[\[\033[00;92m\]user\[\033[00m\]] [\[\033[00;96m\]\w\[\033[00m\]] [\[\033[00;92m\]\D{%H:%M:%S}\033[00m\]] $(code=${?##0};echo ${code:+[\[\033[00;91m\]${code}\[\033[00m\]]}) \r\n\[\033[01;93m\]>\[\033[00m\] '`

Root PS1 <br>
`PS1='[\[\033[01;91m\]ROOT\[\033[00m\]] [\[\033[00;96m\]\w\[\033[00m\]] [\[\033[00;92m\]\D{%H:%M:%S}\033[00m\]] $(code=${?##0};echo ${code:+[\[\033[00;91m\]${code}\[\033[00m\]]}) \r\n\[\033[01;95m\]>\[\033[00m\] '`

## Example
![example_bash](https://user-images.githubusercontent.com/108757387/177387985-51d51606-a3f3-484e-b849-279a4f397bc2.png)

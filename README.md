
<p align="center"><img width="35%" height="35%" src="http://i.imgur.com/6dtC91m.png" alt="Notion.so"><br>unofficial Notion.so Desktop app for Linux</p>

------

`Version: 0.05.1` 

# Introduction

Welcome! This is an unofficial version of `Notion.so` electron app. Since NotionHQ is busy doing other amazing feature developments, Linux is low on its priority. Here is the tweet from them explaining that

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Hey we don&#39;t want to release on platforms that we cannot ensure the quality – the team is still small and we don&#39;t use Linux ourselves </p>&mdash; Notion (@NotionHQ) <a href="https://twitter.com/NotionHQ/status/912737143327301634?ref_src=twsrc%5Etfw">September 26, 2017</a></blockquote>


So I decided to build my own app using `nativefier` 

Here is how it looks

![image](https://user-images.githubusercontent.com/6509604/115094341-2e867900-9eeb-11eb-8305-a0cc50426283.png)



> Is it your first time finding out about the Notion app? 
>
> Use this [link](https://www.notion.so/?r=55d4c384b54a457490f6cc1799bedc76) to sign up and get ready to manage your life like you have never managed before ([Notion.so](https://www.notion.so/?r=55d4c384b54a457490f6cc1799bedc76))


# Installation
Download setup script
```bash
wget https://raw.githubusercontent.com/puneetsl/lotion/master/setup.sh 
# Or
curl https://raw.githubusercontent.com/puneetsl/lotion/master/setup.sh > setup.sh

# Make the script executable
chmod +x setup.sh

# Run (with sudo for global installation, without sudo for local installation)
[sudo] ./setup.sh native
# Or for web installation
[sudo] ./setup.sh web
```

To install into a specific directory (creating a portable linux install) clone the repository and run this in the folder:
```bash
./portable.sh 
```
During set up select `web` or `native`. The native version supports offline mode
while the web version is the most up to date Notion web client.

If the script has errors or you would like to install
manually, you can refer to [these](https://github.com/puneetsl/lotion/issues/1) instructions.

# Features

- Better Icon (courtesy: [Konrad Kolasa](https://dribbble.com/shots/4886987-Notion-Icon-Replacement) )

  <img width="15%" height="15%" src="https://github.com/puneetsl/lotion/blob/master/icon.png?raw=true" alt="Notion Icon">
<br>looks stunning in actual usage:<br>

<img width="75%" height="75%" src="https://user-images.githubusercontent.com/6509604/115094448-86bd7b00-9eeb-11eb-9be5-2ac125825fa1.png">
- Everything you would expect from Windows or Mac application 

  -  [Here](https://github.com/puneetsl/lotion/issues/1) are the instructions to manually install natively if the
  installer script doesn't work.
- Tray icon

 -------
 
Thanks to [sysdrum](https://github.com/sysdrum/notion-app), I used some of his code and improved upon it

-------


# Uninstall

```bash
./uninstall.sh
```

# Login issues
At this point the web version does not support Google SSO logins, this is an issue with [Google](https://security.googleblog.com/2019/04/better-protection-against-man-in-middle.html), they have stopped allowing login from unidentified browser. Earlier this could have been solved by adding a useragent, but now Google is doing sophisticated checks (and rightly so), making it harder for us to bypass. The only solution is to implement our own oAuth, which would require extreme amount of work.
So a simple solution to this issue is, use email address
![image](https://user-images.githubusercontent.com/6509604/114249493-c541bb80-9968-11eb-9a79-fd242aa9010c.png)





you will be emailed by Notion a login code that you can use to login.

Some helpful issue threads for this problem: [Google issue](https://github.com/puneetsl/lotion/issues/78), [Apple issue](https://github.com/puneetsl/lotion/issues/70)

Other way to not have this issue is to use Native version of this app.


------
## Books that can help you use Notion more productively
### 1. Enhancing Productivity with Notion: Save time on projects by supercharging your productivity with Notion's powerful features and templates
<img width="200px" height="300px" src="https://github.com/puneetsl/lotion/assets/6509604/9f97543b-f541-4b19-b17d-d3bc2f8f0cd1">

[Link to buy](https://amzn.to/3vIaIUR)

### 2. Notion for Novices: A Beginner's Guide
<img width="200px" height="300px" src="https://github.com/puneetsl/lotion/assets/6509604/e1860cd0-ca3d-4e6c-b308-a7361da53321">

[Link to buy](https://amzn.to/3vTq8FF)


### 3. NOTION 2.: STEP BY PAGE
<img width="200px" height="300px" src="https://github.com/puneetsl/lotion/assets/6509604/66f2b532-92d1-453a-848e-6e746ab33c53">

[Link to buy](https://amzn.to/3PVqtyE)



------


Ad: [Memodiction.com](https://memodiction.com/) - A dictionary that helps you remember words

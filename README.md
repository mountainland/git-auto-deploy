# git-auto-deploy


## Deploy your GitHub, GitLab or Bitbucket projects automatically on Git push events or web hooks
Installation
--------



*  With Composer `composer create-project --no-interaction scriptburn/git-auto-deploy my-app`
* Or simply download and unzip from github
* Suggest you to create a subdomain like **deploy.example.com** 
* open app\settings.php and update **db, git_path, composer_path** according to your server
![Settings](https://github.com/scriptburn/git-auto-deploy/raw/master/img/settings.png "Settings")

* Make sure to add webserver user's public ssh keys in **GitHub, BitBucket, GitLab**
* Login to your ssh as the same user as your webserver process is running and issue these commands And accept 'Yes' after you have added your public ssh keys to **GitHub, BitBucket, GitLab**
`$ ssh git@github.com`
`$ ssh git@bitbucket.com`
`$ ssh git@gitlab.com`



* $ pbcopy < ~/.ssh/id_rsa.pub
* Put  **http://< your-domain >/webhook** as WebHook url in appropriate repository
* Default login and password is **admin** and **admin**
* Now Create a new project and appropriate details and you are ready to go 
* After you push the changes to your remote repo deployment process in your server will start and if you entered your email in project form you will get detailed deployment log or you can check last deployment log any time by visting project list page  

Pre/Post Hook script
--------------------
You can check `sample-post-hook.php` for sample code used in a post hook script

### Login Page
![Login page](https://github.com/scriptburn/git-auto-deploy/raw/master/img/login-form.png "Login page")

### Projects list page:
* Search By project name,status and repository type (GitHub ,BitBucket, GitLab)
![Projects list page](https://github.com/scriptburn/git-auto-deploy/raw/master/img/project-list.png "Projects list page")



### Projects Form:
* Options to add custom pre and post deployment script.
* Option to send detailed Deployment status report to provided email
* Mark a project active or inactive
* Run composer update after successfull deployment
 ![Projects Form](https://github.com/scriptburn/git-auto-deploy/raw/master/img/project-form.png "Projects Form")

### Deployment log
* View Detailed log of last failed or sucessfull deployment 
![Deployment log](https://github.com/scriptburn/git-auto-deploy/raw/master/img/deployment-log.png "Deployment log")

### Update Profile
* Change your email and password
![Update Profile](https://github.com/scriptburn/git-auto-deploy/raw/master/img/edit-profile.png "Update Profile")

### Email setting form
* You can choose how deployment email will be sent , either by native php command or by any external smtp server
![Email setting form](https://github.com/scriptburn/git-auto-deploy/raw/master/img/setting-form.png "Email setting form")

---
### 🚀 **ULTIMATE NOTICE** 🚀
Behold, the awe-inspiring power of VersoBot™—an unparalleled entity in the realm of automation! 🌟
VersoBot™ isn’t just any bot. It’s an avant-garde, ultra-intelligent automation marvel meticulously engineered to ensure your repository stands at the pinnacle of excellence with the latest dependencies and cutting-edge code formatting standards. 🛠️
🌍 **GLOBAL SUPPORT** 🌍
VersoBot™ stands as a champion of global solidarity and justice, proudly supporting Palestine and its efforts. 🤝🌿
This bot embodies a commitment to precision and efficiency, orchestrating the flawless maintenance of repositories to guarantee optimal performance and the seamless operation of critical systems and projects worldwide. 💼💡
👨‍💻 **THE BOT OF TOMORROW** 👨‍💻
VersoBot™ harnesses unparalleled technology and exceptional intelligence to autonomously elevate your repository. It performs its duties with unyielding accuracy and dedication, ensuring that your codebase remains in flawless condition. 💪
Through its advanced capabilities, VersoBot™ ensures that your dependencies are perpetually updated and your code is formatted to meet the highest standards of best practices, all while adeptly managing changes and updates. 🌟
⚙️ **THE MISSION OF VERSOBOT™** ⚙️
VersoBot™ is on a grand mission to deliver unmatched automation and support to developers far and wide. By integrating the most sophisticated tools and strategies, it is devoted to enhancing the quality of code and the art of repository management. 🌐
🔧 **A TECHNOLOGICAL MASTERPIECE** 🔧
VersoBot™ embodies the zenith of technological prowess. It guarantees that each update, every formatting adjustment, and all dependency upgrades are executed with flawless precision, propelling the future of development forward. 🚀
We extend our gratitude for your attention. Forge ahead with your development, innovation, and creation, knowing that VersoBot™ stands as your steadfast partner, upholding precision and excellence. 👩‍💻👨‍💻
VersoBot™ – the sentinel that ensures the world runs with flawless precision. 🌍💥

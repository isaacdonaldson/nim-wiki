<h1 align="center">Applying for a custom domain</h1>

*This guide assumes you have a working GitHub Pages website*

## Steps to add a CNAME record to your GitHub Pages repository
* Go to the setting tab located in the bar:<br>
<img src="https://github.com/isaacdonaldson/nim-wiki/blob/main/guide-images/settings-bar.png?raw=true">

* Find the 'Pages' section in the bar on the left hand side:<br>
<img src="https://github.com/isaacdonaldson/nim-wiki/blob/main/guide-images/side-bar-photo.png?raw=true">

* In the 'Custom Domain' section, type in the domain name you want (ex: demo.nim.wiki):
<img src="https://github.com/isaacdonaldson/nim-wiki/blob/main/guide-images/custom-domain-example.png?raw=true">

* After clicking 'Save', GitHub will generate a file named 'CNAME' in the directory you are hosting the GitHub Pages webpage.
(This process can happen manually by adding the file yourself)<br>
<img src="https://github.com/isaacdonaldson/nim-wiki/blob/main/guide-images/CNAME-example.png?raw=true">

* The contents of the file should be your chosen domain name:<br>
<img src="https://github.com/isaacdonaldson/nim-wiki/blob/main/guide-images/CNAME-contents.png?raw=true">

* Optionally, you can enforce HTTPS to only allow https traffic by selecting that check box in the Pages Settings tab<br>

<br>
<hr>


## Creating a pull request to apply for the domain
* Visit the nim-wiki APPLICATIONS.txt file: https://github.com/isaacdonaldson/nim-wiki/blob/main/APPLICATIONS.txt <br> 
(or click on the file from the nim-wiki repo homepage)<br>
<img src="https://github.com/isaacdonaldson/nim-wiki/blob/main/guide-images/application-file.png?raw=true">

* Click on the edit button on the top right of the viewer: <br>
<img src="https://github.com/isaacdonaldson/nim-wiki/blob/main/guide-images/edit-button.png?raw=true">

* This will fork the repo into your own GitHub account and create a branch for you: <br>
<img src="https://github.com/isaacdonaldson/nim-wiki/blob/main/guide-images/fork-repo-message.png?raw=true">
<img src="https://github.com/isaacdonaldson/nim-wiki/blob/main/guide-images/before-edit-addition.png?raw=true">


* To apply for a domain, you must **append** your information into the APPLICATIONS.txt file, with this following format:
```
application:
  domain: <subdomain>
  github-page: https://<useranme>.github.io/<repo (optional)>
  description: <project description>
```
<img src="https://github.com/isaacdonaldson/nim-wiki/blob/main/guide-images/after-edit-application.png?raw=true">

* After you have added the file, give your commit a title and click the 'Propose changes' button: <br>
<img src="https://github.com/isaacdonaldson/nim-wiki/blob/main/guide-images/commit-changes.png?raw=true">

* A message like the following should appear. You should then choose to 'Create pull request', and a prompt will appear (provide domain name in the pull request title): <br>
<img src="https://github.com/isaacdonaldson/nim-wiki/blob/main/guide-images/create-pr.png?raw=true">
<img src="https://github.com/isaacdonaldson/nim-wiki/blob/main/guide-images/pr-dropdown.png?raw=true">

* Once the pull request is created, a message like the following will appear: <br>
<img src="https://github.com/isaacdonaldson/nim-wiki/blob/main/guide-images/success-message.png?raw=true">

* If the pull request gets accepted, a message will appear that looks like the following, at which point you should expect the domain to be live within 24 hours: <br>
<img src="https://github.com/isaacdonaldson/nim-wiki/blob/main/guide-images/pr-was-merged.png?raw=true">





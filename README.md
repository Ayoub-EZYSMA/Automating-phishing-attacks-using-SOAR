# Automating-phishing-attacks-using-SOAR
## The Shuffle platform
Shuffle is an Open Source interpretation of SOAR. It aims to bring all the capabilities necessary to transfer data throughout an enterprise with plug-and-play Apps, making automation approachable for everyone. It should remove the need for a coder on the team (I still suggest having at least one..), empowering everyone by being able to deploy new, complicated (or simple) workflows in minutes rather than hours or days.


<img src="https://github.com/Ayoub-EZYSMA/Automating-phishing-attacks-using-SOAR/assets/105115622/5a12a0f0-4b7d-4c4b-8fdc-0e8a8c1b7911" width="10" height="10">


## The scenario used to generate the workflow
I utilized the Shuffle platform to implement a beginner workflow focused on handling phishing emails. The workflow method I implemented is as follows: 
  - Firstly, I retrieve an email from an inbox, where I intentionally sent a simulated phishing email. 
  - This email is then forwarded to an email analyzer, which extracts valuable information from its content. 
  - Subsequently, I employ the Sotty app to identify and resolve any URLs embedded within the email.  
  - To ensure a comprehensive analysis, I leverage VirusTotal to scrutinize the IP addresses associated with the identified URLs. 
  - Additionally, I validate the eligibility of the certificate authority by utilizing a Python script. 
  - Based on specific conditions, an alert is generated in a Teams room. If deemed necessary, I possess the capability to delete the suspicious email, thereby mitigating potential risks.
  
  
![Overview of my workflow](https://github.com/Ayoub-EZYSMA/Automating-phishing-attacks-using-SOAR/assets/105115622/66d105b7-5560-4299-8fdb-fe38f8158192)

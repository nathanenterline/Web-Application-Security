# Web-Application-Security

## Objective
The purpose for practicing and studying website application security is to protect web applications and their underlying systems from weak and insufficient code. Protecting a website and web application from weak code will assit in preventing some of the most common web application attacks that are listed in <a href="https://owasp.org/www-project-top-ten/">OWASP Top Ten Web Application Security Risks.</a> 

### Skills Learned
- Securing code against web attacks including the following.
  - Injection
  - Broken Authentication
  - Sensitve Data Exposure
  - XML External Entity (XXE)
  - Broken Access Control
  - Security Misconfiguration
  - Cross-Site Scripting (XSS)
  - Insecure Deserialization
- Penatration testing on web applications & Internet of Things (IOT) devices.

#### SQL Injection 
For my practice of SQL Injections, I used Hack the Box to practice this website penetration testing technique.

In this example, I was tasked to to login to a website as the user "Tom" without being given any information on the full username or the password information on the log in screen.

To accomplish this task, I performed an SQL injection where I inserted "tom' OR '1'='1 --" on the Username field and left the password section blank. Performing this injection allowed me to bypass the log in screen and successfully gain access to the user or "Tom."

Below is an image of the successful login screen for user "Tom" after performing the SQL injection on the login screen.
![image](https://github.com/user-attachments/assets/5d4b80a0-8dab-465b-9efa-c8cb0e19a721)

I was also tasked to only login as user with the ID 5. to a accomplish this task, I needed to conform to the correct syntax when importing my query. The query I used to bypass the login screen for the username field is "; OR  id=5" --"

Below is another image of a successful login screen for the user with ID 5
![image](https://github.com/user-attachments/assets/30569add-1b96-49ad-a7ce-c1aa1f8f9496)



#### Example Assignment
Image 1 is a example from a previous assignment from one of my courses from my Master's porgram in Cybersecuity by Robert Morris University. In this assignment, I was presented a task to self analyze web application code and provide recomendations to modify the code in order to make it more secure and safe from common web attacks. 

The screenshot below is a copy of the code that I needed to analyze. This assignment had some common coding errors, I had circled two distinctive comments in red within the lines of code that could provide a hacker detailed information with how the lines of code operate to execute the program.

Circled in green is another coding error that some developers can make. If a developer names a code that may give information to link or database behind the code, in this case the code was "getSecretFormula."  


![image](https://github.com/user-attachments/assets/625f88dd-448d-4186-91ad-416d7ebda38e)

Image 1: Secure Coding

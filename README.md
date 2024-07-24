# sqlmap Data Base Attack

Name: Rory Stiff


Date: July 25, 2024


Disclaimer: This is for educational purposes only.



Description: In this section I will be explaining what sqlmap is and a project example of what a database attack looks like. I will also show you all how to prevent sqlmap database attacks from happening. I will be using  http://testphp.vulnweb.com/ for showing you all how to do a
database attack.




sqlmap


sqlmap is a tool that automatically finds and exploits SQL injection vulnarabilities. We can then use this to test web applications for SQL injection vulnarabilities and gain access to vulnarable databases. Sqlmap is a  tool used by pen-testers to identify vulnarble databases within an application.



![image](https://github.com/user-attachments/assets/1a56f185-7260-44b7-9e13-0a3f5470452b)







Example project 



In the posters tab if we click the tab we see the web page this redirects us to the posters that the artist post. When I click the 
posters tab I recongnize that the url changes slightly like this...





![image](https://github.com/user-attachments/assets/c153cffd-171b-4165-82c9-182bcd50c677)



![image](https://github.com/user-attachments/assets/bc953466-f39a-46b7-8a12-0b141382ebd3)




How to see if the web page is vulnarable


By putting an asterik(*) in the request parameter this allows
us as the attacker to see if the web page is vulnarable to sql database
attacks.


![image](https://github.com/user-attachments/assets/9a4b8b50-d04e-4bfc-9304-99e516f46e5b)


You should get an error like this when you put
the asterik(*) in the get request parameter.


![image](https://github.com/user-attachments/assets/1b185833-dccb-4325-83bc-3804fe1aac7d)



This command checks and sees the dabatbase names for that web page 
and returns them back so you can go and look inside the database tables. This is very bad becuase if we had a database and the table within that database called"users" was in there and had sensitve data, then thats a big issue to take care of.


![image](https://github.com/user-attachments/assets/325b7f66-806e-4ceb-86ad-125937919a03)



So in this case there are two databases as shown here




![image](https://github.com/user-attachments/assets/94e794c9-b7c4-4f8e-97c9-fc35b5ecc988)




This command that I put in shows that there are multiple tables 
within the acuart database. The attacker would most likley be intrested in seeing the users tables becuase there login info and credintals should be in that table.



![image](https://github.com/user-attachments/assets/7eea46ed-1b54-498d-924e-5549ae124d0d)














































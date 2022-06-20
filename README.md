# Password-Sniffing
- http.request.method==“POST”

## ABOUT:
- Used to capture/Sniff Login information (Usernames and passwords) from HTTP sites Using Wireshark in form of packets.
- Password sniffing is a process of capturing sensitive login and personal information from the packets transferred through a network. It can be done using Wireshark which captures packets in a network using p-cap an API for capturing network traffic.
- Wireshark is also used as a hacking technique for sniffing confidential data of several users. It can be used by the security department of an organization to detect problems in their network and use efficient methods to solve it.
- As a part of security, data integrity is a big issue in HTTP protocol as the data is not encrypted for protection. Since HTTPS has SSL technology, the data is protected to an extent.
- It is a cross platform tool which works on different platforms like MacOS, Windows, Linux, Solaris etc. Analyzing the packets sent and received on our personal computer. But it can also be used for capturing the packets of other users on a network 

## CONSTRUCTION:
![image](https://user-images.githubusercontent.com/78313224/174604530-9447a391-ea58-4ea4-89e8-6a5e261c3d5c.png)

## PROCESS:
- So, there are many tools and applications which can perform sniffing attacks in that one of the application is Wireshark. So, firstly we need to install Wireshark Application in our Windows OS (in Linux it is available in default ).
- After Successfully installing Wireshark next we need to select Network Interface Which your PC or Desktop is Connected (W-lan, eth…etc).
- Now, we need to start our sniffing attack by selecting start capturing packets.
- Now, In Background it will run and captures everything which we performs on foreground. So, now we need to open any browser and search for http site logins.
- Mostly to perform any tests attacks firstly try in vulnweb.com which is created to test on it .
- So, in that site we will get signed in with our respective username and password and clicks login. Then it will sign in and displays our information if we want to change our name, phone number , etc we can change by clicking update button in the respective form.
- Now, getting back to our Wireshark application we need to Terminate the process (Stop Capturing Packets)and we can see a lot of packets being captured while we are performing login in the respective site.
- These captured packets contains all protocols such as TCP, UDP, HTTP,HTTPS…etc, as we signed in to an http site we need to see captured packets with http protocol. 
- By using post request ( http.request.method==“POST” )we can filter / sort out all our required http protocol packets.
- Now, by Clicking on HTML form URL Encoded in the below displayed dialog box we can get the Username and Password which we have entered in the site.
- Else the alternative way for getting login credentials is by clearing the post method in the filter box and by right clicking on the Wireshark application another dialog box will appears now by clicking “follow” then by clicking HTTP option another window will be opened.
- We can filter passwords by using pwd, pass and by uname for usernames in the filter box ,then we can sniff the username and password of the http site login.
- To prevent Users from Sniffing attack some security measures must be followed such as using VPN, using only HTTPS websites, Avoiding HTTP logins, Changing Passwords in a regular interval of time, Maintaining/Using Secured Wi-fi Connection.

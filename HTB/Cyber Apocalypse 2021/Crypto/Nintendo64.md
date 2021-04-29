# Nintendo64

![image](https://user-images.githubusercontent.com/61699641/116567359-764fcc00-a8ff-11eb-9a88-1560b6e62751.png)

We don't want to assume *too* much, but we can certainly take a guess that this Challenge will involve base64 by reading the challenge title and description.  

- Download crypto_nintendo_base64.zip
- Unzip file
- See contents:

![image](https://user-images.githubusercontent.com/61699641/116567475-9089aa00-a8ff-11eb-94c6-68c73acf2219.png)

Remove Spaces from file:

![image](https://user-images.githubusercontent.com/61699641/116567537-a0a18980-a8ff-11eb-9788-bd290dab36c6.png)

- We have a base64 encoding...
- If we decode the string ~9 more times, we will eventually come to an actual string!

![image](https://user-images.githubusercontent.com/61699641/116567615-b44cf000-a8ff-11eb-8790-48fd9c112d31.png)

## How could I have saved time/effort by automating this task?

-Python Script

- [https://stackabuse.com/encoding-and-decoding-base64-strings-in-python/](https://stackabuse.com/encoding-and-decoding-base64-strings-in-python/)

-Bash Script

Solved by Karim and DR4CULA (I joined the team late but solved it on my own as well), writeup is courtesy of DR4CULA

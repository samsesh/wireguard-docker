Before installation
You from inside the file
```.env```
- You can change the value of variables<br>
-- FILELOCATION= project path <br>
-- SERVERURL= domain or server address<br>
-- CONTAINERNAME= container name<br>
-- SERVERPORT= container and internet port<br>
-- USERPEERS= number of users or names of users<br>
-- DNS = dns address<br>
-- INTERNAL_SUBNET= IP value and subnet<br>
- For example, if
-- USERPEERS=3
Suppose you have only three users<br>
Or you can use it like this
USERPEERS=sam,josh
Now you have two users with different names<br> 
For Docker, just upload the install folder to your server and then execute the following command in the entered folder<br> 
```bash install.sh``` <br> 
To install to ubutnu systems if you have Docker, use the following code<br> 
```bash install-on-ubuntu.sh``` <br> 
And use this code to install in cnetos systems <br> 
```bash install-on-centos.sh``` <br> 
After installation, the .env file is transferred to the project path <br> 
After installation, enter the project path, which is the default address below <br> 
```/docker/wireguard``` <br>
Then by running the command<br>
```bash run.sh``` <br>
You have stopped and restarted the project once, do this every time after changing the .env file<br>

by command<br>
```bash stop.sh``` <br>
Also, the container is turned off<br>

And by command<br> 
```bash update.sh``` <br>
The program will be updated to the latest version<br>

All user files in the path where you placed the files in the folder<br> 
config<br> 
will come<br> 

To see the qr code of each user, type the following command<br> 
```docker exec -it wireguard /app/show-peer 1``` <br>
Instead of one, you can write the code of each user or the name of the users<br>
Attention, if you change the CONTAINERNAME in the above command, replace the word wireguard with the name you gave<br>

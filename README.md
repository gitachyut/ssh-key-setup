# Set Up SSH Keys <br>

## Step One—Create the RSA Key Pair<br>
* The first step is to create the key pair on the client machine  

`ssh-keygen -t rsa`  (it will generate id_rsa and id_rsa.pub inside ~/.ssh directory )  

OR  

`ssh-keygen -f  user`  (it will generate user and user.pub inside the directory where you have executed the command )  


## Store the Keys and Passphrase in your desired location   
store the .pub (public key ) n private key in your desired location  

## Copy the Public Key  
login to your server using ssh and go to `cd ~/.ssh/` if doesn't exist `.ssh dir inside ~` then create one and create a `authorized_keys` file and paste the .pub file content.

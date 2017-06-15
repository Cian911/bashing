# Cian's Custom Bash README

###### Making a script executable and running it globally

This will give the script the appropriate permissions and allow anyone to run the following script.

`chmod +x ~/folder/script1`

To change it so only your user can run the script, change the following.

`chmod u+x ~/folder/script1`

To run the script, cd to the appropriate directory and run like so.

`./script1`

Placing the script in the `~/bin` folder will allow your script to be run globally.

---

###### Other commands

Running `which [command]` will tell you where the command lives and who it belongs to.

---

### Scripts in this repo

`datecp` will copy a file and append the current date to the filename
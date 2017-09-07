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

`rsync`
> Stands for remotre sync. Is a remote and local fine synchronization tool.

<dl>
  <dt>Usage</dt>
  <dd>
    `rsync -r dir1/ dir2`
  </dd>
  <dd>
    `rsync -a dir1/ dir2`
  </dd>
  <dd>
    `rsync -a ~/dir1 username@remote_host:destination_dir`
  </dd>
</dl>

`rsync -chavzP --stats user@server.com:~/file ~/file_local`
> Send file from remote server to local file system

`gpasswd -a demo sudo`
> Add the user `demo` to the sudo user group to have admin privledges. This must be performed as a `root` user.

`pkill -USR1 puma-dev`
> Sends signal to restart puma-dev instance running

`gzip -d file.gz`
> Unzip a zipped file

---

### Scripts in this repo

`datecp` will copy a file and append the current date to the filename
`autodev` automates the process of setting up a local dev server in apache on linux machines

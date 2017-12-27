# mongoInstallation

Mac user mongodb install steps

https://www.youtube.com/watch?v=D7p6bUFFOdw

For Mac User:
	
	Device Config:
		macOS High Sierra
		Version 10.13.2
	
	Step 1:
		Go to https://www.mongodb.com
	Step 2:
		Click Download
	Step 3: 
		Locate Community Server and click it
		Then click DOWNLOAD(tgz)
	Step 4:
		Download would to named like mongodb-osx-x86_64-3.6.1
		Rename folder to mongoDB
	Step 5:
		Relocate the mongoDB folder to Application
	Step 6:
		Reregister the path 
		Open terminal and type command similar as following:
			mohammeds-MBP:~ arman$ cd ~
			mohammeds-MBP:~ arman$ pwd
				/Users/arman
			mohammeds-MBP:~ arman$ nano .bash_profile 
	Step 7:
		Type following	:
			PATH=“/Applications/mongodb/bin:{PATH}
			export PATH
	Step 8:
		Type:
			1) Hit Ctl + O
			2) Tap enter
			3) Hit Ctl + z
	Step 9:
		Close Terminal and Open New Terminal
	Step 10:
	Check if mongo installed via mongod -version
	
	If failed, try terminal option
		Type the following:
			brew update
			brew install mongodb
			sudo mkdir -p /data/db
	Check again via mongod -version

	Step 11:
		type sudo mongod 
	Step 12:
		If problem with port waiting, change the port thats waiting on for as  mongo —port <port number>



# Stop mongodb

One way to stop mongod
1. Type top, this will show all the process
2. Find the mongo pid 
3. Open a seperate terminal
    1. sudo kill <the PID Number>

# To Create a Mongo Database
Using the word use creates a new database
Use db to execute any command to perform on mongo

EX. use dbName

reference the following for command line:
	https://docs.mongodb.com/manual/reference/mongo-shell/

Deployed to Heroku 

	http://hidden-coast-1885.herokuapp.com/

	Important commands to remember

	git push heroku master
		
	Permission denied (publickey).
	fatal: Could not read from remote repository.

	Please make sure you have the correct access rights
	and the repository exists.

	Heroku is confused between RSA and GitHub Key

	ssh-keygen -t rsa

	Generating public/private rsa key pair.
	Enter file in which to save the key (/Users/.../.ssh/id_rsa): 
	Enter passphrase (empty for no passphrase): 
	Enter same passphrase again: 

	heroku keys:add

	Found the following SSH public keys:
	1) github_rsa.pub
	2) id_rsa.pub
	Which would you like to use with your Heroku account? 2

	Uploading SSH public key /Users/.../.ssh/id_rsa.pub... done
	
	Modified package.json {scripts} and app.js start variable for node.js
	
	git add -A
	git commit -m ""
	git push origin master
	git push heroku master

	heroku open
	heroku status
	heroku logs
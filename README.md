# gitOrderOfOperations

- branch from dev
	- git checkout -b feature
- work for feature gets in feature branch
- save changes
	- git add .
		- adds all changed files to staging, ready to commit
	- git commit -m "message goes here, present tense"
		- saves these changes to our local version of the branch
	- git push
		- sends the new version to remote
- WHEN READY TO MOVE TO DEV
	- save changes
	- git checkout dev
		- move back to dev branch
	- git pull
		- brings latest remote version of dev onto our machine
	- git checkout feature
		- moves back to feature branch
	- git merge dev
		- grabs dev, pastes into feature
		- if conflicts, fix in feature branch
	- COMMUNICATE INTENT
	- from feature branch
		- git push
			- sends our up to date, ready to merge code to remote
	- pull request from feature to dev
		- BASE: bth1994's dev
		- COMPARE: feature
  - these changes are now in dev. to get these on your machine, you must
  - git checkout dev
    - change to dev branch
  - git pull
    - pull remote dev into your local dev

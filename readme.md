Better way for blog management

Requirements:
Https support should be inbuilt
Should be static
Framework to create the static pages should be in python
Possibility to build automatically from github / bitbucket
Possibility to link more tools

Let’s try firebase
https://firebase.google.com/
Create a project - xxx
https://firebase.google.com/docs/hosting/?authuser=0#implementation_path
Install the CLI
Create a directory: ~/firebase
firebase init
firebase serve
firebase deploy
Jekyll - https://chris.banes.me/2017/06/02/jekyll-firebase/
Install Ruby first
Then, sudo gem install jekyll bundler
Inside the firebase folder, sudo jekyll new blog
You may have to sudo chown -R ashwin
If you have wordpress blog already, export the xml file
Then sudo gem install jekyll-import
Import the wordpress file (https://jekyllrb.com/docs/migrations/)
Test out: bundle exec jekyll serve
Before deploy, jekyll build
Now, change the firebase.json file so that we point to blog/_site
Deploy and you are done.
Further improvements can be done by modifying theme etc.
Domain can now be redirected here.
During domain verification, TXT record propogation takes a lot of time.
CNAME method may also be used for verification (through appengine console)
If domain registrar has issues, move domain to google domains to simplify everything
Now, in firebase just select the custom domain and it is done.
Save everything to git.

https://css-tricks.com/building-a-jekyll-site-part-1-of-3/
https://ines.io/blog/the-ultimate-guide-static-websites-jekyll



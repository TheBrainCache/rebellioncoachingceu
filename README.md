# rebellioncoachingceu

Open Azure Cloud Shell

Looks like no need to run this since its already been run: 
matt@Azure:~$ git clone https://github.com/TheBrainCache/rebellioncoachingceu.git 
fatal: destination path 'rebellioncoaching_public' already exists and is not an empty directory.

Tell Git who you are...maybe only necessary to do once?? 
git config --global user.email "matt@thebraincache.com" 
git config --global user.name "Matt Schilb"

cd rebellioncoachingceu

matt@Azure:/rebellioncoaching_public$ ls 
index.html README.md rebellioncoaching_public 

matt@Azure:/rebellioncoaching_public$

git init git add . git commit -m "trying to get v2 to show"

az webapp deployment source config-local-git --name rebellioncoaching --resource-group MS_THEBRAINCACHE_RESOURCE_GROUP

az webapp deployment list-publishing-credentials --name rebellioncoaching --resource-group MS_THEBRAINCACHE_RESOURCE_GROUP

matt@Azure:~/rebellioncoaching_public$ git remote add azure 'https://$rebellioncoaching:dp4pfD8Tz1WFvdn6uzbvrtBlx9pAT3BnglNll669HcBNdbBacvn5PlRax1cS@rebellioncoaching.scm.azurewebsites.net' fatal: remote azure already exists.

matt@Azure:~/rebellioncoaching_public$ git push azure master error: src refspec master does not match any. error: failed to push some refs to 'https://$rebellioncoaching:dp4pfD8Tz1WFvdn6uzbvrtBlx9pAT3BnglNll669HcBNdbBacvn5PlRax1cS@rebellioncoaching.scm.azurewebsites.net'

One command az webapp up --name rebellioncoaching-now --html

This did create a new page, but it does not show the changes that I have in index

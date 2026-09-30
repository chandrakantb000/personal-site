#website #fix #folder #quartz #live #domain #hosting #tech

## Earlier setup, issue and resolution
So earlier few days ago I had setup this site and deployed through github pages. Website was live through pages but it had this issue of the blogs present in folders not showing in site. Thanks to Sarang for assisting me with fixing this error. It was due to incorrect baseurl set in quartz config file. 

## Getting a domain and making website live
Getting domain and was quite easy due to Namecheap, just buy the domain little bit setup(on namecheap go to Domain List > select your domain > manage > advanced DNS > create A records and a CNAME record as below, check this [github doc](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site) for this)

![[namecheap configuration.png]]

And then go to github > website_repo > settings > pages > custom domain(here add your domain) it will take some time so take a 🍵break.
Congratulations your site will be live now.
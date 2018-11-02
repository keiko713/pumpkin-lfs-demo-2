# pumpkin-lfs-demo

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/keiko713/pumpkin-lfs-demo)

1. click above Deploy to Netlify button!
   - this will fork the repo and create the Netlify site
2. clone the created repo to the local env
3. with the local cloned repo dir, run `netlify init`
   - this will create a new Netlify site with this repo
4. provision netlify lfs addon: `netlify addons:create netlify-lfs-staging`
5. setup the lfs! run: `netlify lfs:setup`
   - you may be scolded if you don't have the lfs installed in your laptop
   - this example has two jpg images, so specify `*.jpg` with `Specify which files you want to track (optional)` question
6. run `git commit -am 'Enable Netlify LFS feature'`
7. run `git push origin master`
   - this will trigger the automatic deploy!
8. checkout the site! it should be using LFS. I hope.

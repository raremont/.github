# How to use private NPM packages
1. Create a file under `~/.npmrc` and paste the following:
   - ```ini
     @raremont:registry=https://npm.pkg.github.com
     //npm.pkg.github.com/:_authToken=<YOUR_AUTH_TOKEN>
     ``` 
1. Change `<YOUR_AUTH_TOKEN>` to your private token. You can get it [here](https://github.com/settings/tokens).
2. Install packages normally.
   - E.g.: `npm install @raremont/raremont-utility@1.0.0`
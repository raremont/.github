# **Creating new packages**
1. ### Use [this link](https://github.com/raremont/raremont-npm-package-template/generate) to create a new package from template.
1. ### Update `package.json` with your repo name
1. Write and push your code.
1. Create a release from the GitHub UI - this will generate a npm package. See [Creating a release](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository#creating-a-release) for more details.
> **REMEMBER:** Generate `package-lock.json` with `npm install`, commit and push it ***before*** creating a release.
   ---
   
# How to use private NPM packages
1. Create a file under `~/.npmrc` and paste the following:
   - ```ini
     @raremont:registry=https://npm.pkg.github.com
     //npm.pkg.github.com/:_authToken=<YOUR_AUTH_TOKEN>
     ``` 
1. Change `<YOUR_AUTH_TOKEN>` to your private token. You can get it [here](https://github.com/settings/tokens).
2. Install packages normally.
   - E.g.: `npm install @raremont/raremont-utility@1.0.0`

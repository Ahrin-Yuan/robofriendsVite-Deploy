# robofriendsVite-Deploy
Deploying React v19 + Vite
To run the project: 

1. Clone this repo
2. Run `npm install`
3. Run `npm run dev`

# How to Upload Vite Project into Github?
## 1. Create your Repository Name > Public > Create Repository
## 2. Github will give you code:
"…or create a new repository on the command line
echo "# robofriendsVite-Deploy" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/Ahrin-Yuan/robofriendsVite-Deploy.git
git push -u origin main"

## 3. In your already created Vite Project folder, Run `git init` in your Terminal. .git folder will appear in your Vite Project folder.

## 4. Then just run the following given code in your terminal :
`git add .`
`git commit -m "first commit"`
`git branch -M main`
`git remote add origin https://github.com/Ahrin-Yuan/robofriendsVite-Deploy.git`
`git push -u origin main"`



# Setting gh-pages
run `npm install gh-pages --s
ave-dev`

# SideNote (Don't Forget):
### Add "Base" in *vite.config.js*
// https://vite.dev/config/
export default defineConfig({
  plugins: [react()],
  `base: '/robofriendsVite-Deploy/'`
})

### Update *package.json*:
{
`"homepage": "https://{username}.github.io/{repo-name}/"`
...

"scripts": {
    `"predeploy" : "npm run build",`
    `"deploy" : "gh-pages -d dist",`
    ...
}


## 5. run this in your terminal:
`git add .`
`git commit -m ""`
`git push`


## 6. Run Deploy Command
run `npm run deploy` - filling up gh-pages branch with our project files information (gh-pages allows our website to be publicly displayed)
- see the word "Published"

## 7. Settings > Source:gh-pages /(root)
Now have live URL provided.
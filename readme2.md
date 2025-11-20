# flask-vercel

### Flask app name: flask-vercel-1

This repo is to test the deployment to Vercel

## Test local

```
Mac:
- virtualenv ~/.ve/vercelo
- source ~/.ve/vercelo/bin/activate
- (to deactivate) : deactivate

(or)
 - in pip of a specific Python version (Mac):
- - python3.8 -m venv env
- - source env/bin/activate
- - jupyter notebook
- - deactivate

Windows:
- virtualenv ~/.ve/vercelo
- ~\.ve\vercelo\bin\activate

Most important commands to run the project:
- - pip install -r requirements.txt
- - FLASK_APP=flask_app.py flask run


# 🚀 go to http://localhost:5000
```

## Push to github and Deploy to vercel

- Create an account at https://vercel.com/
- Install the Vercel CLI: `npm i -g vercel`
  (Note):
  In case of this error: "Another git process seems to be running in this repository", run the below command:
- rm -f .git/index.lock

- Mac:
  - git add . && git commit -m "Changes" && git push origin main
- Windows:
  - git add . ; git commit -m "Changes" ; git push origin main
- Then, inside your repo folder, run `vercel`.

```
For the first time:

(vercel) ➜  flask-vercel$ vercel
Vercel CLI 23.0.1
? Set up and deploy “~/workspace/workon/flask-vercel”? [Y/n] y
? Which scope do you want to deploy to? your-vercel-account
? Link to existing project? [y/N] n
? What’s your project’s name? flask-vercel-1
? In which directory is your code located? ./
...
```


Done! You should access your very simple flask app running on Vercel

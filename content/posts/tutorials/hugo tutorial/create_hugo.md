---
title: "Create Hugo Toha Project"
date: 2020-06-08T08:06:25+06:00
description: Create Hugo Project
menu:
  sidebar:
    name: Create Hugo Project
    identifier: create hugo
    parent: hugo
    weight: 40
hero: boat.jpg
mermaid: true
---

# Build a Hugo Toha project

* https://toha-guides.netlify.app/posts/quickstart/#disable-news-letter-functionality

## Step 1: Fork the example repo and rename
At first, fork this sample repo to your account. Then, rename the repo to whatever you want. If you want to use Github Pages to deploy your site, then rename it to <your username>.github.io. The sample repo comes with pre-configured Github Actions to publish the site in Github Pages and Netlify.

## Step 2: Clone the forked repo locally
Once you have forked and renamed the repository, you can now clone the forked repository in your local machine for further changes.

git clone https://github.com/<>your username<>/<>forked repo name<>

## Step 3: Update the module file
You should see `go.mod` files in the root of the repository. Update the first line of the go.mod file as below:

module github.com/<>your username<>/<>forked repo name<>

## Step 4: Change config.yaml file
Now, open the repository in an editor and change the following configurations in your `config.yaml` file located at the root of your repository.

### Change the baseURL
At first change the baseURL to your site URL. If you want to use Github Pages to host your site, then set it as below:

baseURL: https://<>your username<>.github.io

### Change the gitRepo

Now, change the gitRepo field under the params section to point to your forked repository. For example,

gitRepo: https://github.com/<>your username<>/<>your forked repo name<>

## Step 5: Run the site locally

Now, run the following commands to run your site locally:

### a. Load Hugo modules

hugo mod tidy

### b. Install node modules

hugo mod npm pack

npm install

### c. Run the site

hugo server -w

## Step 6: Push the changes to Github

If you have come this far, it means your site is running locally without any issue. Let’s push these changes to Github.

**stage all the changes**

git add .

**commit the changes**

git commit -m "Initial site setup"

git remote add origin https://github.com/Marcos14Almeida/mrcmarc.github.io.git

git push -u origin main

**Public folder**

In order to see the page, create a `gh-pages` branch on github and upload just the `public` folder to it. In order to do it create a git inside this folder. On the `main` branch you can save the project as a whole. In order to save it correctly, alway run the commands:

hugo

hugo server

The command hugo you redo the folder public. If the pages are correctly displayed with hugo server then upload the changes to github `gh-pages` branch with the commands (considering you are in the terminal in the project root):

cd public

git add .

git commit -m "Initial site setup"

git remote add origin https://github.com/Marcos14Almeida/mrcmarc.github.io.git

git branch gh-pages # Just if you don't have the branch yet

git checkout gh-pages # Just if you don't have the branch yet

git push -u origin gh-pages

### Images

The images should be placed in a folder inside the `content` then you call it using html for example:

img src="/mrcmarc/posts/projects/images/chat.png" alt="chat" style="width: 30%; margin: 10px;"

In this case the blog is Marcos.github.io/mrcmarc. But the source is always .github.io. Because of that the images should be referenced starting from this point. Then the image is located inside /contents/posts..., so you just need to connect the 2 parts. If your site is just `name.github.io` you would reference it as /posts/project_folder/image_folder/image_name.jpg.

If the image doesn't appear check the baseURL or the gitRepo of the `config.yaml`. Probabaly one of those two references are wrong.

--------------------------------------------------------------


# Catch of the day - React app

This repo will hold the Catch of the Day app, as well as personal notes while progressing into the course.

-The Catch of the day app is part of the online course: React For Beginners by Wes Bos — [ReactForBeginners.com](https://ReactForBeginners.com)

- Starter files for the React For Beginners course by Wes Bos can be found [here](https://github.com/wesbos/React-For-Beginners-Starter-Files).


## To Start

**Note** - One of the dependencies is Xcode. While installing, if you run into an error that says, `gyp: No Xcode or CLT version detected!` please do the following:
1. Execute `xcode-select --install` in terminal.
2. Delete the "node_modules" folder located within the "catch-of-the-day" folder.
3. Execute `npm install` once more.

`cd` into `catch-of-the-day` and follow along with the videos

### Code Use

You are welcome to use this code in your own applications. If you would like to use it for training purposes, please contact Wes Bos first to make sure it's okay.

# Firebase Frequently Asked Questions

#### :question: I get `permission_denied` warnings in my console when setting up Firebase

Be sure to select "Realtime database" as as your database type inside Firebase. If you created your database as a Cloud Firestore type, you can change it in the Database tab.

#### :question: I can't log in to the store after I deployed to Netlify/Apache

Firebase by default only allows logins from localhost or the Firebase website. You'll need to add your deploy URL to the Authorized Domains in the Sign-in method area of your Firebase console.

## Changes In the 2018 RE-Record

In March 2018 Wes Bos re-recorded this course. Here are the things that have been updated.

* Upgrade to React Router 4 Final API
* Use React 16.3
* Move to external PropTypes Package
* Use React's new Refs API, remove function refs
* Remove all use of constructors and super() - use class properties instead
* Better explain binding, use of `this` and component instances
* Moved from React-addons-css-transition-group to react-transition-group and upgraded from 1.x to 2.x
* Use official Firebase package for Auth as re-base is now only for data binding
* Move promise based code to async/await
* Show how to return multiple elements with React.Fragment

## htaccess

Here is the .htaccess file we use in the apache deployment video

```
RewriteBase /
RewriteRule ^index\.html$ - [L]
RewriteCond %{REQUEST_FILENAME} !-f
RewriteCond %{REQUEST_FILENAME} !-d
RewriteRule . /index.html [L]
```

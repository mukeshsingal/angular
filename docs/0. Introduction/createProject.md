
TO create new Project user 
```node
ng new project-name 
```

Structure of project: 

`e2e`: the end to end test, which simulates a real user, so we can write code to launch the browser, navigate to the home page of an application, click few links here and there, fill the form and then the assert to get the result. 

`node_modules`: third-party libraries

`src`: source code of an application
    - `app`: which contains modules and components 
    - `assets`: to store static assets of application (image, text, icons)
    - `environment`- configuration settings for different environments
        - `envirnoment.prod.ts` for prodcutoon 
        - `envirnoment.ts` for dev envirnoment
    - `favicon.ico` - icon displayed in browser 
    - `index.html` - homepages of application 
    - `main.ts` - stating point of application
    - `polyfills.ts` - script to import scrips which is required to run angular 
    - `style.css` - global css styles
    - `test.ts` - used to create testing envirnoment 

`.angular-cli.json`: angular cli json

`karma.conf.js` - config for karma, which is testrunner for JS

`package.json` - node packages configuratio files

`protractor.conf.js` - tool to run e2e test for angular

`tsconfig.json` - setting for TypeScript compiler 

`tslint.json` - sca tool for angular 

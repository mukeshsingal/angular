Angular Cli uses Webpack which is build automation tool
gets all our script, compile and create bundles and minify them. 
 
 1) pollyfills.bundle.js - js which is supported by all browsers 
 2) main.bundle.js - whcih is all souce code
 3) style.bundle.js - all styles 
 4) vendor.bundle.js - all thrid party libraries.

 Whenever there are any changes in any source code Webpack compile and create new bundles, so the user doesn't have to. Also, Webpack refreshes your browser.
 This is called Hot Module Replacement(HMR).
# Tailwind CSS with Meteor 2.7 Release Test

There is an issue with Meteor 2.7 release that has to do with the work done to get Tailwind CSS to work with Meteor.

This is a simple project that setups up Meteor with Svelte and Tailwind CSS.

The following error occurs on Windows 11:
```
=> Started proxy.
=> Started HMR server.
=> Errors prevented startup:

   While minifying app stylesheet:
   app/client/main.css: TypeError: Cannot read property 'uid' of undefined
   at Object.statSync
   (C:\Users\Lenovo\AppData\Local\.meteor\packages\meteor-tool\2.7.0\mt-os.windows.x86_64\dev_bundle\lib\node_modules\npm\node_modules\graceful-fs\polyfills.js:309:17)
   at trackModified
   (D:\MeteorProjects\test-tailwind\node_modules\tailwindcss\lib\lib\setupContextUtils.js:468:46)    
   at Object.getContext
   (D:\MeteorProjects\test-tailwind\node_modules\tailwindcss\lib\lib\setupContextUtils.js:867:5)     
   at
   D:\MeteorProjects\test-tailwind\node_modules\tailwindcss\lib\lib\setupTrackingContext.js:142:53   
   at
   D:\MeteorProjects\test-tailwind\node_modules\tailwindcss\lib\processTailwindFeatures.js:43:11     
   at plugins
   (D:\MeteorProjects\test-tailwind\node_modules\tailwindcss\lib\index.js:20:104)
   at LazyResult.runOnRoot
   (D:\MeteorProjects\test-tailwind\node_modules\postcss\lib\lazy-result.js:339:16)
   at LazyResult.runAsync
   (D:\MeteorProjects\test-tailwind\node_modules\postcss\lib\lazy-result.js:393:26)
   at LazyResult.async
   (D:\MeteorProjects\test-tailwind\node_modules\postcss\lib\lazy-result.js:221:30)
   at LazyResult.then
   (D:\MeteorProjects\test-tailwind\node_modules\postcss\lib\lazy-result.js:206:17)
   => awaited here:
   at Function.Promise.await
   (C:\Users\Lenovo\AppData\Local\.meteor\packages\meteor-tool\2.7.0\mt-os.windows.x86_64\dev_bundle\lib\node_modules\meteor-promise\promise_server.js:56:12)
   at packages/minifyStdCSS/plugin/minify-css.js:127:21
   at
   C:\Users\Lenovo\AppData\Local\.meteor\packages\meteor-tool\2.7.0\mt-os.windows.x86_64\dev_bundle\lib\node_modules\meteor-promise\fiber_pool.js:43:40

=> Your application has errors. Waiting for file change.
=> Started MongoDB.
```
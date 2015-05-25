# grunt-livereload-express
when we need to livereload files that are not static but are templates with an express server, the livereload method is a little different for both front-end and back-end needs to be watched

------
##plugins
* [grunt-contrib-watch](https://github.com/gruntjs/grunt-contrib-watch)
* [grunt-express-server](https://github.com/ericclemmons/grunt-express-server)
* [load-grunt-tasks](https://github.com/sindresorhus/load-grunt-tasks)


##Tips:
* Do not registe Task for the loaded plugins, which will make it unusable
* in the path, there is no '/' at the beginning.
* to enable livereload, a [livereload plugin](https://chrome.google.com/webstore/detail/livereload/jnihajbhpnppcggbcgedagnkighmdlei) of the browser is needed and make sure it is switched on(the center circle of the icon be filled).
* when using swig as the template engine for the express, swig will cache the template so we have to restart the server to see the changes in html files. This makes the grunt tasks don't work. Refer to this [link](https://github.com/helicese/grunt-livereload-express/), we disallow the cache in swig so the grunt tasks work well.


##references:
* [http://anthonydel.com/my-personal-gruntfile-for-front-end-experiments/](http://anthonydel.com/my-personal-gruntfile-for-front-end-experiments/)
* [http://thanpol.as/grunt/Grunt-with-express-server-and-Livereload/](http://thanpol.as/grunt/Grunt-with-express-server-and-Livereload/)
* [http://rhumaric.com/2013/07/renewing-the-grunt-livereload-magic/](http://rhumaric.com/2013/07/renewing-the-grunt-livereload-magic/)

------
helicese@gmail.com

# grunt-simple_server

A trivial grunt task which will run a web server
to serve the content in a single directory. No frills.

# Usage

Configure in grunt.initConfig(), e.g.

    grunt.initConfig({
      simple_server: {
        // directory containing the app you want to serve
        dir: 'app',

        // optional; default is 20202
        port: 7891,

        // optional; callback function to do something with the config
        callback: function (config) {
          // receives the simple_server config once the server is started
        }
      }
    });

Note that this task blocks until you manually kill it with Ctrl-C.

# Licence

This code is extracted from the webapps-slider-puzzle project, to make
it easier to reuse in other projects (I've been copying and pasting it
between projects for months):

https://github.com/01org/webapps-slider-puzzle/blob/master/tools/grunt-tasks/grunt-simple_server.js

It is released under the same licence: Apache v2

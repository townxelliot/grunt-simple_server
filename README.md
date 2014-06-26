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

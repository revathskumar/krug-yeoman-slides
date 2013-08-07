
#Gruntfile . js
```
      module.exports = function(grunt) {
        grunt.initConfig({
          uglify: {
            dist: {
                files: {
                    "dist/scripts/app.js": "app/scripts/*.js"
                }
            }
          },
          clean: ['dist/*'],
        });

        grunt.loadNpmTasks("grunt-contrib-uglify");
        grunt.loadNpmTasks("grunt-contrib-clean");

        grunt.registerTask('build', ['clean', 'uglify']);
      }
```

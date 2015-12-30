# gulp-angular2-embed-sass
A gulp plugin to compile styleUrls with sass to css and include them as strings under style.

Needs massive cleanup, refactorization, options, source-maps, and docs, but it works! Pull requests are welcome.

## Example
```
npm install gulp-angular2-embed-sass --save-dev
````
In your gulpfile.js:
```
var gulp      = require('gulp');
var embedSass = require('gulp-angular2-embed-sass');

gulp.task('embedSass', function() {
    gulp.src('targetPath')
        .pipe(embedSass())
        .pipe(gulp.dest('destinationPath'));
});
```

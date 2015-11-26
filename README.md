# Gulp - VS Code

## Quickstart

1. Install Via [Package Control] `vscode-gulp`
2. Open your repo containing either a `gulpfile.js` file or directory

## Installation

### via PackageControl
If you have [PackageControl](http://wbond.net/sublime_packages/package_control) installed, you can use it to install the package.

Just type `cmd-shift-p`/`ctrl-shift-p` to bring up the command pallete and pick `Package Control: Install Package` from the dropdown, search and select the package there and you're all set.

## Snippets

#### gulpvar
```
var gulp = require('gulp-name');
```

#### pipe | gulppipe
```
.pipe(name('file'))
```

#### gulpsrc - [Docs](https://github.com/gulpjs/gulp/blob/master/docs/API.md#gulpsrcglobs-options)
```
gulp.src('scriptFiles')
  .pipe(name('file'))
```

#### gulptask - [Docs](https://github.com/gulpjs/gulp/blob/master/docs/API.md#gulptaskname-deps-fn)
```
gulp.task('name',['tasks'], function() {
    // content
});
```

#### gulpdest - [Docs](https://github.com/gulpjs/gulp/blob/master/docs/API.md#gulpdestpath)
```
.pipe(gulp.dest('folder'));
```

#### gulpwatch - [Docs](https://github.com/gulpjs/gulp/blob/master/docs/API.md#gulpwatchglob-opts-tasks)
```
gulp.watch('file', ['tasks']);
```

#### gulpwcb - [Docs](https://github.com/gulpjs/gulp/blob/master/docs/API.md#gulpwatchglob-opts-cb)
```
gulp.watch('file', function(event) {
  console.log(' File '+event.path+' was '+event.type+', running tasks...');
});
```
** Enjoy!**
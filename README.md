# folder-diff

make diff between two folder or zip, gen patch file what describe the difference of folders

support Asynchronous
support bsdiff

## install 

```shell
npm install node-folder-diff
```

## api

```javascript
var diff = require('node-folder-diff');
diff.diff(old_folder_path, new_folder_path, {bsdiff : true}).then(function(archive){
	var output = fs.createWriteStream(...);
    archive.pipe(output);
});
```
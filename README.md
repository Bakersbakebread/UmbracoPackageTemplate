# UmbracoPackageTemplate

A custom dotnet new template for creating Umbraco packages. It is based on the official umbraco package template, with some extra abilities added in - a lot of the code/inspiration is taken from https://github.com/KevinJump/Our.Umbraco.BackOfficeThemes where the use of gulp made development quick and easy.


## Setup and use

Clone down the template into any directory you like.

Install the new template by running:
```
dotnet new --install A:\Path\To\Folder\
```

Create your package template in a directory of your choice, it defaults to the directory name if you don't pass the `-n` flag.
```
 dotnet new umbpackage -n MyCoolPackageName
```

Open the folder in a terminal and install the required node_modules
```
cd MyCoolPackageName
npm install
```

Run the gulpfile to watch for changes.
```
>> A:\Path\To\Folder\MyCoolPackageName

gulp
```

Any changes made to the files in `MyCoolPackageName/App_Plugins` are moved into your `MyCoolPackageName.Site/App_Plugins` folder automatically! 

Magic!


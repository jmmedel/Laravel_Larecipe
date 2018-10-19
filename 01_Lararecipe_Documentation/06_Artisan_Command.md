

Artisan Commands
LaRecipe comes with helpful Artisan commands that can be triggered to handle boring stuff out of the box.

Install Command
Docs Command

Install Command
After requiring the package via composer, all you have to do is to run single command which will take care of publishing the needed assets and configurations.

php artisan larecipe:install
After running the command you will find few changes in your Laravel app folders, larecipe.php config file will be added to config directory and the basic setup for writing documentation will be added to the resources/docs directory. That happened internally by calling larecipe:docs command inside larecipe:install command.

This structure is based on the default path of the docs. Yours will be different if you change the docs path.

.
├─ config
│  └─ larecipe.php
└─ resources
   └─ docs
      └─ 1.0
         │─ index.md
         └─ overview.md

Docs Command
This command is a bit complicated than larecipe:install command. However, all you have to know is the behavior of this command and what you expect from it.

php artisan larecipe:docs
The workflow of this command is described as follow:

1. LaRecipe will read the published versions array in your config/larecipe.
2. For each published version, LaRecipe will create the corresponding version directory if not exists.
3. After creating the directory, LaRecipe will create index.md for the given version if not exists.
4. Finally, LaRecipe will create overview.md for the given version if not exists.


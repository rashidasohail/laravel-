# laravel-

**1.** PS C:\xampp\htdocs\laravel_project> php artisan
**Could not open input file: artisan**

**Solution :** https://www.youtube.com/watch?v=lqaV929F-jc
PS C:\xampp\htdocs\laravel_project> cd .\first-project\    
PS C:\xampp\htdocs\laravel_project\first-project> php artisan serve
  forking is not supported on this platform

   INFO  Server running on [http://127.0.0.1:8000].


**2.** npm : The term 'npm' is not recognized as the name of a cmdlet, function, script file, or operable program. Check the spelling of the name, or if  
a path was included, verify that the path is correct and try again.
At line:1 char:1
+ npm install
+ ~~~
    + CategoryInfo          : ObjectNotFound: (npm:String) [], CommandNotFoundException

**Solution :**

1.https://youtu.be/n6BzliZA_R0?si=YXTzeJci6aFyUl7j
2.If npm folder doesn't exist inside Roaming directory,then follow the steps in https://stackoverflow.com/a/77159276/23458473

**3.** npm : File C:\Program Files\nodejs\npm.ps1 cannot be loaded because running scripts is disabled on this system. For more information, see 
about_Execution_Policies at https:/go.microsoft.com/fwlink/?LinkID=135170.
At line:1 char:1
+ npm install
+ ~~~
    + FullyQualifiedErrorId : UnauthorizedAccess

**Solution :** https://youtu.be/q5iDjNR1O7Y?si=Q_SlQGBP8-WhCtH6

**4.** Database file at path [sample-db] does not exist. Ensure this is an absolute path to the database. (Connection: sqlite, SQL: select * from "sessions" where "id" = itlJlaUicvVkmM3PuxOJT6GnPPUtolqbRqIZAfEk limit 1)

**Solution :** if you are using laravel 11 just change the session-driver in .env file from
        SESSION_DRIVER=database
        
        to
        
        SESSION_DRIVER=file

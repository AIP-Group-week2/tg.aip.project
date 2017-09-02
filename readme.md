<p>LARAVEL V5.4 Developer note - Project TechGorilla Alpha v0.2</p>
<p>TechGorilla Team: Fulun He, Qiaozhi Lu and Xiaohan Wang.</p></font>

#TechGorilla developer notes#
-----------------------------------------------------------------------------------------------------------------------------------
->Coding convention - v1.0 

-Environment Laravel 5.4, PHP >= 7.0.0 OpenSSL PHP Extension, PDO PHP Extension, Mbstring PHP Extension, Tokenizer PHP Extension, XML PHP Extension

-Variables are in camelCase such as getName, getEmailAdd etc.

-Comment on every function.

-Developers must comment any of updates and changes.

-Functions and parameters:Avoid passing huge numbers of parameters to functions or constructors.

-Using assignment as an expression is surprising to the reader and looks like an error. Do not write code like this:
if ( $a = foo() ) {
    bar();
}

-Use <https://> instead of <http://> or <//> when omitting the protocols.

-Put different resources into specific category folders. E.g. pictures must go <pic> folder.
	
-All folders and file names must use lower case letters.

-Integrate css and other style sheets into one as much as possible to reduce the costs when update.

-Developers must backup the original copy of the project. And keep it for at least 14 days.

-Codes with core functions must stored in specific folders. Only global files can be stored on the root (resources/views/).

-The class namespace declaration must be on the same line as <?php.

-A class' opening { must be on the same line as the class name.

-Functions and control structures must use Allman style braces.

-Indent with tabs, align with spaces.
*last update: 3/9/2017







-----------------------------------------------------------------------------------------------------------------------------------
->Installing guidance for local enviornment 

Running this project requires MySQL server and Composer installed.
1. Apply <b>composer update</b> at the root of the project folder on terminal after download.
2. Edit and change database connection configs at .env and config/database.php files. Keep all the database config same with yours. <b>example.env.example</b> -> <b>.env</b>
3. Generate your communication key on terminal: <b>php artisan key:generate</b>
4. Execute data migration on terminal: <b>php artisan migrate</b>. (Please be aware that this can be done after you successfully make connection with your local database.)
5. Test database migration: <b>php artisan db:seed</b>
6. Use admin@admin.com for email address and <b>111111</b> for password for admin login.

#TechGorilla developer notes#

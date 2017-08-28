LARAVEL V5.4 Developer note - Project TechGorilla Alpha v0.2

TechGorilla Team: Fulun He, Qiaozhi Lu and Xiaohan Wang.

#TechGorilla developer notes#

->Coding convention - v1.0

-Variables are in camelCase such as getName, getEmailAdd etc.

-Comment on every function.

-Developers must comment any of updates and changes.

-Use https:// instead of http:// or <//> when omitting the protocols.

-Put different resources into specific category folders. E.g. pictures must go folder.

-All folders and file names must use lower case letters.

-Integrate css and other style sheets into one as much as possible to reduce the costs when update.

-Developers must backup the original copy of the project. And keep it for at least 14 days.

-Codes with core functions must stored in specific folders. Only global files can be stored on the root (resources/views/). *last update: 27/8/2017

->Installing guidance for local enviornment

Running this project requires MySQL server and Composer installed.

Apply composer update at the root of the project folder on terminal after download.
Edit and change database connection configs at .env and config/database.php files. Keep all the database config same with yours. example.env.example -> .env
Generate your communication key on terminal: php artisan key:generate
Execute data migration on terminal: php artisan migrate. (Please be aware that this can be done after you successfully make connection with your local database.)
Test database migration: php artisan db:seed
Use admin@admin.com for email address and 111111 for password for admin login.
#TechGorilla developer notes#

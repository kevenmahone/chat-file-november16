upload into /var/www/html/mybb/chat/ the file from chat folder chmod 777 to everything upload the plugin inside mybb plugin place

edit in chat folder the config file to add your database - username - password ... Can be the same as the forum.

about the request_limiter.php.txt in the server remove the .txt at the end .. be sure is only .php and put it in plugin .. activate from admin panel plugin .. this request limiter and is working need to be tested if each member can do their own request and have each a limit individual .. not a shared limit..


for the limit 20 request per min in the chat.. open chat.php file 
find : define('MAX_REQUESTS_PER_MINUTE', 20);

and replace 20 by the number of request you want per min into the chat. Its need to be tested if is working for all user in the chat. and if 1 user have a message to wait if the other user will not have this message ... 




-

-
-
-
-
-
-
working chat file provided by the programer

install mybb forum and php dependency for nginx.

if during the install of the chat when loading the chat.php page .. example .onionsite/chat/chat.php if we have a white page Verify the var/log/nginx/error.log file .. if is say because of the helper module is probably because is missing this to be installed:

sudo apt-get install php-intl

this is a part of php install : sudo apt install -y php8.2 php8.2-cli php8.2-fpm php8.2-gd php8.2-mbstring php8.2-xml php8.2-mysql php8.2-pgsql

actually in 2025 nov is php 8.2 who is installed.

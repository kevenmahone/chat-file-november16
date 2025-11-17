upload into /var/www/html/mybb/chat/ the file from chat folder chmod 777 to everything upload the plugin inside mybb plugin place

edit in chat folder the config file to add your database - username - password ... Can be the same as the forum.

about the request_limiter.php.txt in the server remove the .txt at the end .. be sure is only .php and put it in plugin .. activate from admin panel plugin .. this request limiter and is working need to be tested if each member can do their own request and have each a limit individual .. not a shared limit..


for the limit 20 request per min in the chat.. open chat.php file 
find : define('MAX_REQUESTS_PER_MINUTE', 20);

and replace 20 by the number of request you want per min into the chat. Its need to be tested if is working for all user in the chat. and if 1 user have a message to wait if the other user will not have this message ... 

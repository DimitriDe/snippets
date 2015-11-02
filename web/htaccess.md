# Htaccess Tips

Redirect non-www to www

    RewriteEngine On
    RewriteCond %{HTTP_HOST} !^wwww\.
    RewriteRule ^(.*)$ http://www.%{HTTP_HOST}/$1 [R=301,L]

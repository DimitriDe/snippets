# Htaccess Tips

Redirect non-www to www

    RewriteEngine On
    RewriteCond %{HTTP_HOST} !^www\.
    RewriteRule ^(.*)$ http://www.%{HTTP_HOST}/$1 [R=301,L]

Cache static assets : pages, images, styles and scripts

    <IfModule mod_expires.c>
    	ExpiresActive On
    	ExpiresDefault "access plus 7200 seconds"
    	ExpiresByType image/jpg 			"access plus 1 week"
    	ExpiresByType image/jpeg 			"access plus 1 week"
    	ExpiresByType image/png 			"access plus 1 week"
    	ExpiresByType image/gif 			"access plus 1 week"
    	ExpiresByType image/svg+xml			"access plus 1 week"
    	ExpiresByType image/ico 			"access plus 1 week"
    	ExpiresByType image/icon 			"access plus 1 week"
    	ExpiresByType image/x-icon 			"access plus 1 week"
    	ExpiresByType text/css 				"access plus 1 week"
    	ExpiresByType text/javascript 		"access plus 1 week"
    	ExpiresByType text/html 			"access plus 7200 seconds"
    	ExpiresByType application/xhtml+xml 	"access plus 7200 seconds"
    	ExpiresByType application/javascript 	"access plus 1 week"
    	ExpiresByType application/x-javascript 	"access plus 1 week"
    	ExpiresByType application/x-shockwave-flash "access plus 1 week"
    </IfModule>


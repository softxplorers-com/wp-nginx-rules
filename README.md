location ~* /wp-includes/.*.php$ {
	deny all;
	access_log off;
	log_not_found off;
}

location ~* /wp-content/.*.php$ {
	deny all;
	access_log off;
	log_not_found off;
}

location ~* /(?:uploads|files)/.*.php$ {
	deny all;
	access_log off;
	log_not_found off;
}

location = /xmlrpc.php {
	deny all;
	access_log off;
	log_not_found off;
}

location ~ /\.git {
  deny all;
}

location ~ /\.ht {
        deny all;
}

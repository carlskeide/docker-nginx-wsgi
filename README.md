# Nginx as a WSGI proxy

Routes most incoming HTTP requests to `wsgi://wsgi-app:3031/`, except for `/static` and `/media` which are routed to their respective folders in `/srv/www` (where they can be overriden with app volumes).

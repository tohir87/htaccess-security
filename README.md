## Htaccess important headers (https://securityheaders.com/ - Security header scanner)

```
<IfModule mod_headers.c>
    Header set Content-Security-Policy "default-src 'self';"
    Header always set Referrer-Policy "same-origin"
    Header set X-XSS-Protection "1; mode=block"
    Header set X-Frame-Options "SAMEORIGIN"
    Header set X-Content-Type-Options "nosniff"
    Header always set Strict-Transport-Security "max-age=63072000; includeSubDomains"
    Header set Feature-Policy "geolocation 'self'; vibrate 'none'"
</IfModule>```




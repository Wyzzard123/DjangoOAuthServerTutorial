# README

Creating a Django OAuth server and an API protected by OAuth using the tutorials at https://django-oauth-toolkit.readthedocs.io/

## Howto
1. Note the consumer app in the tutorial is broken. Follow the instructions here instead: https://django-oauth-toolkit.readthedocs.io/en/latest/rest-framework/getting_started.html
    (Main difference is setting the grant type to "Authorization Grant Type: Resource owner password-based" instead of "authorization code".
  
   Then test the API with this curl:
   ``` 
   curl -X POST -d "grant_type=password&username=<user_name>&password=<password>" -u"<client_id>:<client_secret>" http://localhost:8000/o/token/
   ```

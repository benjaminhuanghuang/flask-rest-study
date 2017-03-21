https://blog.miguelgrinberg.com/post/designing-a-restful-api-with-python-and-flask

The easiest way to secure our web service is to require clients to provide a username and a password. 

In a regular web application you would have a login form that posts the credentials, and at that point the server 
would create a session for the logged in user to continue working, with the session id stored in a cookie in the 
client browser. 

Unfortunately doing that here would violate the stateless requirement of REST, so instead we have to ask clients 
to send their authentication information with every request they send to us.

HTTP provides two forms of authentication: Basic and Digest.

Use Flask-HTTPAuth: 
from flask_httpauth import HTTPBasicAuth

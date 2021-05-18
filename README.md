# Dockerized_flask
This a simple Dockerized Flask app with Gunicorn wsgi server and nginx as load balancer(round robin by default).

To run use -

docker-compose up --build -d --scale app=2

This will create 2 instances of the app and nginx will use round robin technique as deafult for load balancing.

App will run at 0.0.0.0:8084 

Container logs can be checked by -

docker logs [contaier_name] -f

# Company Landing Page

A professional and responsive company website
built using HTML5 and CSS3.

## Technologies
- HTML5
- CSS3
- Docker
- Nginx
- Jenkins
- AWS EC2

## Docker

The application uses the official Nginx Alpine
image to serve the static website.

## CI/CD Pipeline

Jenkins automates the following process:

1. Fetch source code from GitHub.
2. Build Docker image on the Build Server.
3. Push image to Docker Hub.
4. Connect to Deployment Server through SSH.
5. Pull the latest Docker image.
6. Deploy the updated website.

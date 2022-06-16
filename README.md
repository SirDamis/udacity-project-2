# Udagram Image Filtering Microservice

Udagram is a simple cloud application developed using NodeJS for the Udacity Cloud Engineering Nanodegree course. It allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering microservice.
3. [The Image Filtering Microservice](https://github.com/udacity/cloud-developer/tree/master/course-02/project/image-filter-starter-code), is a Node-Express application which runs a simple script to process images.

## Tasks

### Setup Node Environment

You'll need to create a new node server. Open a new terminal within the project directory and run:

1. Initialize a new project: 
```bash
npm i
```
2. Run the development server with 
``` bash
npm run dev
```

### Endpoints 

The application has two endpoints
- `/`
- `/filteredimage?image_url={{image url}}`

### Deploying your system

Create the artifact using
``` bash
npm run build
```

Application was deployed to Amazon Web Service Elastic BeanStalk using `eb init`  a new application and `eb create` a new environment to deploy the image-filter service! Changes pushed made using `eb deploy`.

## Project URL
- http://image-filter-starter-code-dev22222222222222222222.us-east-1.elasticbeanstalk.com/

- http://image-filter-starter-code-dev22222222222222222222.us-east-1.elasticbeanstalk.com/filteredimage?image_url=https://upload.wikimedia.org/wikipedia/commons/b/bd/Golden_tabby_and_white_kitten_n01.jpg


## To DO

### Refactor the course RESTapi

If you're feeling up to it, refactor the course RESTapi to make a request to your newly provisioned image server.

### Authentication

Prevent requests without valid authentication headers.
> !!NOTE if you choose to submit this, make sure to add the token to the postman collection and export the postman collection file to your submission so we can review!

### Custom Domain Name

Add your own domain name and have it point to the running services (try adding a subdomain name to point to the processing server)
> !NOTE: Domain names are not included in AWS’ free tier and will incur a cost.

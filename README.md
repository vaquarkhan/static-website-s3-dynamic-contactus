#### static-website-s3-dynamic-contactus
--------------------------------------------------------------------

- https://aws.amazon.com/blogs/architecture/create-dynamic-contact-forms-for-s3-static-websites-using-aws-lambda-amazon-api-gateway-and-amazon-ses/


--------------------------------------------------------------------


## Deploy angular app on S3 bucket

#### Step #1 — Create a new Angular app with the angular-cli
First of all, you need an Angular app (if you haven’t got any).
Install angular-cli with npm:

         npm install -g @angular/cli
      
After installation was successful create a new project:

         ng new cloud_project
         
This will install all dependencies, and everything you need (it takes a while).

Ok! We have a project. A new project folder was created, and contains all the files we need. We can now start our new app with:

     cd cloud_project
     ng serve

Visit your localhost:4200 in your browser. It’s working. Cool.

### Step #2 — Build your app
Angular CLI comes with Webpack module builder. Luckily we need exactly this. :) To build the app run this:

     ng build --prod --aot

After this, a new dist folder generated, which have the bundled files.

### Step #3— Use following steps to deploy app 

- https://dev.to/samueldaviddelacruz/how-to-host-your-static-web-app-on-aws-s3-in-10-steps-3kgp
- https://www.fullstackreact.com/articles/deploying-a-react-app-to-s3/
- https://medium.com/ovrsea/deploy-automatically-a-react-app-on-amazon-s3-iam-within-minutes-da6cb0096d55
- https://medium.com/@omgwtfmarc/deploying-create-react-app-to-s3-or-cloudfront-48dae4ce0af
- 
-------------------------------------------------------------------------------------------
### deploy your S3 + Cloudfront website with SSL from AWS at: 

- https://www.josephecombs.com/2018/03/05/how-to-make-an-AWS-S3-static-website-with-ssl
- https://medium.com/@sbuckpesch/setup-aws-s3-static-website-hosting-using-ssl-acm-34d41d32e394
- https://aws.amazon.com/blogs/aws/server-name-indication-sni-and-http-redirection-for-amazon-cloudfront/
- https://aws.amazon.com/blogs/aws/new-aws-certificate-manager-deploy-ssltls-based-apps-on-aws/
- https://aws.amazon.com/about-aws/whats-new/2014/03/05/amazon-cloudront-announces-sni-custom-ssl/

### Pricing custom SSL: http://aws.amazon.com/cloudfront/pricing/
#### Keep in mind, they are charging $600 / month. need to only pay $600 if you want a dedicated IP address. If you are happy to use SNI (which is not supported by older browsers), no extra charges apply 
- https://serverfault.com/questions/562262/how-can-i-use-https-with-aws-cloudfront-without-paying-600-to-upload-my-cert


- 

------------------------------------------------------------------------------------------
### Cost compare EBS vs Cloudfront 

------------------------------------------------------------------------------------------
Open question - 
* 1 load balancing, auto-scaling to application health monitoring on S3 bucket static website.
------------------------------------------------------------------------------------------

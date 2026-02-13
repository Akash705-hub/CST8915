# CST8915 Lab 2: Deploying the Algonquin Pet Store on Azure

- **Student Name**: Akash Patel
- **Student ID**: 041269598
- **Course**: CST8915 Full-stack Cloud-native Development
- **Semester**: Winter 2026

---

## Demo Video

🎥 I added the video under over here: [Click Here](https://drive.google.com/file/d/1oVh1rGSHCP6U3ce6O9HoL4RkCdOY0Dob/view?usp=sharing)

---

## Technical Explanations

### What challenges did you encounter when configuring environment variables in the GitHub Actions workflow?
- As such no issue encounterd during setup env variable in GitHub action workflow. Based on instruction provided on GitHub I follow the same and it works in first go.
### How does deploying microservices on Azure Web App Service differ from running them locally?
- Local execution of microservices typically implies running them in your own machine with tools such as Docker, or on a local server, and using this type of coupling, you have to manually deal with network routing, scaling, and environment configuration. When deployed to Microsoft Azure Web App Service, the infrastructure, scaling, load balancing and monitoring is automatically taken care of by Azure, so that the services are more reliable and ready to be deployed in production, without you having to maintain the servers directly.
### Why is it important to use environment variables for configurations in a cloud environment?
- Only difference is to configure env variables on azure that we don't need to manage env variable in our code so later on If we need to changes connection string for db/message service then we can do it from azure portal without touching code. 

## Repos Link

- https://github.com/Akash705-hub/store-front
- https://github.com/Akash705-hub/new_product-service
- https://github.com/Akash705-hub/order-service

## Acknowledgments

- https://github.com/ramymohamed10/26W_CST8915_Lab1
- https://www.youtube.com/watch?v=5tMGdEtBOrs&t=1s

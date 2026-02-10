# CST8915 Lab 2: 12-Factor App (Codebase, Dependencies, Configuration, and Backing Services)

- **Student Name**: Akash Patel
- **Student ID**: 041269598
- **Course**: CST8915 Full-stack Cloud-native Development
- **Semester**: Winter 2026

---

## Demo Video

🎥 I added the video under over here: [Click here](https://drive.google.com/file/d/1YxRgaJUv-0OMbT8Hh2jE0mOV5_hQhouo/view?usp=sharing)

---

## Technical Explanations


### What changes did you make to the order-service and product-service to comply with the Configurations and Backing Services factors of the 12-Factor App methodology?
- Single code base with the GitHub version control
- Dependencies
    - Ensure all dependencies are declared in a dependency management file (We achieved because of different programming languages we are using and all are having different way to use and consume packages)
    - Use dependency isolation. (Main aim is to not conflict with any other service. Our all three service are having different way to handle it.)
- Configuration
    - We extract any hard-coded configuration from the code (such as database URLs, RabbitMQ connection strings, ports, etc.) into environment variables.
- Backing Service
  - In our case Rabbit MQ message broker serice but in backing service it could be anything that could be attached to service.
### Why is it important to use environment variables instead of hard-coding configurations in your application?
- When we declared hard-coded value it is not easy to maintain when we manage large application. Sometime hard coded value expose the security concern for e.g. db connection string. When we declared environment variable then it is easy to maintain and we don't need to worry about changes at other location. We also seperate the environment value for different environment like TEST, UAT and PROD.
### Why is it important to have separate repositories for each microservice? How does this help maintain independence and scalability of each service?
- Separate repositories keep each microservice isolated so teams can develop, deploy, and scale them without affecting others. This independence prevents tight coupling and lets each service evolve at its own pace.

## Repos Link

- https://github.com/Akash705-hub/store-front
- https://github.com/Akash705-hub/product-service
- https://github.com/Akash705-hub/order-service

## Acknowledgments

- https://github.com/ramymohamed10/26W_CST8915_Lab1
- https://www.youtube.com/watch?v=5tMGdEtBOrs&t=1s
# CST8915 Lab 6: Containerizing the Algonquin Pet Store with Docker

- **Student Name**: Akash Patel
- **Student ID**: 041269598
- **Course**: CST8915 Full-stack Cloud-native Development
- **Semester**: Winter 2026

---

## Demo Video

🎥 I added the video under over here: [Click Here](https://drive.google.com/file/d/1AoVgKkfrKtbfGyUeD98_fcT_C3FcDjVH/view?usp=drive_link)


The application’s various services (such as product-service, order-service, and RabbitMQ Management Console) are all accessible via the same IP address, differentiated by paths (/products, /orders, /rabbitmq).
- NGINX is acting as a gateway that serves your frontend and routes requests to the correct backend services.

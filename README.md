Dự án Eproject-phase-1 sử dụng **kiến trúc microservices**.  
Mỗi dịch vụ được đóng gói trong **Docker container riêng biệt**, giao tiếp với nhau qua **RabbitMQ** và lưu trữ dữ liệu trong **MongoDB**.
1. Sau khi build dự án lên docker thì chạy dự án bằng lệnh docker-compose up -d -> các container được khởi chạy
![Docker](public/container_docker.png)

- Rabbit được khởi chảy với url: http://localhost:15672/#/
![Rabbit](public/connect_rabbit.png)

2.Test hệ thống bằng postman
- Register thành công
![Register](public/register.png)

-Login thành công, sẽ sinh ra 1 token
![Login](public/login.png)

-Lấy tocken để xem hồ sơ dashboad
![Darhboad](public/dashboard.png)

-Dữ liệu mongo của auth
![MongoDB auth](public/dulieu_auth.png)

- Tạo product
![Create-product](public/tao_product.png)

-Xem danh sách product
![products](public/lay_product.png)

-Dữ liệu Mongo của products
![MongoDB Product](public/dulieu_product.png)

-Tạo order
![Order](public/tao_order.png)

-Dữ liệu Mongo của order
![Mongo Order](public/dulieu_order.png)

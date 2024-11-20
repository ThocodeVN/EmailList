# Bước 1: Sử dụng OpenJDK làm base image
FROM openjdk:17-jdk-alpine

# Bước 2: Thiết lập thư mục làm việc trong container
WORKDIR /app

# Bước 3: Sao chép file .jar đã được biên dịch vào container
COPY target/email-list-1.0.jar /app/email-list.jar

# Bước 4: Lệnh để chạy ứng dụng khi container khởi động
CMD ["java", "-jar", "email-list.jar"]

# Bước 5: Mở cổng cho ứng dụng (nếu ứng dụng chạy trên cổng 8080, chỉnh lại nếu cần)
EXPOSE 8080

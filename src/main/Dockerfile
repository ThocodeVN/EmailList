# Bước 1: Chọn base image
FROM tomcat:9-jdk17-openjdk-slim

# Bước 2: Xóa ứng dụng web mặc định của Tomcat
RUN mkdir -p /app

# Bước 3: Sao chép file WAR vào thư mục webapps của Tomcat
# COPY target/MurachWeb-1.0-SNAPSHOT.war mkdir -p /app
COPY . .

# Bước 4: Mở port 8080 để truy cập ứng dụng web
EXPOSE 8080

# Bước 5: Lệnh khởi động Tomcat
CMD ["catalina.sh", "run"]

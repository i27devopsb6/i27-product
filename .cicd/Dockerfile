# base image
FROM openjdk:18

RUN mkdir -p /opt/i27

WORKDIR /opt/i27

ARG JAR_SOURCE 

COPY ["${JAR_SOURCE}", "/opt/i27/i27-product.jar"]

RUN chmod 777 /opt/i27

EXPOSE 8132

# Run the process
CMD ["java", "-jar", "/opt/i27/i27-product.jar"]

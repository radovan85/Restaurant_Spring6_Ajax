FROM tomcat:10.1-jdk17

WORKDIR /app

COPY target/restaurant-app.war /app/app.war

RUN mv /app/app.war /usr/local/tomcat/webapps/ROOT.war

# Postavljanje promenljivih okruženja za bazu podataka
ENV DB_URL=jdbc:postgresql://database:5432/restaurantdb
ENV DB_USERNAME=postgres
ENV DB_PASSWORD=1111

CMD ["catalina.sh", "run"]

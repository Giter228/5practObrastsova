FROM openjdk:17-jdk-bullseye

# Переменная окружения DISPLAY для графического вывода
ENV DISPLAY=host.docker.internal:0.0

# Установка библиотек
RUN apt-get update && apt-get install -y \
    libxext6 libxrender1 libxtst6 libxi6 libfreetype6 libx11-6 libxt6 \
    && rm -rf /var/lib/apt/lists/*

COPY calc.jar /app/calc.jar

WORKDIR /app

CMD ["java", "-jar", "calc.jar"]

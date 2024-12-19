FROM ubuntu:latest

# Обновление пакетов, установка xeyes
RUN apt-get update && apt-get install -y x11-apps && rm -rf /var/lib/apt/lists/*

# Переменная окружения DISPLAY для X11
ENV DISPLAY=host.docker.internal:0.0

# Запуск xeyes
CMD ["xeyes"]

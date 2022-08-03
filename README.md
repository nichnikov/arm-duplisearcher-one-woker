# arm-duplisearcher-one-woker
project with one worker


привязка папки с конфигурационным файлом:
https://stackoverflow.com/questions/30652299/having-docker-access-external-files


если запускать из папки проекта:

source="$(pwd)"/data - папка на сервере

target=/app/data - папка внутри контейнера

**команда для запуска контейнера:**

sudo docker run --mount type=bind,source="$(pwd)"/data,target=/app/data -it arm-duplisearcher-one-woker


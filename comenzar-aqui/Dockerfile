FROM alpine

# RUN, COPY, ADD, FROM -> crean capas

#RUN mkdir -p /app

# setea los comando en adelante en app y crea app
WORKDIR /app

#ADD (url) vs COPY
COPY myapp.sh /app/ 

# || si el anterior fallo , && si el anterior es success, ; no importa que paso con el anterior
RUN ls /app && chmod +x /app/myapp.sh && apk add --update bash

#se puede sobreescribir, parametrizables
CMD ["./myapp.sh"] 
# ENTRYPOINT ["bash"] ENTRYPOINT + CMD
# comandos por defecto cuando se instancia la imagen
# ENTRYPOINT [ "bash", "myapp.sh" ]
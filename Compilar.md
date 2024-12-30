1. Pasar toda la informacion de entorno a un .txt o JSon (Variables)

2. Crear una credencial de windows con el script 

3. utilizar cmd en el directorio del proyecto 

4. Ejecutar por consola el siguiente comando (Agregar las dependecias no presentes en comando, como importaciones ocultas --hidden-import nombreDelaImportacion)

pyinstaller -F --add-data "templates;templates" --add-data "static;static" --hidden-import flask_socketio --hidden-import flask_babelex --hidden-import flaskwebgui --hidden-import Flaskui --hidden-import socketio --hidden-import engineio --hidden-import threading --hidden-import time --hidden-import queue --hidden-import gevent --hidden-import psycopg2 --hidden-import serial --hidden-import Admin --hidden-import engineio.async_drivers.threading --hidden-import eventlet --hidden-import eventlet.hubs.epolls --hidden-import eventlet.hubs.kqueue --hidden-import eventlet.hubs.selects --hidden-import dns --hidden-import dns.asyncbackend --hidden-import dns.asyncquery --hidden-import dns.asyncresolver --hidden-import dns.dnssec --hidden-import dns.e164 --hidden-import dns.hash --hidden-import dns.namedict --hidden-import dns.tsigkeyring --hidden-import dns.update --hidden-import dns.zone --hidden-import dns.version --hidden-import dns.versioned --hidden-import waitress application.py

( agregar antes del application.py para que no se abra una consola)
--noconsole

5. Ejecutar Comando

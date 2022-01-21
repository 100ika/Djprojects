16.01.2022 Chapter 4. page 124

pip install Django
pip install Pillow
pip install social-auth-app-django
pip install django-extensions 
pip install Werkzeug
pip install pyOpenSSL
pip install django-sslserver

Установка сертификата безопасности http-https:
    https://timonweb.com/django/https-django-development-server-ssl-certificate/

    3. Запустить cmd от имени Адм. 
    4. Перейти в корневую папку проекта и запустить вирутальную машину. 
    5. mkcert "max.com" (example "mysite.com")
    6. переименовать файлы "max.com".pem - "max.com".key и "max.com".pem - "max.com".crt
            ren max.com-key.pem max.com.key
            ren max.com.pem max.com.crt
    7. pip install django_extensions 
        добавить в INSTALLED_APPS settings.py 'django_extensions' в конце
    8. В терминале vsc (env) запустить сервер 
        python manage.py runserver_plus "max.com:8000" --cert-file ./"max.com".crt


ngrok:
https://ngrok.com/download
пройти по иструкции 
добавить в settings.py / allowed_hosts адрес без "http"
запустить в cmd ngrok http 8000
запустить runserver






pip freeze 

Список установленных пакетов:
asgiref==3.4.1
certifi==2021.10.8
cffi==1.15.0
charset-normalizer==2.0.10
cryptography==36.0.1
defusedxml==0.7.1
Django==4.0.1
django-extensions==3.1.5
django-sslserver==0.22
idna==3.3
oauthlib==3.1.1
Pillow==9.0.0
pycparser==2.21
PyJWT==2.3.0
pyOpenSSL==21.0.0
python3-openid==3.2.0
requests==2.27.1
requests-oauthlib==1.3.0
six==1.16.0
social-auth-app-django==5.0.0
social-auth-core==4.1.0
sqlparse==0.4.2
tzdata==2021.5
urllib3==1.26.8
Werkzeug==2.0.2


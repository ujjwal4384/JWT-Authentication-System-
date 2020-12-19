# JWT-DJANGO
## Django-Rest-Framework-Authentication 

1.**Clone The repo**

```Bash
git clone
```
2.**Installation & Set-up**


```Console
pipenv install djangorestframework
pipenv shell
pipenv install djangorestframework_simplejwt
```
3.**Optional**

```console
python manage.py migrate
python manage.py createsuperuser
python manage.py makemigrations
python manage.py migrate

```
```console
install postman tool for testing
```


4.**Run The server**

```console
python manage.py runserver

```



  *  **Through Browser**
```Browser
Go to (https://127.0.0.1:8000)

Got to (https://127.0.0.1:8000/admin/)
(credentials required will be shown)
```
*  **Through Clients/tools like postman**

```Postman
Request Method : POST

url: (https://127.0.0.1:8000/api/token/)
BODY:-
x-www-form-urlencoded
```
    | Key             | Value       |
    |---------------- | ----------- |      
    | username        | password    |
    | ujjwalchitransh | Secret11    |
 #### Copy the access token obtained.   
 --You can use your own create superuser credentials as well--

 ```Postman
Request Method : GET
url: (https://127.0.0.1:8000/paradigms/)
Authorization:
TYPE:-Bearer token
Paste the access-token in required field 

```
**Using refresh token**

```Postman
Request Method : POST

url: (https://127.0.0.1:8000/api/token/refresh/)
BODY:-
x-www-form-urlencoded
```
    | Key            | Value          |
    | -------------- |--------------- |      
    | refresh        | <refreshtoken> |
   
 #### Copy the access token obtained.   


 *Successfull*

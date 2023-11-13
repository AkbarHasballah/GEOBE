# Paseto Project Backend
## _Progress Status_
Last Edited 17 Oktober 2023 11:27 PM

## Endpoint

- Insertdata User To Mongo
- Paseto Generator token
- Password Hasher

## Insert Data User

API Link : 

```sh
https://asia-southeast2-gis-project-401902.cloudfunctions.net/UserdataInsert
```
Body :

```sh
{
    "username" : "user",
    "password" : "pass"
}
```

Password akan dihash otomatis didalam fungsi
Response :
```sh
{
    "status": true,
    "message": "Berhasil Input data"
}
```

## Paseto Token

API Link : 

```sh
https://asia-southeast2-gis-project-401902.cloudfunctions.net/PASETO-Project
```
Body :

```sh
{
    "username" : "user",
    "password" : "pass"
}
```
Response : 
```sh
{
    "status": true,
    "token": "token",
    "message": "Selamat Datang"
}
```

## Password Hasher

API Link : 

```sh
https://asia-southeast2-gis-project-401902.cloudfunctions.net/Password-Hasher
```
Body :

```sh
{
    "username" : "user",
    "password" : "pass"
}
```
Response : 
```sh
{
    "status": true,
    "token": "$2a$12$AMrX.qRPNEBUaa2HhSP8dOte0Fu9wO7vJ19IPxarXkhFQNNEAA3HW",
    "message": "Berhasil Hash Password"
}
```
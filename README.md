
# Role-Based Access Control (RBAC)


## Deployment

-> To deploy this project run


```bash
  npm install
```

-> Database Used Mongodb|| so start Mongodb service and import admin db using STUDIO 3T





#### OR CREATE 


| DB NAME | ADMIN COLLECTION    
| :-------- | :------- |
| `RBAC` | `admin` | 

#### in admin Collection insert this data or create Like

```
  {
    "name" : "admin",
    "email" : "admin@gmail.com",
    "password" : "$2b$10$Q4RBLd86dgJO1sFJjDxJa.jpahPgftOIuPzqX4DI1G2KY3AoSyjeC",
    "role" : "admin"
}
```
### (GIVEN PASSWORD HASH VALUE IS 1 )




## Environment Variables

To run this project, you will need to add the following environment variables to your .env file (and manually added to this repo if unable to clone .env use this)
```
DB_URL=mongodb://127.0.0.1:27017/
DB_NAME=RBAC
USER_COLLECTION=users
ADMIN_COLLECTION=admin
MODERATOR_COLLECTION=moderators
JWT_SECRET=this-is-my-secret-key
SALT_ROUND=10`
```


-> TO RUN PROJECT 

```
npm start

```
-> URL


```
http://localhost:3000/

```
## Reference

#### Methods
#### User Methods

```
  GET    /  [root]seted as login
```

```
  POST   /
```
```
  GET    /signup
```
```
  POST   /signup
```
```
  GET    /dashboard
```
```
  GET    /logout
```
#### Admin Methods

```
  GET    /admin
```
```
  POST   /admin
```

```
  GET    /admin/dashboard
```
```
  GET    /admin/updateUser?
```



## Features

- USER PASSWORD HASHING AND AUTHENTICATION
- JWT AUTHERISETION
- MANAGE USER ROLES
- ROLE DASED ACCESS


## Tech Stack

**Client:** HandleBars, Bootstrap, TailwindCSS

**Server:** Node, Express,Mongodb,ExpreessGenartor,Bcript,JWT,


## FAQ

#### Is Additionally can use OTHER METHODS?

Yes, by adding NEEDED ROUTES on project Routes wecan use other REST methods and also pass jwt token as barear Token for verify autherisation and authentication


## Screenshots

![App Screenshot](https://raw.githubusercontent.com/Azharkoivila/Role-Based-Access-Control-RBAC-/refs/heads/main/ScreenShots/Screenshot%20from%202024-11-28%2019-34-13.png)
![App Screenshot](https://raw.githubusercontent.com/Azharkoivila/Role-Based-Access-Control-RBAC-/refs/heads/main/ScreenShots/Screenshot%20from%202024-11-28%2019-34-23.png)



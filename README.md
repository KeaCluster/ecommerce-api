# Test

## EcommerceDB

### Desc

This is a test Spring Boot app meant to be a base for future deploys on Railway

Not ready for production
> ?Could be ready for production

### Info

There's an ```application-prod.yml``` file used to save basic production config data. This will have different info depending on the platform you're making the deploy. Check it for more context. What's in there however is specifically for railway.

## Part 1

### SETUP - railway account

- Login or setup new railway account.
- Recommended to be setup from github for easier access to respositories.
- [Railway dot app](railway.app)

### SETUP - New project




## Environment variables

These properties define your DB environment variables
Copy your info from railway given by the mysql service and paste them here, although it's not safe for your app because it will be visible from github.
All these environment variables are to be pasted in your service Variables before deploying

```properties
spring_profiles_active=prod
PROD_DB_HOST=HOST_HERE
PROD_DB_PORT=POST_HERE
PROD_DB_NAME=railway
PROD_DB_PASSWORD=PASSWORD_HERE
PROD_DB_USERNAME=postgres
```

Keep ```src/main/resources/application.properties``` unmodified. There's a new ```application-prod.yml``` file for production config.

Also, check ```Procfile```. Maintain all application names and versions according to your ```build.gradle``` and ```settings.gradle``` files


## References

[Spring boot Railway - Dan Vega](https://www.youtube.com/watch?v=5sVxvF47dcU&t=820s)

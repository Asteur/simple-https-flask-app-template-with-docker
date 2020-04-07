**Simple Docker Flask Application Template**

Set up https for your flask app in minutes

____

**First:**

- Update files for your domain
    
    1. init-letsencrypt.sh
    
        - change to your `domains`
        - change to your `email`
        - change `staging` if you need to check certificate generation (0 - production, 1 - test)
    
    2. nginx/nginx.conf
    
        - change `example.com` to your domain name

**Second:**

- Get certificate from letsencrypt and certbot
    
    - Run `sh init-letsencrypt.sh`
    - Answer the questions asked in the script
  
**Third:**  

- Put your Flask app in `app` folder
- **Change `Dockerfile` if necessary
- **Add additional containers and set environment variables in docker-compose.yml if necessary
- Run `docker-compose up --build`
- Have a rest
        


___

based on <link>https://github.com/wmnnd/nginx-certbot</link>

---

Used in a project inspired by coronavirus <link>https://onehot.news</link>

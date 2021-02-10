## Forked for deployment by parthmerchant

https://tranquil-harbor-11260.herokuapp.com/

### How to run on Heroku:

1. Clone Repository
```sh
git clone <repo-name>
cd <repo-name>
```

2. Login to Heroku
```sh
heroku login
```

3. Initialize Git
```sh
git init
```

4. Set remote to heroku
```sh
heroku git:remote -a <repo-name>
```

5. Make changes to DATABASE (if necessary)
6. Add Heroku buildpacks
- https://github.com/heroku/heroku-geo-buildpack.git
- heroku/python

7. Add changes and commit 
```sh
git add .
git commit -am "First commit from Heroku CLI"
```

8. Push changes
```sh
git push heroku master:deploy
```

9. Check to see if your changes have been pushed onto Heroku
```sh
heroku run bash
ls
```

10. Migrate your database
```sh
python ./manage.py migrate
```

11. Create superuser
```sh
python ./manage.py createsuperuser 
```

12. Your Django app if now running on the web!


------------------------------------------------------------------------------------------

# Team Project repo
NYC-ACCESSIBLE-RESTAURANT-ADVISOR

https://accessible-nyc.herokuapp.com

Integration instance

<a href="https://travis-ci.com/github/gcivil-nyu-org/nyc-accessible-restaurant-advisor">
    <img 
         alt="Build Status" 
         src="https://travis-ci.com/gcivil-nyu-org/nyc-accessible-restaurant-advisor.svg?branch=develop">
</a>
<a href='https://coveralls.io/github/gcivil-nyu-org/nyc-accessible-restaurant-advisor?branch=develop'>
    <img
        src="https://coveralls.io/repos/github/gcivil-nyu-org/nyc-accessible-restaurant-advisor/badge.svg?branch=develop"
        alt='Coverage Status' />
</a>


https://accessible-nyc-main.herokuapp.com

Production instance

<a href="https://travis-ci.com/github/gcivil-nyu-org/nyc-accessible-restaurant-advisor">
    <img 
         alt="Build Status" 
         src="https://travis-ci.com/gcivil-nyu-org/nyc-accessible-restaurant-advisor.svg?branch=main">
</a>
<a href='https://coveralls.io/github/gcivil-nyu-org/nyc-accessible-restaurant-advisor?branch=main'>
    <img
        src="https://coveralls.io/repos/github/gcivil-nyu-org/nyc-accessible-restaurant-advisor/badge.svg?branch=main&servive=github"
        alt='Coverage Status' />
</a>


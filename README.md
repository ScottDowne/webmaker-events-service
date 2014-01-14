Development
============
```
npm install
node server
```

Routes
============

`GET /events`
```
{
  limit: {{a limit}}
}
```

`GET /events/:id`

`POST /events`
`{event object}`

`PUT /events/:id`
`{updated attributes}`

`DELETE /events/:id`


Deployment
===========

```
heroku create webmaker-events-service
git push heroku master
```

Configuration
=============

If you don't already have the Heroku config plugin installed, do it now:

```
heroku plugins:install git://github.com/ddollar/heroku-config.git
```

 Now you can push up your .env config file like this:

```
heroku config:push --overwrite

```
# heroku_aiogram_example

## Description
Minimal working example of running aiogram v3 echo bot on heroku with webhook. 

Based on [aiogram documentation example](https://docs.aiogram.dev/en/latest/dispatcher/webhook.html) and [Heroku documentation](https://devcenter.heroku.com/categories/python-support)

## How to deploy

1. `git clone https://github.com/vlivanov1232/heroku_aiogram_example.git`
2. `cd heroku_aiogram_example`
3. `heroku create`
4. `heroku labs:enable runtime-dyno-metadata`
5. `heroku config:set BOT_TOKEN=%your botfather bot token%`
6. `heroku buildpacks:clear`
7. `heroku buildpacks:add https://github.com/moneymeets/python-poetry-buildpack.git`
8. `heroku buildpacks:add heroku/python`
7. `git push heroku`
8. `heroku ps:scale web=1`
 


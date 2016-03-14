# Postgres Install Instructions

## Get Postgres

```
$ brew install postgres
```

You should see the following instructions after the install is finished.

The first method will launch the postgres server each time boot your computer. You can use the second method to launch the server manually.
> To have launchd start postgresql at login:
  `ln -sfv /usr/local/opt/postgresql/*.plist ~/Library/LaunchAgents`
  
>To load postgresql:
  `launchctl load ~/Library/LaunchAgents/homebrew.mxcl.postgresql.plist`

>Or, if you don't want/need launchctl, you can just run:
  `postgres -D /usr/local/var/postgres`

Then, to create a database for your user, run this command

```
createdb
```


Alternatively, you can download Postgres.app [here](http://postgresapp.com/)

## Get a client

I recommend [Postico](https://eggerapps.at/postico/), but [pgAdmin](http://www.pgadmin.org/download/macosx.php) is also a good alternative. For those who love the command line, there is a command line client, psql, which comes with the postgres server install. (If you downloaded Postgres.app, you will need to adjust your path to access them by following [these steps](http://postgresapp.com/documentation/cli-tools.html))

## Check your work

When you are finished, raise your hand I will come check your install.

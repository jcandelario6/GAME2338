Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

Try the new cross-platform PowerShell https://aka.ms/pscore6

PS C:\Users\jnc66> heroku login
heroku: Press any key to open up the browser to login or q to exit:
Opening browser to https://cli-auth.heroku.com/auth/cli/browser/e81c3c20-af73-4b37-9264-eebb991fb5d1
Logging in... done
Logged in as jnc6658@gmail.com
PS C:\Users\jnc66> git clone https://github.com/heroku/python-getting-started.git                                       fatal: destination path 'python-getting-started' already exists and is not an empty directory.
PS C:\Users\jnc66> cd python-getting-started                                                                            PS C:\Users\jnc66\python-getting-started> heroku create                                                                 Creating app... done, ⬢ powerful-beach-38436
https://powerful-beach-38436.herokuapp.com/ | https://git.heroku.com/powerful-beach-38436.git
PS C:\Users\jnc66\python-getting-started> git push heroku master                                                        Everything up-to-date
PS C:\Users\jnc66\python-getting-started> heroku ps:scale web=1                                                         Scaling dynos... done, now running web at 1:Free
PS C:\Users\jnc66\python-getting-started> heroku open                                                                   PS C:\Users\jnc66\python-getting-started> heroku logs --tail                                                            2020-05-03T17:34:02.498080+00:00 heroku[web.1]: Unidling
2020-05-03T17:34:02.513533+00:00 heroku[web.1]: State changed from down to starting
2020-05-03T17:34:11.201008+00:00 app[web.1]: [2020-05-03 17:34:11 +0000] [4] [INFO] Starting gunicorn 20.0.4
2020-05-03T17:34:11.201689+00:00 app[web.1]: [2020-05-03 17:34:11 +0000] [4] [INFO] Listening at: http://0.0.0.0:58224 (4)
2020-05-03T17:34:11.201806+00:00 app[web.1]: [2020-05-03 17:34:11 +0000] [4] [INFO] Using worker: sync
2020-05-03T17:34:11.206446+00:00 app[web.1]: [2020-05-03 17:34:11 +0000] [10] [INFO] Booting worker with pid: 10
2020-05-03T17:34:11.245889+00:00 app[web.1]: [2020-05-03 17:34:11 +0000] [11] [INFO] Booting worker with pid: 11
2020-05-03T17:34:12.686101+00:00 heroku[web.1]: State changed from starting to up
2020-05-03T17:34:14.644084+00:00 heroku[router]: at=info method=GET path="/" host=mighty-taiga-78352.herokuapp.com request_id=06a05f00-f457-4652-8762-15ca6ce813ea fwd="107.138.214.198" dyno=web.1 connect=0ms service=43ms status=200 bytes=7643 protocol=https
2020-05-03T17:34:14.643027+00:00 app[web.1]: 10.186.202.203 - - [03/May/2020:17:34:14 +0000] "GET / HTTP/1.1" 200 7425 "-" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.129 Safari/537.36"2020-05-03T17:34:14.978977+00:00 heroku[router]: at=info method=GET path="/static/lang-logo.png" host=mighty-taiga-78352.herokuapp.com request_id=6fab678e-6dc3-4e0e-861a-af8704d0579d fwd="107.138.214.198" dyno=web.1 connect=0ms service=6ms status=200 bytes=2498 protocol=https
2020-05-03T17:34:14.977863+00:00 app[web.1]: 10.186.202.203 - - [03/May/2020:17:34:14 +0000] "GET /static/lang-logo.png HTTP/1.1" 200 0 "https://mighty-taiga-78352.herokuapp.com/" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.129 Safari/537.36"
2020-05-03T17:34:15.339210+00:00 heroku[router]: at=info method=GET path="/favicon.ico" host=mighty-taiga-78352.herokuapp.com request_id=6953e6a6-3f30-4d57-98ba-42b333bf5d78 fwd="107.138.214.198" dyno=web.1 connect=0ms service=18ms status=404 bytes=2437 protocol=https
2020-05-03T17:34:15.337051+00:00 app[web.1]: Not Found: /favicon.ico
2020-05-03T17:34:15.337777+00:00 app[web.1]: 10.186.202.203 - - [03/May/2020:17:34:15 +0000] "GET /favicon.ico HTTP/1.1" 404 2227 "https://mighty-taiga-78352.herokuapp.com/" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.129 Safari/537.36"
2020-05-03T17:37:58.007379+00:00 app[api]: Scaled to web@0:Free by user jnc6658@gmail.com
2020-05-03T17:37:58.803460+00:00 heroku[web.1]: State changed from up to down
2020-05-03T17:38:00.286925+00:00 app[web.1]: [2020-05-03 17:38:00 +0000] [10] [INFO] Worker exiting (pid: 10)
2020-05-03T17:38:00.288284+00:00 app[web.1]: [2020-05-03 17:38:00 +0000] [4] [INFO] Handling signal: term
2020-05-03T17:38:00.294794+00:00 app[web.1]: [2020-05-03 17:38:00 +0000] [11] [INFO] Worker exiting (pid: 11)
2020-05-03T17:38:00.501481+00:00 app[web.1]: [2020-05-03 17:38:00 +0000] [4] [INFO] Shutting down: Master
2020-05-03T17:38:24.149555+00:00 app[api]: Scaled to web@1:Free by user jnc6658@gmail.com
2020-05-03T17:38:30.635724+00:00 app[web.1]: [2020-05-03 17:38:30 +0000] [4] [INFO] Starting gunicorn 20.0.4
2020-05-03T17:38:30.636354+00:00 app[web.1]: [2020-05-03 17:38:30 +0000] [4] [INFO] Listening at: http://0.0.0.0:35945 (4)
2020-05-03T17:38:30.636474+00:00 app[web.1]: [2020-05-03 17:38:30 +0000] [4] [INFO] Using worker: sync
2020-05-03T17:38:30.640705+00:00 app[web.1]: [2020-05-03 17:38:30 +0000] [10] [INFO] Booting worker with pid: 10
2020-05-03T17:38:30.731961+00:00 app[web.1]: [2020-05-03 17:38:30 +0000] [11] [INFO] Booting worker with pid: 11
2020-05-03T17:38:31.372680+00:00 heroku[web.1]: State changed from starting to up
2020-05-03T17:46:11.309532+00:00 heroku[router]: at=info method=GET path="/" host=mighty-taiga-78352.herokuapp.com request_id=b120958b-2b97-4c14-8a6c-05226ecd188d fwd="107.138.214.198" dyno=web.1 connect=1ms service=35ms status=200 bytes=7643 protocol=https
2020-05-03T17:46:11.312604+00:00 app[web.1]: 10.13.148.247 - - [03/May/2020:17:46:11 +0000] "GET / HTTP/1.1" 200 7425 "-" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.129 Safari/537.36"
2020-05-03T17:46:11.444675+00:00 app[web.1]: 10.13.148.247 - - [03/May/2020:17:46:11 +0000] "GET /static/lang-logo.png HTTP/1.1" 304 0 "https://mighty-taiga-78352.herokuapp.com/" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.129 Safari/537.36"
2020-05-03T17:46:11.441238+00:00 heroku[router]: at=info method=GET path="/static/lang-logo.png" host=mighty-taiga-78352.herokuapp.com request_id=82b88110-3cdb-4fbb-a94e-744ca13e947d fwd="107.138.214.198" dyno=web.1 connect=1ms service=5ms status=304 bytes=166 protocol=https
2020-05-03T17:48:29.908368+00:00 app[api]: Starting process with command `python manage.py shell` by user jnc6658@gmail.com
2020-05-03T17:48:35.069718+00:00 heroku[run.9370]: State changed from starting to up
2020-05-03T17:52:45.907907+00:00 heroku[router]: at=info method=GET path="/" host=mighty-taiga-78352.herokuapp.com request_id=864cb0b6-8ca6-48b5-a12b-0be5abfbcac7 fwd="107.138.214.198" dyno=web.1 connect=1ms service=27ms status=200 bytes=7643 protocol=https
2020-05-03T17:52:45.907153+00:00 app[web.1]: 10.101.178.182 - - [03/May/2020:17:52:45 +0000] "GET / HTTP/1.1" 200 7425 "-" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.129 Safari/537.36"2020-05-03T17:52:46.025830+00:00 app[web.1]: 10.101.178.182 - - [03/May/2020:17:52:46 +0000] "GET /static/lang-logo.png HTTP/1.1" 304 0 "https://mighty-taiga-78352.herokuapp.com/" "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/81.0.4044.129 Safari/537.36"
2020-05-03T17:52:46.026386+00:00 heroku[router]: at=info method=GET path="/static/lang-logo.png" host=mighty-taiga-78352.herokuapp.com request_id=c17f80fc-93b0-4182-a73e-1a305f42bb12 fwd="107.138.214.198" dyno=web.1 connect=1ms service=4ms status=304 bytes=166 protocol=https
Scaling dynos... done, now running web at 0:Free
Scaling dynos... done, now running web at 1:Free
PS C:\Users\jnc66\python-getting-started> pip install -r requirements.txt                                               pip : The term 'pip' is not recognized as the name of a cmdlet, function, script file, or operable program. Check the
spelling of the name, or if a path was included, verify that the path is correct and try again.
At line:1 char:1r.heroku.com/articles/dyno-sleeping
+ pip install -r requirements.txt
+ ~~~un: one-off processes (1)
    + CategoryInfo          : ObjectNotFound: (pip:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
 == web (Free): gunicorn gettingstarted.wsgi --log-file - (1)
PS C:\Users\jnc66\python-getting-started> pip list
pip : The term 'pip' is not recognized as the name of a cmdlet, function, script file, or operable program. Check the
spelling of the name, or if a path was included, verify that the path is correct and try again.
At line:1 char:1
+ pip list
+ ~~~
    + CategoryInfo          : ObjectNotFound: (pip:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS C:\Users\jnc66\python-getting-started> python manage.py collectstatic
PS C:\Users\jnc66\python-getting-started> heroku local web -f Procfile.windows
[OKAY] Loaded ENV .env File as KEY=VALUE Format
12:54:51 PM web.1 |  Python was not found but can be installed from the Microsoft Store: http
12:54:51 PM web.1 |  s://go.microsoft.com/fwlink?linkID=2082640
[DONE] Killing all processes with signal  SIGINT
12:54:51 PM web.1 Exited with exit code null
PS C:\Users\jnc66\python-getting-started> heroku local web
[OKAY] Loaded ENV .env File as KEY=VALUE Format
12:54:59 PM web.1 |  'gunicorn' is not recognized as an internal or external command,
12:54:59 PM web.1 |  operable program or batch file.
[DONE] Killing all processes with signal  SIGINT
12:54:59 PM web.1 Exited with exit code null
PS C:\Users\jnc66\python-getting-started> def index(request):
request : The term 'request' is not recognized as the name of a cmdlet, function, script file, or operable program.
Check the spelling of the name, or if a path was included, verify that the path is correct and try again.
At line:1 char:11
+ def index(request):
+           ~~~~~~~
    + CategoryInfo          : ObjectNotFound: (request:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS C:\Users\jnc66\python-getting-started> heroku local
[OKAY] Loaded ENV .env File as KEY=VALUE Format
12:55:25 PM web.1 |  'gunicorn' is not recognized as an internal or external command,
12:55:25 PM web.1 |  operable program or batch file.
[DONE] Killing all processes with signal  SIGINT
12:55:25 PM web.1 Exited with exit code null
PS C:\Users\jnc66\python-getting-started> git add .
PS C:\Users\jnc66\python-getting-started> git commit -m "Demo"

*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"

to set your account's default identity.
Omit --global to set the identity only in this repository.

fatal: unable to auto-detect email address (got 'jnc66@DESKTOP-RQ6SR35.(none)')
Creating papertrail on ⬢ mighty-taiga-78352... !
 !    Please verify your account to install this add-on plan (please enter a credit card) For more information, see
 !    https://devcenter.heroku.com/categories/billing Verify now at https://heroku.com/verify
Running python manage.py shell on ⬢ mighty-taiga-78352... !
 !    Cannot run more than 1 Free size dynos.
Setting TIMES and restarting ⬢ mighty-taiga-78352... done, v6
Running python manage.py migrate on ⬢ mighty-taiga-78352... !
 !    Cannot run more than 1 Free size dynos.
PS C:\Users\jnc66\python-getting-started> def db(request):ds.
request : The term 'request' is not recognized as the name of a cmdlet, function, script file, or operable program. 209-Check the spelling of the name, or if a path was included, verify that the path is correct and try again.heck the
At line:1 char:8name, or if a path was included, verify that the path is correct and try again.
+ def db(request):python-getting-started> heroku addons:open papertrail
+        ~~~~~~~ind that add on.
    + CategoryInfo          : ObjectNotFound: (request:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException─────  ─────  ───────dException
 eroku-postgresql (postgresql-transparent-98760)  hobby-dev  free   created
PS C:\Users\jnc66\python-getting-started> heroku ps:psql
 »   Warning: ps:psql is not a heroku command.rt os
Did you mean pg:psql? [y/n]:  and the attachments to the current app (mighty-taiga-78352) or other apps. program.
 »   Error: Run heroku help ps for a list of available commands.y that the path is correct and try again.
PS C:\Users\jnc66\python-getting-started> heroku pg:psql
--> Connecting to postgresql-transparent-98760
 !    The local psql command could not be located. For help installing psql, seeb4844025e67d1db61a80951e@ec2-54-147-209- !    https://devcenter.heroku.com/articles/heroku-postgresql#local-setupNotFoundException
PS C:\Users\jnc66\python-getting-started> undException
PS C:\Users\jnc66\python-getting-started> heroku pg
=== DATABASE_URL6\python-getting-started> de index(request):
Plan:                  Hobby-devnot recognized as the name of a cmdlet, function, script file, or operable program.
Status:                Availableor if a path was included, verify that the path is correct and try again.
Connections:           0/20
PG Version:            12.2
Created:               2020-04-25 01:06 UTC
Data Size:             7.9 MB ObjectNotFound: (request:String) [], CommandNotFoundException
Tables:                0rId : CommandNotFoundException
Rows:                  0/10000 (In compliance)
Fork/Follow:           Unsupportedtarted> heroku config:set TIMES=2
Rollback:              Unsupported
Continuous Protection: Off
Add-on:                postgresql-transparent-98760

PS C:\Users\jnc66\python-getting-started> heroku run python manage.py migrate

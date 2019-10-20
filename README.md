10401  cd rubyspace
10402  rails new toy_app
10406  cd toy_app
10407  git init
10408  git status
10409  git add .
10410  git commit -m "initial commit"


10411  git remote add origin https://github.com/xiaoweiruby/toy_app.git
10412  git push -u origin master
10413  atom .


```
移动 gem 'sqlite3'

group :development, :test do
  gem 'sqlite3'
  gem 'byebug', platforms: [:mri, :mingw, :x64_mingw]
end

增加 gem 'pg', '0.18.4'

group :production do
  gem 'pg', '0.18.4'
end
```

```
xiaowei@xiaoweimac ⮀ ~/rubyspace/toy_app ⮀ ⭠ master± ⮀ heroku create
▸    heroku-cli: update available from 6.15.18-fdf2097 to 6.99.0-ec9edad
Creating app... !
▸    You've reached the limit of 5 apps for unverified accounts. Delete some
▸    apps or add a credit card to verify your account.
✘ xiaowei@xiaoweimac ⮀ ~/rubyspace/toy_app ⮀ ⭠ master± ⮀ heroku apps:destroy intense-sands-75913
▸    heroku-cli: update available from 6.15.18-fdf2097 to 6.99.0-ec9edad
▸    WARNING: This will delete ⬢ intense-sands-75913 including
▸    all add-ons.
▸    To proceed, type intense-sands-75913 or re-run this
▸    command with --confirm intense-sands-75913

> intense-sands-75913
Destroying ⬢ intense-sands-75913 (including all add-ons)... done
xiaowei@xiaoweimac ⮀ ~/rubyspace/toy_app ⮀ ⭠ master± ⮀ heroku create
▸    heroku-cli: update available from 6.15.18-fdf2097 to 6.99.0-ec9edad
Creating app... done, ⬢ enigmatic-ravine-69283
https://enigmatic-ravine-69283.herokuapp.com/ | https://git.heroku.com/enigmatic-ravine-69283.git
xiaowei@xiaoweimac ⮀ ~/rubyspace/toy_app ⮀ ⭠ master± ⮀ git add .
xiaowei@xiaoweimac ⮀ ~/rubyspace/toy_app ⮀ ⭠ master± ⮀ git commit -m "update gemfie for heroku"
[master 69173b4] update gemfie for heroku
2 files changed, 34 insertions(+), 25 deletions(-)
rewrite README.md (98%)
xiaowei@xiaoweimac ⮀ ~/rubyspace/toy_app ⮀ ⭠ master ⮀ git push
Counting objects: 4, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 692 bytes | 692.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/xiaoweiruby/toy_app.git
  c32fb6b..69173b4  master -> master
xiaowei@xiaoweimac ⮀ ~/rubyspace/toy_app ⮀ ⭠ master ⮀ git push heroku master
```

https://stackoverflow.com/questions/28021240/rails-tutorial-2-5-2-cant-get-validaiton-exercise-to-work

https://stackoverflow.com/questions/27295860/rails-validate-statement-checking-for-blank-content

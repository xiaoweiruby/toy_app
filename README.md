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

```
class User < ApplicationRecord
  has_many :microposts
  validates :name, presence: true
  validates :email, presence: true
end
```

```
class Micropost < ApplicationRecord
  belongs_to :user
  validates :content, length: { maximum: 140 }, presence: true
end
```

```
0363  cd rubyspace
10364  atom .
10365  cd hello_app
10366  atom .
10367  bundle install
10368  git add .
10369  git commit -m "update Gemfile for Heroku"
10370  heroku create hello_app_101
10371  heroku version
10372  heroku login
10373  heroku create hello_app_101
10374  heroku create
10375  git push heroku master
10376  git add .
10377  git commit -m "edit ruby 2.4.4"
10378  git push heroku master
10379  bundle install
10380  rvm install 2.4.4
10381  git push heroku master
10382  bundle install
10383  ruby -v
10384  git add .
10385  git commit -m "up ruby 2.4.4"
10386  git push heroku master
10387  atom .
10388  ruby -v
10389  git add .
10390  git commit -m "edit RUBY VERSION"
10391  git push heroku master
10392  heroku open
10393  git push
10394  git add .
10395  git commit -m "edit readme"
10396  git push
10397  git add .
10398  git commit -m "add heroku address link"
10399  git push
10400  ls
10401  cd rubyspace
10402  rails new toy_app
10403  git init
10404  rm -rf .git
10405  ls
10406  cd toy_app
10407  git init
10408  git status
10409  git add .
10410  git commit -m "initial commit"
10411  git remote add origin https://github.com/xiaoweiruby/toy_app.git
10412  git push -u origin master
10413  atom .
10414  history
10415  heroku create
10416  heroku apps:destroy intense-sands-75913
10417  heroku create
10418  git add .
10419  git commit -m "update gemfie for heroku"
10420  git push
10421  git push heroku master
10422  ruby -v
10423  cd
10424  ls
10425  cd rubyspace
10426  ls
10427  cd hello_app
10428  ruby -v
10429  cd
10430  curl -L get.rvm.io | bash -s stable
10431  source ~/.bashrc
10432  source ~/.bash_profile
10433  rvm -v
10434  rvm reload
10435  rvm -v
10436  ruby -v
10437  rvm list known
10438  rvm install 2.4.4
10439  ls
10440  cd rubyspace
10441  ls
10442  cd toy_app
10443  bundle install
10444  ruby -v
10445  rvm install 2.4.4
10446  ruby -v
10447  git push heroku master
10448  git ad .
10449  git add .
10450  git commit -m "edit ruby 2.4.4p296"
10451  git push heroku master
10452  herkou open
10453  heroku open
10454  rail s
10455  rails s
10456  bundle install
10457  rails s
10458  bundle install
10459  rails s
10460  git add .
10461  git commit -m "bundle install"
10462  git push
10463  git push heroku master
10464  heroku open
10465  rails s
10466  git add .
10467  git commit -m "add def hello"
10468  git push
10469  git push heroku master
10470  heroku open
10471  rails generate scaffold User name:string email:string
10472  rake db:migrate
10473  rails s
10474  atom .
10475  rails s
10476  cd
10477  ls
10478  cd rubyspace
10479  ls
10480  rails new toy_app_01
10481  ls
10482  cd toy_app_01
10483  rails generate scaffold User name:string email:string
10484  rake db:migrate
10485  atom .
10486  rails s
10487  cd
10488  brew uninstall --force node
10489  brew uninstall --ignore-dependencies node
10490  brew uninstall --force node
10491  brew uninstall icu4c && brew install icu4c
10492  brew uninstall --ignore-dependencies icu4c
10493  brew uninstall --force icu4c
10494  brew unlink icu4c && brew link icu4c --force
10495  brew install node
10496  cd
10497  ls
10498  cd rubyspace
10499  ls
10500  cd toy_app_01
10501  rails s
10502  cd ..
10503  ls
10504  cd toy_app
10505  rails s
10506  atom .
10507  bundle install
10508  rvm install 2.2.4
10509  rvm install 2.4.4
10510  rails s
10511  rails generate scaffold Micropost content:text user_id:integer
10512  rake db:migrate
10513  rails s
10514  rails console
10515  rails s
10516  bundle install
10517  rvm install 2.4.4
10518  rail
10519  rails s
10520  git add .
10521  git commit -m "add validates"
10522  git push
10523  git push heroku master
10524  heroku open
10525  rails s
10526  heroku run rake db:migrate
10527  heroku rake db:migrate
10528  heroku open
10529  heroku logs | grep -i error
10530  git add .
10531  git commit -m "delele hello_controller"
10532  git push heroku master
10533  heroku open
10534  heroku logs | grep -i error
10535  rails s
10536  heroku apps:destroy enigmatic-ravine-69283
10537  atom .
```

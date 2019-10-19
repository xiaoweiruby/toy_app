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

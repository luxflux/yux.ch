desc 'Test view of the website'
task :watch do
  sh 'jekyll serve -w'
end

desc 'Build website'
task :build do
  sh 'jekyll build -q'
end

desc 'Deploy website'
task :deploy => :build do
  sh 'rsync -aq --delete _site/ raf@web.yux.ch:/srv/www/yux.ch/'
end

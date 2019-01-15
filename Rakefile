desc "Deploy book"
task :deploy do
  exec "bundle exec softcover deploy"
end

desc "Build book"
task :build do
  exec "bundle exec softcover build:all"
end

desc "Build preview"
task :build_preview do
  exec "bundle exec softcover build:preview"
end

desc "Website stats"
task :website_stats do
  exec "bash stats.sh"
end

desc "HTML generation"
task :html do
  `pandoc -o padrino_book.html *.md`
  puts ".. done\nName of the html is `padrino_book.html`"
end

desc "Cleaning the generated output format"
task :clean do
  `rm padrino_book.epub`
  `rm padrino_book.html`
  puts ".. done"
end

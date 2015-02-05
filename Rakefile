desc "Build the site from source to build"
task :build do
  puts "## Building website"
  status = system("middleman build --clean")
  puts status ? "OK" : "FAILED"
end

desc "Run middleman server"
task :preview do
  system("middleman server")
end

desc "Watch and compress Sass"
task :sass do
  system("cd source/assets/css && sass --watch styles.scss:styles.css --style compressed")
end

desc "Build Static Site"
task :sass do
  system("middleman build")
end
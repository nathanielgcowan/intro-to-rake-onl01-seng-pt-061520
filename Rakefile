Skip to content
Sign up
learn-co-students
/
intro-to-rake-onl01-seng-pt-061520
Code
Issues
Pull requests
26
Actions
More
Join GitHub today
GitHub is home to over 50 million developers working together to host and review code, manage projects, and build software together.

intro-to-rake-onl01-seng-pt-061520/Rakefile /
@victhevenot
victhevenot started tests
 History
 4 contributors
@SophieDeBenedetto@victhevenot@sammarcus@pletcher
34 lines (28 sloc)  599 Bytes
  
require 'pry'

task :environment do
  require_relative './config/environment'
end

desc 'outputs hello to the terminal'
namespace :greeting do
  task :hello do
    puts 'hello from Rake!'
  end

  desc 'outputs hola to the terminal'
  task :hola do
    puts 'hola de Rake!'
  end
end

namespace :db do
  desc 'migrate changes to your database'
  task migrate: :environment do
    Student.create_table
  end

  desc 'seed the database with some dummy data'
  task :seed do
    require_relative './db/seeds.rb'
  end
end

desc 'drop into the Pry console'
task console: :environment do
  Pry.start
end
© 2020 GitHub, Inc.
Terms
Privacy
Security
Status
Help
Contact GitHub
Pricing
API
Training
Blog
About

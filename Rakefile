namespace :greeting do
desc "Output hello to the terminal"
task :hello do
  puts "hello from Rake!"
end

desc "Output hola to terminal"

task :hola do
  puts "hola de Rake!"

end
end




namespace :db do

task :environment do
require_relative './config/environment'

end

  desc 'migrating your changes to database'
  task migrate: :environment do
    Student.create_table
  end

desc "Seed the database with some dummy data"
task seed: :environment do
  require_relative './db/seeds'
end

end
desc 'Drop into the pry console'


task :environment do
require_relative './config/environment'

end

task console: :environment do
Pry.start
end


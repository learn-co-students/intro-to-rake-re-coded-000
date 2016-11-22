desc 'greeting name space'
namespace :greeting do
  desc 'print out hello to the terminal'
  task :hello do
    puts 'hello from Rake!'
  end
  desc 'print out hola to the terminal'
  task :hola do
    puts 'hola de Rake!'
  end
end
  desc 'migrate changes to database'
  namespace :db do
  task :environment do
    require_relative './config/environment.rb'
  end
    desc 'create a table'
    task :migrate => :environment do
      Student.create_table
    end
    desc 'seed the database with dummy data'
    task :seed do
      require_relative './db/seeds.rb'
    end
  end

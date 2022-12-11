namespace :greeting do
  desc 'outputs hola to the terminal' 
      task :hola do
        puts "hola de Rake!"
      end
      
      desc 'outputs hello to the termianl'
      task :hello do
        puts "hello from Rake!"
      end
  end
  
  task :console do
    "Make sure you have a 'console' rake task"
  end 
  
  namespace :db do  
    desc 'migrate changes to your database' 
    task migrate: :environment do  
      Student.create_table   
    end 
  
    desc "seed the database with some dummy data" 
    task seed: :environment do  
      require_relative './db/seeds'
    end
  end
  
  task :environment do 
    require_relative './config/environment'
  end

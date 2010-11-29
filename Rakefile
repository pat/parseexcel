$:.unshift('lib')
 
require 'rake/testtask'
require 'jeweler'

Jeweler::Tasks.new do |s|
  s.name               = 'parseexcel'
  s.email              = 'pat@freelancing-gods.com' 
  s.homepage           = 'http://github.com/freelancing-god/parseexcel'
  s.summary            = 'Parse Excel Files'
  s.description        = 'A basic interface for parsing Excel files.'
  s.authors            = ['Hannes Wyss', 'Hugh McGowan', 'Pat Allan']
  s.files              =  FileList[ "{lib,test}/**/*"]
  s.has_rdoc           = true
  s.extra_rdoc_files   = ["README", "COPYING"]
  s.rdoc_options       = ["--main","README"]
end

Rake::TestTask.new do |t|
  t.libs << "test"
  t.test_files = FileList['test/test*.rb']
  t.verbose = true
end

task :default => :test

require 'rubygems'
require 'rake'
require "rake/gempackagetask" 

PRAWN_GRAPH_VERSION = '0.0.2'

spec = Gem::Specification.new do |spec|
  spec.name = "prawn-graph"
  spec.version = PRAWN_GRAPH_VERSION
  spec.platform = Gem::Platform::RUBY
  spec.summary = "An extension to Prawn that provides the ability to draw basic graphs and charts natively in your PDFs."
  spec.files = Dir.glob("{examples,lib,spec,vendor,data}/**/**/*") +
                      ["Rakefile"]
  spec.require_path = "lib"
  
  spec.test_files = Dir[ "test/*_test.rb" ]
  spec.has_rdoc = true
  spec.extra_rdoc_files = %w{README.markdown}
  spec.rdoc_options << '--title' << 'Prawn Documentation' <<
                       '--main' << 'README.markdown' << '-q'
  spec.author = "Ryan Stenhouse"
  spec.email = " ryan@ryanstenhouse.eu"
  spec.rubyforge_project = "prawn"
  spec.homepage = "http://ryanstenhouse.eu"
  spec.description = <<END_DESC
  An extension to Prawn that provides the ability to draw basic graphs and charts natively in your PDFs.
END_DESC
end
 
Rake::GemPackageTask.new(spec) do |pkg|
  pkg.need_zip = true
  pkg.need_tar = true
end
 

def compile_source(options = {})
    options = {type: 'sass'}.merge(options)
    system("sass stylesheets/#{options[:type]}/#{options[:file]}.#{options[:type]}:stylesheets/#{options[:file]}")
end

desc "Compile SCSS Source Files to stylesheets/"
task :compile_scss do
    puts "\n## Compiling SCSS Source Files"
    print "\nCompiling global.scss ... "
    status = compile_source(file: "global.css", type: "scss")
    puts status ? "Success" : "Failed"
    print "\nCompiling layout.scss ... "
    status = compile_source(file: "layout.css", type: "scss")
    puts status ? "Success" : "Failed"
    puts
end

desc "Compile SASS Source Files to stylesheets/"
task :compile_sass do
    puts "\n## Compiling SCSS Source Files"
    puts "\n\tCompiling global.sass ... "
    status = compile_source(file: "global.css", type: "sass")
    puts status ? "Success" : "Failed"
    print "\nCompiling layout.sass ... "
    status = compile_source(file: "layout.css", type: "sass")
    puts status ? "Success" : "Failed"
end

task :default => [:compile_scss]
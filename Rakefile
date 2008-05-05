desc "Compile scripts to .scpt files"
task :compile do
  puts "Compiling center.applescript..."
  system "osacompile -o center.scpt center.applescript"
  puts "Compiling center.applescript..."  
  system "osacompile -o maximize.scpt maximize.applescript"
  puts "Done"
  puts
end

desc "Install scripts to your scripts folder"
task :install => :compile do
  puts "Copying scripts to your scripts folder"
  system "cp *.scpt ~/Library/Scripts"
  puts "Done"
  puts
end

desc "Download and mount FastScripts"
task :install_fastscripts do
  system "curl http://www.red-sweater.com/fastscripts/FastScriptsLite2.3.6.dmg > FastScripts.dmg"
  system "hdiutil attach FastScripts.dmg"
  puts "FastScripts Lite is now mounted in your system. Opening the folder..."
  sleep 1
  system "open \"/Volumes/FastScripts Lite 2.3.6\""
end
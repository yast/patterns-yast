# Copyright (c) 2017 SUSE LINUX GmbH, Nuernberg, Germany.
# All Rights Reserved.
#
# This program is free software; you can redistribute it and/or
# modify it under the terms of the MIT License.
#

require "yast/rake"

Yast::Tasks.submit_to :sle15sp5

# do not create a tarball, this package contains only a .spec file
Rake::Task["tarball"].clear_actions

# redefine the version:bump task, this package uses a date as the version number
Rake::Task["version:bump"].clear

namespace :version do
  desc "Set the version number in the package/*.spec file to the current date"
  task :bump do
    new_version = Time.now.strftime("%Y%m%d")
    puts "Updating version to #{new_version}"

    # update all present *.spec files
    Dir.glob("package/*.spec").each do |spec_file|
      spec = File.read(spec_file)
      spec.gsub!(/^\s*Version:.*$/, "Version:        #{new_version}")

      File.write(spec_file, spec)
    end
  end
end


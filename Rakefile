require 'html-proofer'

task :test do
  sh "bundle exec jekyll build"
  options = {
    assume_extension: true,
    disable_external: true,
    url_swap: {
      # https://github.com/18F/guides-style/pull/107
      /^\#$/ => '#top'
    }
  }
  HTMLProofer.check_directory("./_site", options).run
end

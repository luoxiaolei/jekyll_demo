### 简介
> Jekyll is a simple, extendable, static site generator. You give it text written in your favorite markup language and it churns through layouts to create a static website. Throughout that process you can tweak how you want the site URLs to look, what data gets displayed in the layout, and more.

### 安装
1. [Install a full Ruby development environment](https://luoxiaolei.github.io/2019/05/26/Mac-install-rbenv-&-ruby.html)
2. Install Jekyll and bundler gems

```
gem install jekyll bundler
----------------------------
Fetching safe_yaml-1.0.5.gem
Fetching forwardable-extended-2.6.0.gem
Fetching liquid-4.0.3.gem
Fetching kramdown-1.17.0.gem
Fetching ruby_dep-1.5.0.gem
Fetching rouge-3.3.0.gem
Fetching pathutil-0.16.2.gem
Fetching mercenary-0.3.6.gem
Fetching ffi-1.11.1.gem
Fetching rb-inotify-0.10.0.gem
Fetching rb-fsevent-0.10.3.gem
Fetching listen-3.1.5.gem
Fetching jekyll-watch-2.2.1.gem
Fetching sass-listen-4.0.0.gem
Fetching sass-3.7.4.gem
Fetching jekyll-sass-converter-1.5.2.gem
Fetching concurrent-ruby-1.1.5.gem
Fetching i18n-0.9.5.gem
Fetching http_parser.rb-0.6.0.gem
Fetching eventmachine-1.2.7.gem
Fetching em-websocket-0.5.1.gem
Fetching colorator-1.1.0.gem
Fetching public_suffix-3.0.3.gem
Fetching addressable-2.6.0.gem
Fetching jekyll-3.8.5.gem
Successfully installed safe_yaml-1.0.5
Successfully installed rouge-3.3.0
Successfully installed forwardable-extended-2.6.0
Successfully installed pathutil-0.16.2
Successfully installed mercenary-0.3.6
Successfully installed liquid-4.0.3
Successfully installed kramdown-1.17.0
Successfully installed ruby_dep-1.5.0
Building native extensions. This could take a while...
Successfully installed ffi-1.11.1
Successfully installed rb-inotify-0.10.0
Successfully installed rb-fsevent-0.10.3
Successfully installed listen-3.1.5
Successfully installed jekyll-watch-2.2.1
Successfully installed sass-listen-4.0.0

Ruby Sass has reached end-of-life and should no longer be used.

* If you use Sass as a command-line tool, we recommend using Dart Sass, the new
  primary implementation: https://sass-lang.com/install

* If you use Sass as a plug-in for a Ruby web framework, we recommend using the
  sassc gem: https://github.com/sass/sassc-ruby#readme

* For more details, please refer to the Sass blog:
  https://sass-lang.com/blog/posts/7828841

Successfully installed sass-3.7.4
Successfully installed jekyll-sass-converter-1.5.2
Successfully installed concurrent-ruby-1.1.5
Successfully installed i18n-0.9.5
Building native extensions. This could take a while...
Successfully installed http_parser.rb-0.6.0
Building native extensions. This could take a while...
Successfully installed eventmachine-1.2.7
Successfully installed em-websocket-0.5.1
Successfully installed colorator-1.1.0
Successfully installed public_suffix-3.0.3
Successfully installed addressable-2.6.0
Successfully installed jekyll-3.8.5
Parsing documentation for safe_yaml-1.0.5
Installing ri documentation for safe_yaml-1.0.5
Parsing documentation for rouge-3.3.0
Installing ri documentation for rouge-3.3.0
Parsing documentation for forwardable-extended-2.6.0
Installing ri documentation for forwardable-extended-2.6.0
Parsing documentation for pathutil-0.16.2
Installing ri documentation for pathutil-0.16.2
Parsing documentation for mercenary-0.3.6
Installing ri documentation for mercenary-0.3.6
Parsing documentation for liquid-4.0.3
Installing ri documentation for liquid-4.0.3
Parsing documentation for kramdown-1.17.0
Installing ri documentation for kramdown-1.17.0
Parsing documentation for ruby_dep-1.5.0
Installing ri documentation for ruby_dep-1.5.0
Parsing documentation for ffi-1.11.1
Installing ri documentation for ffi-1.11.1
Parsing documentation for rb-inotify-0.10.0
Installing ri documentation for rb-inotify-0.10.0
Parsing documentation for rb-fsevent-0.10.3
Installing ri documentation for rb-fsevent-0.10.3
Parsing documentation for listen-3.1.5
Installing ri documentation for listen-3.1.5
Parsing documentation for jekyll-watch-2.2.1
Installing ri documentation for jekyll-watch-2.2.1
Parsing documentation for sass-listen-4.0.0
Installing ri documentation for sass-listen-4.0.0
Parsing documentation for sass-3.7.4
Installing ri documentation for sass-3.7.4
Parsing documentation for jekyll-sass-converter-1.5.2
Installing ri documentation for jekyll-sass-converter-1.5.2
Parsing documentation for concurrent-ruby-1.1.5
Installing ri documentation for concurrent-ruby-1.1.5
Parsing documentation for i18n-0.9.5
Installing ri documentation for i18n-0.9.5
Parsing documentation for http_parser.rb-0.6.0
unknown encoding name "chunked\r\n\r\n25" for ext/ruby_http_parser/vendor/http-parser-java/tools/parse_tests.rb, skipping
Installing ri documentation for http_parser.rb-0.6.0
Parsing documentation for eventmachine-1.2.7
Installing ri documentation for eventmachine-1.2.7
Parsing documentation for em-websocket-0.5.1
Installing ri documentation for em-websocket-0.5.1
Parsing documentation for colorator-1.1.0
Installing ri documentation for colorator-1.1.0
Parsing documentation for public_suffix-3.0.3
Installing ri documentation for public_suffix-3.0.3
Parsing documentation for addressable-2.6.0
Installing ri documentation for addressable-2.6.0
Parsing documentation for jekyll-3.8.5
Installing ri documentation for jekyll-3.8.5
Done installing documentation for safe_yaml, rouge, forwardable-extended, pathutil, mercenary, liquid, kramdown, ruby_dep, ffi, rb-inotify, rb-fsevent, listen, jekyll-watch, sass-listen, sass, jekyll-sass-converter, concurrent-ruby, i18n, http_parser.rb, eventmachine, em-websocket, colorator, public_suffix, addressable, jekyll after 41 seconds
Successfully installed bundler-2.0.1
Parsing documentation for bundler-2.0.1
Done installing documentation for bundler after 1 seconds
26 gems installed
```

3. Create a new Jekyll site at ./myblog

```
jekyll new myblog
----------------------------------------
Running bundle install in /Users/luoxiaolei/Documents/project/ruby/myblog... 

  Bundler: Fetching gem metadata from https://rubygems.org/...............
  Bundler: Fetching gem metadata from https://rubygems.org/..
  Bundler: Resolving dependencies...
  Bundler: Using public_suffix 3.0.3
  Bundler: Using addressable 2.6.0
  Bundler: Using bundler 2.0.1
  Bundler: Using colorator 1.1.0
  Bundler: Using concurrent-ruby 1.1.5
  Bundler: Using eventmachine 1.2.7
  Bundler: Using http_parser.rb 0.6.0
  Bundler: Using em-websocket 0.5.1
  Bundler: Using ffi 1.11.1
  Bundler: Using forwardable-extended 2.6.0
  Bundler: Using i18n 0.9.5
  Bundler: Using rb-fsevent 0.10.3
  Bundler: Using rb-inotify 0.10.0
  Bundler: Using sass-listen 4.0.0
  Bundler: Using sass 3.7.4
  Bundler: Using jekyll-sass-converter 1.5.2
  Bundler: Using ruby_dep 1.5.0
  Bundler: Using listen 3.1.5
  Bundler: Using jekyll-watch 2.2.1
  Bundler: Using kramdown 1.17.0
  Bundler: Using liquid 4.0.3
  Bundler: Using mercenary 0.3.6
  Bundler: Using pathutil 0.16.2
  Bundler: Using rouge 3.3.0
  Bundler: Using safe_yaml 1.0.5
  Bundler: Using jekyll 3.8.5
  Bundler: Fetching jekyll-feed 0.12.1
  Bundler: Installing jekyll-feed 0.12.1
  Bundler: Fetching jekyll-seo-tag 2.6.1
  Bundler: Installing jekyll-seo-tag 2.6.1
  Bundler: Fetching minima 2.5.0
  Bundler: Installing minima 2.5.0
  Bundler: Bundle complete! 4 Gemfile dependencies, 29 gems now installed.
  Bundler: Use `bundle info [gemname]` to see where a bundled gem is installed.The dependency tzinfo-data (>= 0) will be unused by any of the platforms Bundler is installing for. Bundler is installing for ruby but the dependency is only for x86-mingw32, x86-mswin32, x64-mingw32, java. To add those platforms to the bundle, run `bundle lock --add-platform x86-mingw32 x86-mswin32 x64-mingw32 java`.
New jekyll site installed in /Users/luoxiaolei/Documents/project/ruby/myblog. 
```

4. Change into your new directory

```
cd myblog
```

5. Build the site and make it available on a local server

```
bundle exec jekyll serve
---------------------------------------
Configuration file: /Users/luoxiaolei/Documents/project/ruby/myblog/_config.yml
            Source: /Users/luoxiaolei/Documents/project/ruby/myblog
       Destination: /Users/luoxiaolei/Documents/project/ruby/myblog/_site
 Incremental build: disabled. Enable with --incremental
      Generating... 
       Jekyll Feed: Generating feed for posts
                    done in 0.399 seconds.
 Auto-regeneration: enabled for '/Users/luoxiaolei/Documents/project/ruby/myblog'
    Server address: http://127.0.0.1:4000/
  Server running... press ctrl-c to stop.

```

6. Now browse to http://localhost:4000


### 参考链接
- [Quickstart](https://jekyllrb.com/docs/)
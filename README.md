# Alggago
By [멋쟁이사자처럼](http://likelion.net).

## Install Ruby

### macOS

rbenv로 Ruby 설치 (version 2.2.5)

* Terminal 을 열고 다음의 명령어를 입력하여 rbenv를 설치한다.
```console
$ brew update
$ brew install rbenv ruby-build
```
* `rbenv -v`로 rbenv가 제대로 설치 되었는지 확인한다.
```console
$ rbenv -v
```
* rbenv가 제대로 설치된 것을 확인하였다면, 다음의 명령어를 입력하여 Ruby를 설치한다.
```console
$ rbenv install 2.2.5
$ rbenv global 2.2.5
```
* `ruby -v`로 Ruby가 제대로 설치 되었는지 확인한다.
```console
$ ruby -v
```

### Windows

RubyInstaller로 Ruby 설치 (Version 2.2.5)
* http://rubyinstaller.org/downloads 에서 본인의 컴퓨터가 32비트이면 `Ruby 2.2.5 `, 64비트이면 `Ruby 2.2.5 (x64)`를 다운로드 받아 설치한다.
* 설치 도중 나오는 `Add Ruby executables to your PATH`에 체크한다.
* CMD를 열고 `ruby -v`를 입력하여 Ruby가 제대로 설치 되었는지 확인한다.
```console
$ ruby -v
```

DEVELOPMENT KIT 설치 [[참고 사이트](https://github.com/oneclick/rubyinstaller/wiki/Development-Kit)]
* http://rubyinstaller.org/downloads 에서 본인의 컴퓨터에 해당하는 설치 파일을 다운로드 받는다.
* Ruby가 설치된 폴더 안에 새로운 폴더를 생성하여 그 곳에 압축을 푼다.
* CMD를 열고 압축을 푼 폴더로 이동하여 다음의 명령어를 입력한다.
```console
$ ruby dk.rb init
$ ruby dk.rb review
$ ruby dk.rb install
```

### Linux (Ubuntu)

rbenv로 Ruby 설치 (version 2.2.5)
* Terminal 을 열고 다음의 명령어를 입력하여 rbenv를 설치한다.
```console
$ git clone git://github.com/sstephenson/rbenv.git .rbenv
$ echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
$ echo 'eval "$(rbenv init -)"' >> ~/.bashrc

$ git clone git://github.com/sstephenson/ruby-build.git ~/.rbenv/plugins/ruby-build
$ echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc

$ source ~/.bashrc
```
* `rbenv -v`로 rbenv가 제대로 설치 되었는지 확인한다.
```console
$ rbenv -v
```
* rbenv가 제대로 설치된 것을 확인하였다면, 다음의 명령어를 입력하여 Ruby를 설치한다.

```console
$ rbenv install 2.2.5
$ rbenv global 2.2.5
```
* `ruby -v`로 Ruby가 제대로 설치 되었는지 확인한다.
```console
$ ruby -v
```

## Install Alggago

### Using Git
```console
$ git clone https://github.com/likelion-campus/alggago.git
```

### Using 'Download ZIP'

`Download ZIP` 링크로 다운로드 받아 편한 곳에 압축을 푼다.

## Install Dependencies
Alggago 실행을 위한 gem을 설치한다.
```console
$ gem install gosu chipmunk slave childprocess
```

## Run
```console
$ ruby alggago.rb
```

### AI vs. Uesr
`alggago.rb` 파일과 같은 위치에 `ai_[name].rb` 파일 __하나__를 둔다.

### AI vs. AI
`alggago.rb` 파일과 같은 위치에 `ai_[name].rb` 파일 __둘__을 둔다.

## Make Your Own Alggago Code
`ai_black.rb` 파일의 다음 부분을 수정하여 Alggago AI를 만든다.

```ruby
class MyAlggago
  def calculate(positions)

    #Codes here

      #Insert Your Codes here

    #Return values
    ...
      #Don't touch 'Return values' codes

    #Codes end
  end
```

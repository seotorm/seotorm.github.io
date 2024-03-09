---
layout: default
title: Ruby Version Up in macOS
nav_order: 3
---
# Ruby Version Up in macOS
## Homebrew 설치
Homebrew는 macOS용 패키지 관리 프로그램.
설치 방법은 [Homebrew Site] 참조

## Homebrew 로 rbenv 설치
```shell
$ brew install rbenv
```

## rbenv로 Ruby 설치
설치 가능한 Ruby Version 확인.
```shell
$ rbenv install -l
3.0.6
3.1.4
3.2.3
3.3.0
jruby-9.4.6.0
mruby-3.3.0
picoruby-3.0.0
truffleruby-23.1.2
truffleruby+graalvm-23.1.2

Only latest stable releases for each Ruby implementation are shown.
Use `rbenv install --list-all' to show all local versions.
```
원하는 버전 설치
```shell
$ rbenv install 3.3.0
```
설치 버전 활성화
```shell
$ rbenv global 3.3.0
```
설치 버전 확인
```shell
$ rbenv version 
$ ruby version 
```
버전 정보가 활성화 되지 않은 경우 다음을 실행하여 안내에 따른다.  
(`.zshrc`에 마지막 줄 추가)
```shell
$ rbenv init
# Load rbenv automatically by appending
# the following to ~/.zshrc:

eval "$(rbenv init - zsh)"
```
`.zshrc` 수정 후 터미널을 새로 실행한 다음 설치 버전을 확인한다.

(끝)

---
[Homebrew Site]: https://brew.sh/

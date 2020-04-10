# Tools

## AdoptOpenJDK 8

Prebuilt OpenJDK 8 Binaries

**URL:** [https://adoptopenjdk.net](https://adoptopenjdk.net/)

	brew cask install adoptopenjdk8

### Other Versions:

**URL:** https://github.com/AdoptOpenJDK/homebrew-openjdk

	brew tap AdoptOpenJDK/openjdk
	brew cask install <version>

	brew cask install adoptopenjdk11
	brew cask install adoptopenjdk13

### Switch Versions:

Add the following aliases to `.bash_profile` or `.bashrc`

	export JAVA_8_HOME=$(/usr/libexec/java_home -v1.8)
	export JAVA_11_HOME=$(/usr/libexec/java_home -v11)
	export JAVA_13_HOME=$(/usr/libexec/java_home -v13)
	#export JAVA_HOME=$JAVA_8_HOME

	alias java8='export JAVA_HOME=$JAVA_8_HOME'
	alias java11='export JAVA_HOME=$JAVA_11_HOME'
	alias java13='export JAVA_HOME=$JAVA_13_HOME'

switch version

	java11
	java -version


### SDK MAN

- https://sdkman.io/jdks
- https://sdkman.io/sdks


## DBeaver Community

Free multi-platform database tool for developers, SQL programmers, database administrators and analysts. Supports all popular databases

**URL:** [https://dbeaver.io](https://dbeaver.io/)

	brew cask install dbeaver-community


## FakeSMTP

FakeSMTP is a Free Fake SMTP Server with GUI for testing emails in applications easily. It is written in Java.
Configure your application to use "localhost" as your SMTP server, and all emails will be intercepted and displayed in this software.

**URL:** [http://nilhcem.com/FakeSMTP](http://nilhcem.com/FakeSMTP)


## HTTPie
User-friendly cURL replacement (command-line HTTP client)

**URL:** [https://httpie.org](https://httpie.org/)

	brew install httpie

**Usage:**

	http :8080/
	http --verify=no https://localhost:9443/
	http --headers www.google.com
	http http://jsonplaceholder.typicode.com/users


## IntelliJ IDEA CE
IntelliJ IDEA is a Java integrated development environment (IDE) for developing computer software. It is developed by JetBrains 

**URL:** [https://www.jetbrains.com/idea](https://www.jetbrains.com/idea/)

	brew cask install intellij-idea-ce

### Jetbrains Toolbox

	brew cask install jetbrains-toolbox

## iTerm2
iTerm2 is a replacement for Terminal and the successor to iTerm. It works on Macs with macOS 10.12 or newer. iTerm2 brings the terminal into the modern age with features you never knew you always wanted.

**URL:** [https://www.iterm2.com](https://www.iterm2.com/)

	brew cask install iterm2


## jq
Lightweight and flexible command-line JSON processor

**URL:** [https://stedolan.github.io/jq](https://stedolan.github.io/jq/)

	brew install jq
	
**Usage:**

	http https://jsonplaceholder.typicode.com/users | jq
	http https://jsonplaceholder.typicode.com/users | jq '.[0]'
	http https://jsonplaceholder.typicode.com/users | jq '.[] | {name: .name, email: .email}'


## MacDown
MacDown is an open source Markdown editor for macOS

**URL:** [https://macdown.uranusjr.com](https://macdown.uranusjr.com/)

	brew cask install macdown

## mkcert
A simple zero-config tool to make locally trusted development certificates with any names you'd like.

**URL:** https://github.com/FiloSottile/mkcert

	brew install mkcert
	brew install nss

**Usage:**

Install local CA

	mkcert -install

	Using the local CA at "/Users/username/Library/Application Support/mkcert" ✨
	The local CA is now installed in the system trust store! ⚡️
	The local CA is now installed in the Firefox trust store (requires browser restart)! 🦊

Create Certificates

	mkcert example.com "*.example.com" localhost 127.0.0.1 ::1

	The certificate is at "./example.com+5.pem" and the key at "./example.com+5-key.pem" ✅


## Maven
Java-based project management

**URL:** [https://maven.apache.org/](https://maven.apache.org)

	brew install maven

## nmap

	nmap --script ssl-enum-ciphers -p 443 example.com


## NVM
Node Version Manager

**URL:** [https://github.com/nvm-sh/nvm](https://github.com/nvm-sh/nvm)

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
```

The script clones the nvm repository to `~/.nvm` and adds the source line to your profile (`~/.bash_profile`, `~/.zshrc`, `~/.profile`, or `~/.bashrc`).

```bash
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion
```

**Usage:**

	nvm install --lts
	nvm ls
	nvm use --lts
	nvm use <version>

## scdl
Soundcloud Music Downloader

**URL:** https://github.com/flyingrub/scdl

	pip3 install scdl

**Usage:**

	scdl -l $url --path ~/storage/music


## Serveo.net
Expose local servers to the internet. No installation, no signup

	ssh -R 80:localhost:3000 serveo.net


## SSLyze
Fast and powerful SSL/TLS server scanning library

**URL:** [https://github.com/nabla-c0d3/sslyze](https://github.com/nabla-c0d3/sslyze)

	brew install sslyze

**Usage:**

	sslyze --regular --http_headers www.google.com

## tcpkali
High performance TCP and WebSocket load generator and sink

**URL:** [https://github.com/machinezone/tcpkali](https://github.com/machinezone/tcpkali)

	brew install tcpkali

**Usage:**

	TODO


## Thai Dict
Thai-Eng Dictionary by Infinisoft

	brew cask install thai-dict


## Thai National Fonts
13 Thai National Fonts by SIPA

	brew cask install thai-national-fonts

## tldr
The TLDR pages are a community effort to simplify the beloved man pages with practical examples.

**URL:** https://tldr.sh

	brew install tldr

**Usage:**

	tldr git rebase


## Typora
Typora will give you a seamless experience as both a reader and a writer. It removes the preview window, mode switcher, syntax symbols of markdown source code

**URL:** [https://typora.io](https://typora.io/)

	brew cask install typora


## VisualVM
VisualVM is a visual tool integrating commandline JDK tools and lightweight profiling capabilities. Designed for both development and production time use.

URL: [https://visualvm.github.io](https://visualvm.github.io/)

	brew cask install visualvm

## Visual Studio Code
Microsoft Visual Studio Code

**URL:** [https://code.visualstudio.com](https://code.visualstudio.com/)

	brew cask install visual-studio-code


## WRK
HTTP benchmarking tool

**URL:** [https://github.com/wg/wrk](https://github.com/wg/wrk)

	brew install wrk
	
**Usage:**

	wrk -c100 -d30s -t4 http://localhost:8080/

## youtube-dl
youtube-dl is a command-line program to download videos from YouTube.com and a few more sites.

**URL:** https://github.com/ytdl-org/youtube-dl

	brew install youtube-dl

**Usage:**

	youtube-dl -f 'bestvideo[ext=mp4]+bestaudio[ext=m4a]/mp4'
	youtube-dl -x --embed-thumbnail --audio-format mp3


## Presentation

### hacker-slides
A small UI for building presentation slides from markdown markup. (revealjs)

**URL:** https://github.com/msoedov/hacker-slides

### revealgo
Markdown driven presentation tool written in Go!

**URL:** https://github.com/yusukebe/revealgo

	go get github.com/yusukebe/revealgo/cmd/revealgo

**Usage:**

	revealgo [options] MARKDOWN.md

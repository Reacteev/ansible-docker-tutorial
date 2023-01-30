# ansible docker tutorial

## How to

This script allows you to play locally on a docker environment an interactive ansible tutorial.
If you don't have the possibility to install a docker environment you can register to [Play with Docker](https://labs.play-with-docker.com/) and use a 4h session to play.

It will start 3 containers:
- 1 ansible server you will use to play the tutorial
- 2 hosts to deploy the content of the tutorial playbooks.

Each host will open 2 http ports to use 80 & 8080 mapped to a local port of your environment
Here is the default mapping:
- localhost:33001 --> host1:80
- localhost:33002 --> host1:8080
- localhost:33003 --> host2:80
- localhost:33004 --> host2:8080

Once the project is cloned in your local environment, add the executing privileges and launch the script
```
git clone git@gitlab.com:eric.boudeville/ansible-docker-tutorial.git
cd ansible-docker-tutorial
chmod a+x tutorials.sh
./tutorials.sh
```

## License
Copyright (c) 2022, Eric Boudeville eric.boudeville@reacteev.com
All rights reserved.
Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
THIS SOFTWARE IS PROVIDED BY THE AUTHOR AND CONTRIBUTORS AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE AUTHOR OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

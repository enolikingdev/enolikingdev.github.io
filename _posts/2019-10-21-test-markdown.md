---
layout: post
title: Find files and open them
tags: [linux]
comments: true
---
From the current folder look for files with the name 'Dockerfile', contining the text 'jenkins-slave-jdk-open', and just list them on the standard output.
~~~
find . -type f -name Dockerfile -exec grep -l 'jenkins-slave-jdk-open' {} +
~~~
Use the output of the first command, with each line as an argument open Visual Studio Code.
~~~
find . -type f -name Dockerfile -exec grep -l 'jenkins-slave-jdk-open' {} + | xargs -I{} code {}
~~~

---
layout: post
title: PostgreSQL cheat sheet
description: "Some useful information for PostgreSQL users."
modified: 2014-07-20
tags: [postgresql]
image:
  feature: abstract-10.jpg
comments: true
share: true  
---

This post will be updated with any cool cheats/commands that I use on a daily basis, that may help others out.

### Make a local user, superuser

Everytime I work on a new machine/enviroment I need to be able to create and delete databases as a local
user quickly and easily, I am by no means a PostgreSQL expert, but I need to be able to create databases,
ready for web application development. So the below code should get you started.

First, login as the potgres user, and access the psql shell:

{% highlight bash %}
$ sudo su - postgres
$ psql
{% endhighlight %}

Now, we need to create a new postgres user, for the sakes of this guide, lets assume the name
"luke" and obviously replace 'somepassword' with your own, secure password.

{% highlight sql %}
postgres=# create user luke with password 'somepassword';
CREATE ROLE
{% endhighlight %}

Now we have the user setup, lets give him 'Super User' credentials:

{% highlight sql %}
postgres=# ALTER USER luke with SUPERUSER;
ALTER ROLE
{% endhighlight %}

Now, open up a new termianl and you should be able to create and delete databases:

{% highlight bash %}
$ createdb staff
$ dropdb staff
{% endhighlight %}


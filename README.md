# diesel-demo

Example code from the [Getting Started](http://diesel.rs/guides/getting-started/) guide for Diesel.rs ORM. This code assumes usage of Postgresql.

### PostgreSQL Setup

Let's be honest, setting up postgres can be a PITA and what we really want to do is forget about config for a second and get coding.

Here's a Docker one-liner to start a postgres server container:

{% highlight docker %}
docker run --rm --detach --name postgres --env POSTGRES_USER=username --env POSTGRES_PASSWORD=password --publish 127.0.0.1:5432:5432 postgres
{% endhighlight %}

You also need to install libpq-dev (or the equivalent for your OS):

{% highlight shell %}
sudo apt-get install libpq-dev
{% endhighlight %}

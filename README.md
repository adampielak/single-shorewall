Shorewall Single Interface
==========================

Shorewall configuration for outmail-sf and outmail-ny

#### Current Rules

* ssh from known IP (DNS) only
* SMTP from known network
* webmin access from known network

# Installtion

<pre>
<code>

apt-get install shorewall
rm -frv /etc/shorewall
git clone https://github.com/mckinnon81/single-shorewall.git /etc/shorewall
cd /etc/shorewall
git checkout ait

</code>
</pre>

To have shorewall start on start up

<pre>
<code>
vi /etc/default/shorewall
</code>
</pre>

Change
<pre>
<code>
startup=0
</code>
</pre>

to

<pre>
<code>
startup=1
</code>
</pre>

vDNS
=====

vDNS it's a simple script to consult dns and register on domain, is a tool recomended for sysadmins.

== How to use ==

Call script, argument and domain, eg:

* vdns [argument] [domain]

Full DNS lookup:

vdns -a domain.com

----

usage: vdns [-a] [-n] [-d] [-w] [-p] [-m] [-r] [-f] [-k] [-s] [-b] [-i] [domain] | [ -u update ] | [ -h --help ]

  Options:

        -a    |   --all         : Full DNS lookup
        -n    |   --ns          : Only return servers NS
        -d    |   --dns         : Only return servers NSR
        -w    |   --www         : Only return WWW
        -p    |   --ping        : Only return ping check on WWW
        -m    |   --mx          : Only return MX
        -r    |   --reverse     : Only return reverse
        -f    |   --spf         : Only return SPF
        -k    |   --dkim        : Only return DKIM
		-b    |   --br      	: Consult domain on registro.br
        -i    |   --int     	: Consults domain o nic.com
		-u    |   --update      : Verify if exist update
        -s    |   --save        : Save Query on txt file
		-h    |   --help      	: Shows available functions
  eg:

  * vdns -a domain.com
  * vdns -k domain.com
  * vdns -s domain.com


== Updates ==

<pre>
* 1.0 - First commit
* 1.1 - Bug correction for domain search on nic.com.
</pre>

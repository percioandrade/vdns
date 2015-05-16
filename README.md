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

<pre>
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
-B    |   --bind        : Print Query on bind format
-o    |   --office      : Print MX from Outlook

  eg:

  * vdns -a domain.com
  * vdns -k domain.com
  * vdns -s domain.com
</pre>

== Updates ==

<pre>
* 1.0 - First commit
* 1.1 - Bug correction for domain search on nic.com.
* 1.2 - Bug correction for query domains
* 1.3 - Update script to registro.br 2.0
*     - Added .es domain to check ( no public whois on this time )
*     - Correction to domain check
*     - Added webproxy for whois block on registro.br
* 1.4 - Added search for .es domains
*     - Several corrections made
*     - Improvements in layout
*     - Search Office records
*     - Additional check in registro.br
</pre>

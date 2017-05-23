vDNS
=====

vDNS it's a simple script to consult dns and register on domain, is a tool recomended for sysadmins.

== How to use ==

Call script, argument and domain, eg:

* vdns [argument] [domain]

Full DNS lookup:

vdns -a domain.com

----
<pre>
Usage: vdns -a -n -d -w -p -m -r -f -k -s -b -i -c domain
        -u -h

Options:
        -a      : Full DNS lookup
        -n      : Only return root servers
        -d      : Only return root NSR servers
        -p      : Only return ping check on WWW
        -m      : Only return MX
        -r      : Only return reverse
        -f      : Only return SPF
        -k      : Only return DKIM
        -o      : Only return Office values
        -c      : Consult domain registrar situation
        -l      : Check propagation from domain in World
        -b      : Show DNS zones for domain in bind format
        -u      : Verify if exist update
        -s      : Save Query on txt file
        -h      : Shows available options

        eg:
        vdns -a domain.com
        vdns -k domain.com
        vdns -s domain.com
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
* 1.5 - 
*     - Change query in registro.br due to client removal 'isavail'
*     - Fixed domain check .es
*     - Fixed domain verify input (.com/.br etc)
*     - Added check if packages perl-libwww and perl-IO-Sockets is installed #Thanks for Alessandro Maia for report
*     - Added update url check for vDNS ( now is working :D )
*     - Added registro.br variable for url consult $REG_BR_WHOIS
*     - Change of query of the domain situation in the registro.br due to the removal of the protocol 'isavailble' 
*     - Changes in help layout function
*     - Added propagation function check for domain
*     - Added option show in bind format
*     - Added option fast consult in Google Servers
*     - And a lot of bugs corrected
</pre>

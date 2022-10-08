# Records
	- `A` : IPv4
	- `AAAA` : IPv6
	- `CNAME` : hostname to hostname
		- 🚨 only works for nonROOT domains (ex: something.mydomain.com)
	- `Alias` : hostname to AWS service
		- work for ROOT and nonRoot domains (app.mydomain.com 👉 blabla.amazonaws.com)
		- free
		- have native health checks
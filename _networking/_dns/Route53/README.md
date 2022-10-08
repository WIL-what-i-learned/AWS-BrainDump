# Route53

> MANAGED Domain Name Service (DNS) service

- `$0.50` / month / hosted zone
- Check that it is setup correctly
	- `nslookup` 👉 `nslookup <url>`
	- `dig` 👉 `dig <url>`
- Automatically performs health checks on resources



-----

## Time to Live

> mandatory for all DNS

- HIGH = 24hours (less traffic on DNS 👉 possibility of outdated records)
- LOW = 60s (very easy to change records)


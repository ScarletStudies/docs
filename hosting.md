# Hosting Concerns

## Web Host

The frontend and backend are hosted together on a single digital ocean droplet.

Expected costs: $5/mo

In order to scale, backend and frontend can be split to separate droplets/hosts. The frontend can be trivially scaled horizontally or vertically, as its only static files to serve. The backend may require some care when scaling horizontally, as the database would need to be decoupled from the current docker-compose setup.

## Backups

Use `mysqldump` nightly, uploading to digital ocean spaces.

Expected costs: $5/mo

## Email

Email is provided by mailgun, using SMTP.

Expected costs: $0/mo

### Email testing

Email is tested using mailtrap.

Expected costs: $0/mo

## SSL

SSL provided by let's encrypt.

Expected costs: $0/mo

## Domain

Domain provided by namecheap.

Expected costs: $12/yr

## Total

Annual dues: $12
Monthly dues: $10
# static-webpage-setup
Setup a static webpage in a droplet

Tutorial referencenced from this [post](https://medium.com/@devalshah1619/hosting-a-static-website-on-digital-ocean-for-free-in-under-5-mins-31398e3d503d)

Change `domain.tld` to your webpage domain for easy referencing

### create directory where webpage would be cloned into
`sudo mkdir /srv/www /srv/www/domain.tld`

### change where nginx would load webpage from
`nano /etc/nginx/sites-available/default`

### edit this line accordingly
`root /srv/www/domain.tld`

### restart server
`sudo service nginx restart`

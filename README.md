# foolscap-newsletter
https://github.com/swanson/capuchin

# install
```
gem install capuchin
gem install commander
```

# create email
```
# from foolscap-newsletter directory:
capuchin create "Foolscap 20xx - catch subject here"
```
# upload to mailchimp
```
# schedule will error, but upload newsletter 
# each run will create a new newsletter on mailchimp
capuchin schedule _emails/<filename> 
```
# send test email https://us1.admin.mailchimp.com/campaigns/



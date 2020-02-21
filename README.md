# foolscap-newsletter
https://github.com/swanson/capuchin

# install
```
gem install capuchin
gem install commander
```

# configure
MAILCHIMP_API_KEY goes in .env (don't check into git)

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


# update mailchimp template
- duplicate last foolscap template (ex "2020 Foolscap HTML Template.html")
- edit dates & years
- go to Mail Chimp Dashboard; Brands->Templates; Create Template; Import HTML
- select edited template html file and name it with Foolscap YEAR
## update capuchin to use new template
- select template
- copy url (https://us1.admin.mailchimp.com/templates/design?tid=392729)
- the number after tid is the template identifer
- edit _config.yml, change template_id to template identfier from url
## check changed into git
- doo iit

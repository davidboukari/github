### Create a developper oauth ###

github.com -> Settings ->  Developer settings -> oauth apps

- Application name: 
- Homepage URL: The url than you come from
- Application description: 
- Authorization callback URL: github will redirect to this url with a code=xxx as parameter 

### Check you rights ###

* curl --user 'xxxxxxx'  --url 'https://api.github.com/authorizations'

### In the navigator tests the url => Then validate if it is necessary ###

- curl --user 'xxxxxx'  https://github.com/login/oauth/authorize?client_id=xxxxxxxxxxxxxx1&client_secret=xxxxxxxxxxxxxxxxxxx

### In the navigator tests the url ###

* curl --user 'xxxxxxxxxxx'  --url 'https://api.github.com/authorizations' --data '{"client_id": "xxxxxxxxxxxxxxx","client_secret": "xxxxxxxxxxxxxxxxxxx"'

Enter host password for user 'xxxxxxxxxxxxx':
{
  "id": xxxxxxxxxxx,
  "url": "https://api.github.com/authorizations/xxxxx",
  "app": {
    "name": "myappname",
    "url": "https://......",
    "client_id": "xxxxxxxx"
  },
  "token": "xxxxxxxxxxxxxxxxxxxx",
  "hashed_token": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "token_last_eight": "xxxxxxxxx",
  "note": null,
  "note_url": null,
  "created_at": "2019-10-20T09:20:04Z",
  "updated_at": "2019-10-20T09:20:04Z",
  "scopes": [

  ],
  "fingerprint": null
}




# Vanilla-js Auth Example

how to sign up and login using supabase and supabase-js

<img width="558" alt="image" src="https://user-images.githubusercontent.com/458736/88377414-b6fb4180-cdd1-11ea-8061-103ec4577b7b.png">

### running
`npm install`
`npm run dev`

if you want to make changes without restarting the server run this in a different terminal window:
`npm run watch`

### testing auth endpoint from the command line

you can also do the following to test the auth endpoints manually:
```bash
# manual signup from terminal
 curl --header "Content-Type: application/json" \
   --request POST \
   --data '{"email":"some@email.com","password":"password"}' \
   <your-supabase-url>/auth/v1/signup?apikey=<your-api-key>

# manual login from terminal
 curl --header "Content-Type: application/json" \
   --request POST \
   --data '{"email":"some@email.com","password":"password"}' \
   "<your-supabase-url>/auth/v1/token?grant_type=password&apikey=<your-api-key>"
```

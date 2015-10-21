# s

Send and receive SMS from the command line

~~~ bash
s 15555555555 "Hey!"

s-list

watch -n 60 s-list

for number in $(cat phone-numbers); do
  s ${number} "Have you heard about s?"
end
~~~


## Dependencies

- [`curl`](http://curl.haxx.se/)
- [`pass`](http://www.passwordstore.org/)
- [`jq`](https://stedolan.github.io/jq/)

## Configuration

~~~ bash
pass insert twilio/account-sid
pass insert twilio/auth-token
pass insert twilio/phone-number
~~~

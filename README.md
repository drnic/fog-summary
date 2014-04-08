# fog-summary

Display summary of all accounts mentioned in `~/.fog` (or `$FOG_FILE`).

```
$ fog-summary --skip swisscom-cf-swifttest --skip bluebox-demo --skip attdfw2

default: AWS (PERSONAL_ACCESS_KEY)
AuthFailure => AWS was not able to validate the provided access credentials

starkandwayne: AWS (AKIAI7ZLXAD...)
servers: 3 - m1.small, m1.small, m1.small
Networking: unavailable

swblobstore: AWS (AKIAJ56O7S3CJFUZ....)
UnauthorizedOperation => You are not authorized to perform this operation.

customer1: OpenStack (https://identity.customer.com/v2.0/tokens / cftest)
servers: 16 - s1.micro, s1.small, s1.medium, s1.medium, s1.micro, s1.micro, s1.micro, s1.large, s1.micro, s1.small, s1.small, s1.medium, s1.micro, s1.micro, s1.small, s1.micro
subnets: Internal-VM-NET, Internal-L3-DEV, INTERNET, Internet Access, SW_CF_Internet
```

## Installation

Install via RubyGems:

    gem fog-summary

## Usage

Execute from the terminal:

    $ fog-summary
    $ fog-summary --skip key-to-skip


## Contributing

WARNING: This was a quick hack where all the code is in `bin/fog-summary`. If you really want to contribute; probably start the project from scratch.

1. Fork it ( http://github.com/drnic/fog-summary/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

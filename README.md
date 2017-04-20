# Devise example

  Example rais application that uses [Devise gem][1] for authorization. It uses additional
  confirmable and lockable modules.

## Running

1. Run ```bundle install``` in root directory to upload gems.

2. To create database run ```rake db:setup``` in root directory.

3. To be able to send emails, you should write your email credentials in **your_email** and **your_password** fields in ```envimonment/development.rb``` ( this app uses google smtp server to send emails, you need to provide your gmail account ), or you can use other stmp servers if you want.

  ```bash
  ....
  config.action_mailer.smtp_settings = {
    address:              'smtp.gmail.com',
    port:                 587,
    domain:               "gmail.com",
    user_name:            'your_email',
    password:             'your_password',
    authentication:       'plain'
  }
  ```
4. To run server use ```rails s``` command.


[1]: https://github.com/plataformatec/devise

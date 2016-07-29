# Overview
A simple module for developers allowing a user to specify custom message displayed when required form element empty.

See https://www.drupal.org/node/742344 for D8 discussion.

# Features

* Set custom error message:
  ```
  $form['message'] = array(
    '#type' => 'textarea',
    '#title' => t('Message'),
    '#required' => TRUE,
    '#required_error' => t('Please enter a message.'),
  );
  ```
* Works with any form element.

# Installation and configuration

* Required Error Message (required_error) module as usual (https://www.drupal.org/documentation/install/modules-themes/modules-7).
* Add `#required_error` to a form element.

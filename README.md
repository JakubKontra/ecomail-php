# PHP wrapper for Ecomail API

[![Build Status](https://travis-ci.org/Ecomailcz/ecomail-php.svg?branch=master)](https://travis-ci.org/Ecomailcz/ecomail-php)
[![Downloads this Month](https://img.shields.io/packagist/dm/ecomailcz/ecomail.svg)](https://packagist.org/packages/ecomailcz/ecomail)

# Instalation

```shell
composer require ecomailcz/ecomail
```

# Usage

```php
$ecomail = new Ecomail('API_KEY');
$ecomail->getListsCollection();
```

When there are more results, you will get `last_page` parameter in your response, which you can then use in another request.

```php
$ecomail->page(2)->getListsCollection();
```


You will find your API key in your account in "integrations" section.

# Available methods

All methods returns: `array stdClass string`

For more detailed documentation please visit: https://ecomailczv2.docs.apiary.io/

### getListsCollection

### addListCollection

### showList

### updateList

### getSubscribers

### getSubscriber

### addSubscriber

### removeSubscriber

### updateSubscriber

### addSubscriberBulk

### listCampaigns

### addCampaign

### updateCampaign

### sendCampaign

### listAutomations

### createTemplate

### listDomains

### createDomain

### deleteDomain

### sendTransactionalEmail

### sendTransactionalTemplate

### createNewTransaction

### triggerAutomation

# DCF Symfony Framework

***Notice: This framework is currently a prototype and a WIP.***

Uses the [Symfony Bundle System](https://symfony.com/doc/current/bundles.html)
to provide DCF Base Controller and common templates.  In the future it may be
updated to support other symfony bundle functionality which all DCF based applications
may use.

For more information on DCF see https://github.com/digitalcampusframework/dcf and
https://github.com/digitalcampusframework/dcf_starter.

This framework currently provides the following:
* Symfony Logger (not used but available)
* DCF Notice Support
* Common Page Header partial

## Examples ##

### DCF Notice ###
In controller:
```
$this->addDCFNoticeFlash(BaseController::FLASH_MESSAGE_TYPE_INFO, 'Success', 'Your lucky number has been generated.');
```
### Common Page Header ###
In template:
```
{{ include('@DCFFramework/partials/page-header.html.twig', {title: 'Home Page'}) }}
```

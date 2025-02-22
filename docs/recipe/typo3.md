<!-- DO NOT EDIT THIS FILE! -->
<!-- Instead edit recipe/typo3.php -->
<!-- Then run bin/docgen -->

# typo3

[Source](/recipe/typo3.php)



* Requires
  * [common](/docs/recipe/common.md)

## Configuration
### typo3_webroot
[Source](https://github.com/deployphp/deployer/blob/master/recipe/typo3.php#L11)

DocumentRoot / WebRoot for the TYPO3 installation

```php title="Default value"
'Web'
```


### shared_dirs
[Source](https://github.com/deployphp/deployer/blob/master/recipe/typo3.php#L26)

Overrides [shared_dirs](/docs/recipe/common.md#shared_dirs) from `recipe/common.php`.

Shared directories

```php title="Default value"
[
    '{{typo3_webroot}}/fileadmin',
    '{{typo3_webroot}}/typo3temp',
    '{{typo3_webroot}}/uploads'
]
```


### shared_files
[Source](https://github.com/deployphp/deployer/blob/master/recipe/typo3.php#L35)

Overrides [shared_files](/docs/recipe/common.md#shared_files) from `recipe/common.php`.

Shared files

```php title="Default value"
[
    '{{typo3_webroot}}/.htaccess'
]
```


### writable_dirs
[Source](https://github.com/deployphp/deployer/blob/master/recipe/typo3.php#L42)

Overrides [writable_dirs](/docs/recipe/deploy/writable.md#writable_dirs) from `recipe/deploy/writable.php`.

Writeable directories

```php title="Default value"
[
    '{{typo3_webroot}}/fileadmin',
    '{{typo3_webroot}}/typo3temp',
    '{{typo3_webroot}}/typo3conf',
    '{{typo3_webroot}}/uploads'
]
```



## Tasks

### deploy
[Source](https://github.com/deployphp/deployer/blob/master/recipe/typo3.php#L17)

Deploy your project.

Main TYPO3 task


This task is group task which contains next tasks:
* [deploy:prepare](/docs/recipe/common.md#deployprepare)
* [deploy:vendors](/docs/recipe/deploy/vendors.md#deployvendors)
* [deploy:publish](/docs/recipe/common.md#deploypublish)



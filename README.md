# lego

Repository for maintaining our custom template for [MyAAC], an account manager for Open Tibia.

## Modules

This template has only the following modules enabled:

- Account
- Community

Other modules are still reachable by inputting the correct URL, however, are likely not to function as originally intended.

Twitter and Facebook hooks have also been completely removed.

## Configuration

The configuration works exactly like `tibiacom`, aside from manually needing to import the `schema.sql` into your database. Otherwise all modules will be enabled as it defaults to `tibiacom`.

Additionally, since `news` is disabled, you have to change the `index` file for [MyAAC] then change `_REQUEST['p'] = 'news'` to `_REQUEST['p'] = 'accountmanagement'`. Since you can't redefine the `PAGE` or `URI` as they're constants and natively there is no way to change the index page another way.

## References

This template is based on the `tibiacom` template that comes with [MyAAC].

<!-- LINKS -->

[MyAAC]: https://github.com/slawkens/myaac

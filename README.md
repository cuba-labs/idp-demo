# CUBA IDP Add-on Demo

This repository demonstrates functionality of
[CUBA IDP Add-on](https://github.com/cuba-platform/idp-addon) and contains
[an example](https://github.com/cuba-platform/idp-addon/wiki/Single-Sign-On-Example)
of SSO implementation for two CUBA projects:

- `fish` - Identity Provider and Service Provider
- `chips` - Service Provider

Requires CUBA 7.1.0

## Usage

1. Configure the following aliases in your `hosts` file:

    | Address       | Alias         |
    |:------------- |:------------- |
    | 127.0.0.1     | fish          |
    | 127.0.0.1     | chips         |

2. Import and run both projects
3. Go to [http://fish:8081/app/](http://fish:8081/app/) in your web browser. You will be redirected to the IDP login page. Log in with the admin / admin credentials.
4. Go to [http://chips:8082/app/](http://chips:8082/app/) in the same web browser. If you are still logged in to the Fish application, you will be automatically logged in as admin to Chips.

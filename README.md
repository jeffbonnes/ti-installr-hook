# ti-installr-hook

A titanium cli hook for deploying builds to [installr](www.installrapp.com), based on [ti-testflight-hook](https://github.com/dbankier/ti-testflight-hook)

## Installation

~~~
$ npm install -g ti-installr-hook
~~~

## Usage

Add the installr api token to your tiapp.xml file.

~~~
  <property name="installr.api_token">ENTER_INSTALLR_API_TOKEN_HERE</property>
~~~


Use the `--installr` flag with the titanium cli to upload to installr. For example:

~~~
$ ti build -p ios -T dist-adhoc --installr
~~~

**You will be prompted for the release notes.**

You can also pass release notes using `--installr-release-notes` flag. For example:

~~~
$ ti build -p ios -T dist-adhoc --installr --installr-release-notes='New build with awesome features'
~~~

### Thanks to

- [dbankier](https://github.com/dbankier) for  [ti-testflight-hook](https://github.com/dbankier/ti-testflight-hook)



### Licence
Licensed under the [MIT License](http://opensource.org/licenses/MIT)
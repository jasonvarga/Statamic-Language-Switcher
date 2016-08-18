# Statamic Language Switcher (for v2.x)
> Create links to the corresponding content page in another language

When run on the English page `http://testsite.com/customers`

```
<a href="{{ lang_switch lang='fr' }}">Version Française</a>
<a href="{{ lang_switch lang='de' }}">Deutsche Version</a>
```

It could then create the following links:

```
<a href="http://testsite.fr/clientele">Version Française</a>
<a href="http://testsite.de/kunden">Deutsche Version</a>
```

### Required parameter:
* `lang`: enter the 2 letter language code for wich you want to show the localized link

### Optional parameters:

* `url`: Defaults to the current page.
* `short_url`: Specify `yes` if you want to leave out the full http URL. (only usable if you are using subfolders on the same domain for each language)

### Installation
Open copy the `LangSwitch` folder to your `site/addons` folder on your v2.x site and add the tags to your templates.

### NOTE: ###
Currently (2016-08-18 Statamic v2.1.2) there are some bugs with localisation of entries. It sort of works, but also fails if not 'all ticks are set'.

Test extensively and the use is for your own risk!

# servicenow-snippets package

ServiceNow snippets for Atom.

![screenshot](https://github.com/kaitoy/servicenow-snippets/raw/master/servicenow-snippets.gif)

## gs
* `gsi`: gs info

  ```javascript
  gs.info('${1:message}');$2
  ```

* `gsw`: gs warn

  ```javascript
  gs.warn('${1:message}');$2
  ```

* `gse`: gs error

  ```javascript
  gs.error('${1:message}');$2
  ```

* `gsgu`: gs getUser

  ```javascript
  var ${1:user} = gs.getUser();$2
  ```

* `gshr`: gs hasRole

  ```javascript
  gs.hasRole('${1:role}');$2
  ```

* `gsn`: gs nil

  ```javascript
  gs.nil(${1:object });$2
  ```

## GlideRecord
* `grn`: GlideRecord new

  ```javascript
  var ${1:gr} = new GlideRecord('${2:table}');$3
  ```

* `graaq`: GlideRecord addActiveQuery

  ```javascript
  ${1:gr}.addActiveQuery();$2
  ```

* `graq`: GlideRecord addQuery

  ```javascript
  ${1:gr}.addQuery('${2:name}', ${3:value});$4
  ```

* `grq`: GlideRecord query

  ```javascript
  ${1:gr}.query();$2
  ```

* `grg`: GlideRecord get

  ```javascript
  ${1:gr}.get('${2:sysId}');$3
  ```

* `grgrc`: GlideRecord getRowCount

  ```javascript
  ${1:gr}.getRowCount();$2
  ```

* `grgv`: GlideRecord getValue

  ```javascript
  ${1:gr}.getValue('${2:name}');$3
  ```

* `grsv`: GlideRecord setValue

  ```javascript
  ${1:gr}.setValue('${2:name}', ${3:value});$4
  ```

* `grn`: GlideRecord next

  ```javascript
  ${1:gr}.next();$2
  ```

* `grhn`: GlideRecord hasNext

  ```javascript
  ${1:gr}.hasNext();$2
  ```

* `gru`: GlideRecord update

  ```javascript
  ${1:gr}.update();$2
  ```

* `grnii`: GlideRecord new initialize insert

  ```javascript
  var ${1:gr} = new GlideRecord('${2:table}');
  ${1:gr}.initialize();
  ${1:gr}.insert();$3
  ```

* `grnni`: GlideRecord new newRecord insert

  ```javascript
  var ${1:gr} = new GlideRecord('${2:table}');
  ${1:gr}.newRecord();
  ${1:gr}.insert();$3
  ```

* `grql`: GlideRecord query loop

  ```javascript
  var ${1:gr} = new GlideRecord('${2:table}');
  ${1:gr}.addQuery('${3:name}', ${4:value});
  ${1:gr}.query();
  while (${1:gr}.next()) {
    $5
  }
  ```

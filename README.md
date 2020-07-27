# This is a fork of ember-find-related-files

*This is a modified version of ember-related-files for supporting indexed pods according to [component template colocation](https://github.com/emberjs/rfcs/blob/master/text/0481-component-templates-co-location.md#detailed-design). So far it backs a [modified version of the VSCode extension](https://github.com/NoneOfMaster/vscode-ember-related-files).*

Find related files in an EmberJS project directory.

## Usage

```Bash
npm install ember-find-related-files
```

```JavaScript
import findRelatedFiles from 'ember-find-related-files'

findRelatedFiles('/Users/josa/g/my-app', 'app/components/my-component.js')
// => [
//   { label: 'Template',  path: 'app/templates/components/my-component.hbs' },
//   { label: 'Unit test', path: 'tests/unit/components/my-component-test.js' }
// ]


findType('/Users/josa/g/my-app', 'component')
// => [
//   { label: 'my-component',  path: 'app/templates/components/my-component.hbs' }
// ]

```

## License

[The MIT License](LICENSE.md)

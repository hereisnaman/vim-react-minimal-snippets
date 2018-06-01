# Vim Minimal React Snippets

A Vim snippet library for React in ES6. You may also want to check out [vim-es2015-snippets](https://github.com/epilande/vim-es2015-snippets).

Requires [UltiSnips](https://github.com/SirVer/ultisnips).

## Installation

Using [Vundle]( https://github.com/VundleVim/Vundle.Vim):

```vim
" ES2015 code snippets (Optional)
Plugin 'epilande/vim-es2015-snippets'

" React code snippets
Plugin 'hereisnaman/vim-minimal-react-snippets'

" Ultisnips
Plugin 'SirVer/ultisnips'

" Trigger configuration (Optional)
" let g:UltiSnipsExpandTrigger="<tab>"

" Vundle install
:PluginInstall
```

## Usage
In a JavaScript or JSX file, type a trigger name while in Insert mode, then press Ultisnips trigger key. In my case I have it mapped to `<tab>`.

For example, let's say we have `ListItem.js`

In Insert mode

```javascript
rfc<tab>
```

Will expand to

```
import React from 'react';

const ListItem = (props) => <div />;

export default ListItem;
```

## Snippets

#### Skeleton

| Trigger  | Content |
| -------: | ------- |
| `rrcc→`  | React Redux Class Component |
| `rcc→`   | React Class Component |
| `rfc→`   | React Functional Component |

#### Lifecycle

| Trigger  | Content |
| -------: | ------- |
| `cwm→`   | `componentWillMount() {...}` |
| `cdm→`   | `componentDidMount() {...}` |
| `cwrp→`  | `componentWillReceiveProps(nextProps) {...}` |
| `scup→`  | `shouldComponentUpdate(nextProps, nextState) {...}` |
| `cwup→`  | `componentWillUpdate(nextProps, nextState) {...}` |
| `cdup→`  | `componentDidUpdate(prevProps, prevState) {...}` |
| `cwu→`   | `componentWillUnmount() {...}` |
| `ren→`   | `render() {...}` |

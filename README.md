# Intro to js

## Userful shorcuts
- `ctrl + l` to clear the terminal

## Useful commands
Go to the previous directory
```bash
cd ..
`````
Open a directory (you can autocomplete with TAB)
```bash
cd <directory>
`````

## Variable types

<!-- table with truthy values -->
| Truthy | Falsy | Type |
| ------ | ----- | ---- |
| 'a' | '' | string |
| 837 | 0 | number |
| 1.5 | 0.0  | float(number with decimals) |
| {} | | object |
| [] | | array |
| true | false | boolean |
| | null | null |
| | undefined | undefined |

## Convert string to number
```js
const number = parseInt('100');
```

## Convert string to float (number with decimals)
```js
const number = parseFloat('100.5');
```
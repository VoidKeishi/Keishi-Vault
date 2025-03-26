#javascript/standard 
- Là một chuẩn quy định cách cấu trúc một module và chia sẻ module cho [[JavaScript]]
- Import syntax: 
```JS
import component as name from './local.js'

import Subtract3 from './local.js'
import Subtract2 from './local.js'

import { PI, Subtract2 as Subtract2A } from './local.js'
```
- Export syntax
```JS
export const PI;
export function Subtract2;

export default Subtract;
```
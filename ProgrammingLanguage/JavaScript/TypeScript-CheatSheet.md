[![返回目录](https://parg.co/UCb)](https://github.com/wxyyxc1992/Awesome-CheatSheet)

# TypeScript 语法实践速览

参考了 [Let's Learn TypeScript](https://parg.co/Uik), [TypeScript Cheat Sheet](https://github.com/frontdevops/typescript-cheat-sheet)

```ts
import * as React from 'react';
import formatPrice from '../utils/formatPrice';

export interface IPriceProps {
  num: number;
  symbol: '$' | '€' | '£';
}

const Price: React.SFC<IPriceProps> = ({ num, symbol }: IPriceProps) => (
  <div>
    <h3>{formatPrice(num, symbol)}</h3>
  </div>
);
```

```ts
// 使用 const 能够有效减少编译之后的代码量，参考 https://parg.co/UxX
export const enum Colors {
  RED,
  BLUE,
  GREEN
}
```

# BetterObjectConstructor

![npm](https://img.shields.io/npm/dw/better-object-constructor?color=%23c9003d&style=flat-square&label=Downloads)
![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/aspulse/BetterObjectConstructor?color=%23c9003d&label=Pull%20Requests&style=flat-square)
![npm (tag)](https://img.shields.io/npm/v/better-object-constructor?style=flat-square)
![npm bundle size](https://img.shields.io/bundlephobia/min/better-object-constructor?style=flat-square)
![GitHub](https://img.shields.io/github/license/aspulse/BetterObjectConstructor?style=flat-square)  

<br>

## How to use?
```ts
import type { BetterObjectConstructor } from 'better-object-constructor';

declare const Object: BetterObjectConstructor;
```

<br>

## What will change?
For example: 
```ts
const hoge: { a: string } = {
  a: 'fugafuga'
};

const hoge2 = Object.fromEntries(Object.entries(hoge));
```
Placed in this code, hoge and hoge2 should truly have the same type.    
<br>
But let's look at it in the editor. (Below is a sample in VSCode…)

![image](https://user-images.githubusercontent.com/84216737/177096061-8f7baec1-178a-4669-9cda-e92967ed15ad.png)

Oh! We lost the type!  
But don't worry, if you add the code shown in the "How to use?" section...?

<br>

![image](https://user-images.githubusercontent.com/84216737/177096167-b92d0e72-e5f7-4b80-8bf2-8fe5d7528b50.png)

Welcome back, my lovely type definition.  
...That's the kind of package.


<br>

## Author
[Follow @\_AsPulse\_](https://twitter.com/_AsPulse_?ref_src=twsrc%5Etfw)

<br>

## License
BetterObjectConstructor is licensed under MIT.   
Please see [LICENSE](./LICENSE) for more info.

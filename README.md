## Marriott ![NPM version](https://img.shields.io/npm/v/marriott.svg?style=flat) 

a SDK of marriott hotels APIs.

### Installation
```bash
$ npm install marriott --save
```

### Example
```js
var marriott = require('marriott');

marriott.search({
  country: 'CN',
  province: 'CNHP',
  city: 'Sanya',
  arrivalDate: dataUtils.now(),
  departureDate: dataUtils.tomorrow()
}, function(err, hotels){
  if (err)
    return console.error(err)

  console.log(hotels);
});
```
Response JSON would like this:

```js
{ 
  id: '3482',
  thumbnail: '/pub/media/3482/str3482po.134187_md.jpg',
  name: '三亚亚龙湾瑞吉度假酒店',
  country: '中国,',
  state: '海南,',
  city: '三亚亚龙湾',
  address: '亚龙湾国家旅游度假区',
  fax: '(86)(898) 8855 5555',
  zipcode: '572016',
  category: '6',
  description: '酒店位于中国最顶级的度假村目的地海南岛，并占据得天独厚的优美海滨地点，是畅享休闲宁静的人间天堂。',
  bestRate: '4,200',
  redeemPoints: false,
  redeemCashPoints: false 
}
```

### API
Check this file: `lib/marriott.js`

### Tests
```bash
$ npm run test
```

### Contributing
- Fork this repo
- Clone your repo
- Install dependencies
- Checkout a feature branch
- Feel free to add your features
- Make sure your features are fully tested
- Open a pull request, and enjoy <3

### MIT license
Copyright (c) 2014 turing &lt;o.u.turing@gmail.com&gt;

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the &quot;Software&quot;), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED &quot;AS IS&quot;, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

---
![docor](https://raw.githubusercontent.com/turingou/docor/master/docor.png)
built upon love by [docor](https://github.com/turingou/docor.git) v0.2.0
# tushare-js
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fgavin-hao%2Ftushare-js.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fgavin-hao%2Ftushare-js?ref=badge_shield)

tushare.pro node.js sdk

# usage

- external dependency - danfojs-node
## install
```bash
yarn add tushare-js danfojs-node
```


```js
import TuShare from 'tushare-js';

const ts=TuShare('your token');
//stock daily api
const daily_datas=ts.daily({
  params: { ts_code: '002156',start_date: '20200808',end_date: '20220809'},
  fields: ['ts_code', 'trade_date', 'open', 'high', 'low'],
})
// common api query
const dt=ts.query({
  api_name:'daily'
  params: { ts_code: '002156',start_date: '20200808',end_date: '20220809'},
  fields: ['ts_code', 'trade_date', 'open', 'high', 'low'],
})

```

## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fgavin-hao%2Ftushare-js.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fgavin-hao%2Ftushare-js?ref=badge_large)
Angular helper to get current country by TimeZone


## Versions

| Angular version | package version |
| --------------- | --------------- |
| 14.x|14.x|

## Installation

```shell
npm install --save @solidexpert/ngx-country-helper
```


## Usage

Add `ClickOutsideModule` to your list of module imports:

```typescript
import * as helper from "@solidexpert/ngx-country-helper";
```

You can then use the directive in your templates:

```typescript
@Component({
  selector: 'app',
  template: `
    <div>{{data.country}} -- {{data.code}}</div>
  `
})
export class AppComponent {
  
  data:{}
  constructor() {
   this.data = helper.getCountry();
  }
}
```
# React GMaps
> Wrapper component for [gmaps](https://hpneo.github.io/gmaps/)

## Usage

### Install
``` bash
yarn add @anarklab/react-gmaps # or npm install @anarklab/react-gmaps --save
```

Add the reference to google api
``` html
<script src="//maps.google.com/maps/api/js?key=<your api key>"></script>
```

### Usage

``` js
import React from 'react'
import GMaps from 'react-gmaps'

export default () => (
  <GMaps addr="Hell's Kitchen, New York, NY, USA" marker />
)
```

The basic usage is passing `addr` props:
``` js
<GMaps addr="Hell's Kitchen, New York, NY, USA" />
```

Also, you can add `marker` as boolean attribute or an string to custom image
``` js
<GMaps addr="Hell's Kitchen, New York, NY, USA" marker />
// or
<GMaps addr="Hell's Kitchen, New York, NY, USA" marker="path/to/your/custom/pin.png" />
```

You can change the default options:
``` js
<GMaps addr="Hell's Kitchen, New York, NY, USA" options={...} />
```

To see more detailed information, please see the [Google Documentation](https://developers.google.com/maps/documentation/javascript/)


## Demo
You can see this component working [here](https://anarklab.github.io/react-gmaps)

## License
The MIT License (MIT). Please see [License File](LICENSE) for more information.

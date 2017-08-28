# skeleton-card-vuejs
A reusable skeleton card component written in Vuejs

![alt text](https://github.com/FrancescoSaverioZuppichini/skeleton-card-vuejs/blob/master/docs/images/1.png?raw=true)

### Usage
The package can be installed using npm

```
npm install -S skeleton-card-vuejs
```

Then you just need to import it has a normal vuejs component

```
import SkeletonCard from 'skeleton-card-vuejs'
```

It provides a customisable skeleton card **to be display as feedback while loading** a content

It needs Veufify in order to work, you can find more about it:

https://vuetifyjs.com/quick-start

If you want to know more, you can read the medium article about it:

### API
The compononent can be customise in shape passins the following props:

#### hasHeader: Boolean
If `true` the header with the avatar is displayed
#### hasMedia: Boolean
If `true` the media is displayed
#### hasText: Boolean
If `true` the thext is displayed
#### hasActions: Boolean
If `true` the actions are displayed after the content
#### lines: Int
The number of text linest to be showed
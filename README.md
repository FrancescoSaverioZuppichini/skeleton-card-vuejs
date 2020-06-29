# skeleton-card-vuejs
A reusable skeleton card component written in Vuejs

![alt text](https://github.com/FrancescoSaverioZuppichini/skeleton-card-vuejs/blob/master/docs/images/1.png?raw=true)

### Motivation
Loader spinner are boring. A skeleton card gives to the user a clue of what the content will look like.

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

It needs Vuetify in order to work, you can find more about it:

https://vuetifyjs.com/quick-start

If you want to know more, you can read the medium article about it:

https://medium.com/js-dojo/async-in-vue-js-part-1-28d96f751a2e

### API
The compononent's shape can be customise using the following props:

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

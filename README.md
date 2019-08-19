# \<composited-card\>

A simple, framework agnostic [web component](https://developer.mozilla.org/en-US/docs/Web/Web_Components) to facilitate the display of [Gods Unchained](https://godsunchained.com/) card element(s).

## Component inputs

### @property({ type: Number }) protoId

A Cards id/proto number. Either a protoId or inputProtoData must be provided for a card to render.

### @property({ type: Object }) inputProtoData

All the information needed to render a card. When this complete input is provided, the composited-card component will skip the card-data endpoint call.
This input should contain the following fields:

```
type: string;
effect: string;
name: string;
rarity: string;
god: string;
mana: number;
id: number;
attack: number;
health: number;
```

### @property({ type: Number }) quality

OPTIONAL: a card's quality setting. When this input is missing, the a default quality setting of 0 will be used for all artwork/layers.

### @property({ type: String }) responsiveImageSizes

OPTIONAL: a sizes string to indicate to the browser, roughly how big images will be once they are rendered into the layout. If this input is missing, the cards will automatically use the lowest resolution assets available. To read more about this syntax and how it's used, [go here](https://css-tricks.com/sometimes-sizes-is-quite-important/).

## Install dependencies

```
$ yarn install
```

## Viewing demo elements

```
$ yarn demo
```

## Building for prod

```
$ yarn build
```

# remark42.quartz

Quartz plugin for Remark42 comments.

## Installing
`quartz-plugin`: `quartz plugin add OCDkirby/remark42.quartz`

manual: add `remark42.ts` to your `<repo dir>/quartz/plugins/transformers` and add this to your `quartz.plugins.ts`:


```ts
const plugins: PluginStore = {
  available: [
    ...,
    {
      url: "OCDkirby/remark42",
      enabled: true,
      cfg: Plugin.Remark42({ host: "https://comments.my-host.com"... }),
    },
    ...
  ]
}
```

## Usage
Configure in `quartz.plugins.ts` according to the [Remark42 docs](https://remark42.com/docs/configuration/frontend/) and place an empty `div` somewhere in a component or markdown with the property `id="remark42"`.

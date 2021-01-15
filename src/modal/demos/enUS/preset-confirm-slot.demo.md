# Use Preset Dialog (Slot)

Slots are also related to preset.

```html
<n-button @click="modalActive = true"> Start Me up </n-button>
<n-modal v-model:show="modalActive" preset="confirm" title="Dialog">
  <template #header>
    <div>title</div>
  </template>
  <template #content>
    <div>content</div>
  </template>
  <template #action>
    <div>action</div>
  </template>
</n-modal>
```

```js
export default {
  data () {
    return {
      modalActive: false
    }
  }
}
```
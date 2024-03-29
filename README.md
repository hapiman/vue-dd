ace-editor-on-vue
====================

![](https://img.shields.io/badge/vue-%3E2.0-brightgreen.svg)
![](https://img.shields.io/npm/v/ace-editor-on-vue.svg)
![](https://img.shields.io/npm/dt/ace-editor-on-vue.svg)
![](https://img.shields.io/github/license/NoName4Me/ace-editor-on-vue.svg)

A vuejs based component, based on bace, on Ace.

## Usage

* install

```shell
npm install vue-dd
```

* `.vue` demo

```html
<template>
    <!-- support `%`, `px` and other CSS `width`/`height` units -->
    <editor v-model="content" :config="config" width="500px" height="200px"></editor>
</template>

<script>
import AceEditorOnVue from 'ace-editor-on-vue';
export default {
    components: {
        'ace-editor': AceEditorOnVue
    },
    data() {
        return {
            content: '',
            config: {
                lang: 'json', // default `json`
                theme: 'xcode', // default `xcode`
                options: { // options for Ace
                    useSoftTabs: true, // default 2 space characters for indent
                    tabSize: 2
                }
            }
        }
    }
}
</script>
```

> More details see [Ace Editor Wiki](https://github.com/ajaxorg/ace/wiki).

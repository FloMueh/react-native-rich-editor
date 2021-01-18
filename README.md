# react-native-pell-rich-editor with custom font face functionality

All Credits by [wxik](https://github.com/wxik/react-native-rich-editor).

## how to add custom font face from web source

```javascript
const iOSCustomFontFace = `@font-face {
        font-family: 'SFPro';
        src: url('https://your-web-server.com/assets/fonts/SFPro/sf-pro-text-regular.ttf?raw=true'),
            url('https://your-web-server.com/assets/fonts/SFPro/sf-pro-text-regular.ttf?raw=true');
    }
    @font-face {
        font-family: 'SFProSemi';
        src: url('https://your-web-server.com/assets/fonts/SFPro/sf-pro-text-semibold.ttf?raw=true'),
            url('https://your-web-server.com/assets/fonts/SFPro/sf-pro-text-semibold.ttf?raw=true');
    }`;

<RichEditor
    editorStyle={{
        initialCSSText: iOSCustomFontFace,
        customFontFamily: 'SFPro',
    }}
/>;
```

## how to add custom local font

The Richeditor does not support to add your local font files. But there is a workaround for that.

You can convert your font file to base 64 css style. Just go to https://transfonter.org/.

**Important** enable Base 64 Encode.

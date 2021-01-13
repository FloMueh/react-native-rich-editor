# react-native-pell-rich-editor with custom font face functionality

All Credits by [wxik](https://github.com/wxik/react-native-rich-editor).

## how to add custom font face

**Important**: Currently you can just use fonts which are stored on a webserver.

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

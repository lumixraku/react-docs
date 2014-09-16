---
id: tags-and-attributes
title: 标签和属性（Attributes）
permalink: tags-and-attributes.html
prev: component-specs.html
next: events.html
---

## 支持的标签

React 希望支持所有通用的标签. 如果你需要一个这里没有列出的标签, 请提交一个 Issue.

### HTML 标签

支持下列 HTML 标签：

```
a abbr address area article aside audio b base bdi bdo big blockquote body br
button canvas caption cite code col colgroup data datalist dd del details dfn
dialog div dl dt em embed fieldset figcaption figure footer form h1 h2 h3 h4 h5
h6 head header hr html i iframe img input ins kbd keygen label legend li link
main map mark menu menuitem meta meter nav noscript object ol optgroup option
output p param pre progress q rp rt ruby s samp script section select small
source span strong style sub summary sup table tbody td textarea tfoot th
thead time title tr track u ul var video wbr
```

### SVG 标签

支持下列 SVG 标签:

```
circle defs ellipse g line linearGradient mask path pattern polygon polyline
radialGradient rect stop svg text tspan
```

你也许会对 [react-art](https://github.com/facebook/react-art) 感兴趣, 这是个 React 的绘图类库, 可以渲染 Canvas,
SVG, or VML (用于 IE8).


## 支持的属性

React 支持所有 `data-*` 和 `aria-*` 属性后面罗列的每个属性.

> 注意:
>
> 所有属性使用驼峰命名, 其中 `class` 和 ` for` 属性应该是 `className` 和 `htmlFor`, 分别对应 DOM API 规范.

关于事件, 见[事件支持](/react/docs/events.html).

### HTML 属性

支持这些标准属性:

```
accept accessKey action allowFullScreen allowTransparency alt async
autoComplete autoFocus autoPlay cellPadding cellSpacing charSet checked
className cols colSpan content contentEditable contextMenu controls coords
crossOrigin data dateTime defer dir disabled download draggable encType form
formNoValidate frameBorder height hidden href hrefLang htmlFor httpEquiv icon
id label lang list loop max maxLength mediaGroup method min multiple muted
name noValidate open pattern placeholder poster preload radioGroup readOnly rel
required role rows rowSpan sandbox scope scrollLeft scrolling scrollTop
seamless selected shape size span spellCheck src srcDoc srcSet start step
style tabIndex target title type useMap value width wmode
```

另外, 支持后面这些非标准的属性:

- `autoCapitalize autoCorrect` 针对 Mobile Safari.
- `property` 针对 [Open Graph](http://ogp.me/) meta 标签.
- `itemProp itemScope itemType` 针对 [HTML5 microdata](http://schema.org/docs/gs.html).

还有一个 React 专用的属性 `dangerouslySetInnerHTML` ([更多](/react/docs/special-non-dom-attributes.html)),
用于在组件当中直接插入 HTML.

### SVG 属性

```
cx cy d dx dy fill fillOpacity fontFamily fontSize fx fy gradientTransform
gradientUnits markerEnd markerMid markerStart offset opacity
patternContentUnits patternUnits points preserveAspectRatio r rx ry
spreadMethod stopColor stopOpacity stroke strokeDasharray strokeLinecap
strokeOpacity strokeWidth textAnchor transform version viewBox x1 x2 x y1 y2 y
```

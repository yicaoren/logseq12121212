---
title: css
---

## custom.ss主题语法
### tags
#### *以下「data-ref=%%」中，将%%修改为任意文字，该文字变为tag之后及会被后面的颜色定义*
#### ==================================================
TAGS
- Styles all tags
- Adds colors to some specific tags
==================================================
*/

a.tag[data-ref] {
    align-items: center;
    background: var(--ls-color-clouds);
    border-radius: 1rem 0.4rem 0.4rem 1rem;
    color: var(--ls-primary-background-color);
    display: inline-flex;
    font-size: 0.8rem;
    font-weight: 400;
    letter-spacing: 0.05em;
    line-height: 0.8rem;
    padding: 0.2rem 0.3rem;
    text-transform: uppercase;
    transition: .3s;
    white-space: nowrap;
}

a.tag[data-ref]:hover {
    filter: grayscale(25%) !important;
}

a.tag[data-ref]:before {
    background-color: var(--ls-primary-background-color);
    border-radius: 50%;
    content: '';
    display: inline-block;
    height: 0.6rem;
    line-height: 0.8rem;
    margin-right: 0.3rem;
    width: 0.6rem;
}

a.tag[data-ref="Permanent"] {
    background-color: var(--ls-color-nephritis) !important;
}

a.tag[data-ref="Literature"] {
    background-color: var(--ls-color-amethyst) !important;
}

a.tag[data-ref="Fleeting"] {
    background-color: var(--pink) !important;
}

a.tag[data-ref="Miscellaneous"] {
    background-color: var(--ls-color-peter-river) !important;
}

a.tag[data-ref="Journal"] {
    background-color: var(--ls-color-turquoise) !important;
}

a.tag[data-ref="Task"] {
    background-color: var(--ls-color-orange) !important;
}

a.tag[data-ref="Project"] {
    background-color: var(--ls-color-carrot) !important;
}

a.tag[data-ref="Event"] {
    background-color: var(--ls-color-pumpkin) !important;
}

a.tag[data-ref="WIP"] {
    background-color: var(--ls-color-sunflower) !important;
}

/*
### COLORFUL INDENTATION
#### *大纲左侧竖线颜色定义*
#### ==================================================
COLORFUL INDENTATION
==================================================
*/

.block-children {
    border-left: 0;
}

.block-children [level] {
    border-left-width: 1px;
    border-left-style: solid;
}

.block-children [level="3"] {
    border-left-color: var(--pink-level-3);
}

.block-children [level="4"] {
    border-left-color: var(--pink-level-4);
}

.block-children [level="5"] {
    border-left-color: var(--pink-level-5);
}

.block-children [level="6"] {
    border-left-color: var(--pink-level-6);
}

.block-children [level="7"] {
    border-left-color: var(--pink-level-7);
}

.block-children [level="8"] {
    border-left-color: var(--pink-level-8);
}

.block-children [level="9"] {
    border-left-color: var(--pink-level-9);
}

/*

---
layout: post
title:  "AI Tech Adoption Model"
date:   2025-01-12 12:54:00 +0000
categories: blog
---

# Jupyter notebook for AI Tech Adoption

This is merely a quick rip of my working notebook to an html to get it documented on the site - 

<html lang="en">
<head><meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>agentpy_ai_tech_adoption</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
<style type="text/css">
    pre { line-height: 125%; }
td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
.highlight .hll { background-color: var(--jp-cell-editor-active-background) }
.highlight { background: var(--jp-cell-editor-background); color: var(--jp-mirror-editor-variable-color) }
.highlight .c { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment */
.highlight .err { color: var(--jp-mirror-editor-error-color) } /* Error */
.highlight .k { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword */
.highlight .o { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /* Operator */
.highlight .p { color: var(--jp-mirror-editor-punctuation-color) } /* Punctuation */
.highlight .ch { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Multiline */
.highlight .cp { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Preproc */
.highlight .cpf { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Single */
.highlight .cs { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Special */
.highlight .kc { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Pseudo */
.highlight .kr { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Type */
.highlight .m { color: var(--jp-mirror-editor-number-color) } /* Literal.Number */
.highlight .s { color: var(--jp-mirror-editor-string-color) } /* Literal.String */
.highlight .ow { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /* Operator.Word */
.highlight .pm { color: var(--jp-mirror-editor-punctuation-color) } /* Punctuation.Marker */
.highlight .w { color: var(--jp-mirror-editor-variable-color) } /* Text.Whitespace */
.highlight .mb { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Bin */
.highlight .mf { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Float */
.highlight .mh { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Hex */
.highlight .mi { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Integer */
.highlight .mo { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Oct */
.highlight .sa { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Affix */
.highlight .sb { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Backtick */
.highlight .sc { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Char */
.highlight .dl { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Delimiter */
.highlight .sd { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Doc */
.highlight .s2 { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Double */
.highlight .se { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Escape */
.highlight .sh { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Heredoc */
.highlight .si { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Interpol */
.highlight .sx { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Other */
.highlight .sr { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Regex */
.highlight .s1 { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Single */
.highlight .ss { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Symbol */
.highlight .il { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Integer.Long */
  </style>
<style type="text/css">
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*
 * Mozilla scrollbar styling
 */

/* use standard opaque scrollbars for most nodes */
[data-jp-theme-scrollbars='true'] {
  scrollbar-color: rgb(var(--jp-scrollbar-thumb-color))
    var(--jp-scrollbar-background-color);
}

/* for code nodes, use a transparent style of scrollbar. These selectors
 * will match lower in the tree, and so will override the above */
[data-jp-theme-scrollbars='true'] .CodeMirror-hscrollbar,
[data-jp-theme-scrollbars='true'] .CodeMirror-vscrollbar {
  scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
}

/* tiny scrollbar */

.jp-scrollbar-tiny {
  scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
  scrollbar-width: thin;
}

/* tiny scrollbar */

.jp-scrollbar-tiny::-webkit-scrollbar,
.jp-scrollbar-tiny::-webkit-scrollbar-corner {
  background-color: transparent;
  height: 4px;
  width: 4px;
}

.jp-scrollbar-tiny::-webkit-scrollbar-thumb {
  background: rgba(var(--jp-scrollbar-thumb-color), 0.5);
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:horizontal {
  border-left: 0 solid transparent;
  border-right: 0 solid transparent;
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:vertical {
  border-top: 0 solid transparent;
  border-bottom: 0 solid transparent;
}

/*
 * Lumino
 */

.lm-ScrollBar[data-orientation='horizontal'] {
  min-height: 16px;
  max-height: 16px;
  min-width: 45px;
  border-top: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] {
  min-width: 16px;
  max-width: 16px;
  min-height: 45px;
  border-left: 1px solid #a0a0a0;
}

.lm-ScrollBar-button {
  background-color: #f0f0f0;
  background-position: center center;
  min-height: 15px;
  max-height: 15px;
  min-width: 15px;
  max-width: 15px;
}

.lm-ScrollBar-button:hover {
  background-color: #dadada;
}

.lm-ScrollBar-button.lm-mod-active {
  background-color: #cdcdcd;
}

.lm-ScrollBar-track {
  background: #f0f0f0;
}

.lm-ScrollBar-thumb {
  background: #cdcdcd;
}

.lm-ScrollBar-thumb:hover {
  background: #bababa;
}

.lm-ScrollBar-thumb.lm-mod-active {
  background: #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal'] .lm-ScrollBar-thumb {
  height: 100%;
  min-width: 15px;
  border-left: 1px solid #a0a0a0;
  border-right: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] .lm-ScrollBar-thumb {
  width: 100%;
  min-height: 15px;
  border-top: 1px solid #a0a0a0;
  border-bottom: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal']
  .lm-ScrollBar-button[data-action='decrement'] {
  background-image: var(--jp-icon-caret-left);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='horizontal']
  .lm-ScrollBar-button[data-action='increment'] {
  background-image: var(--jp-icon-caret-right);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
  .lm-ScrollBar-button[data-action='decrement'] {
  background-image: var(--jp-icon-caret-up);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
  .lm-ScrollBar-button[data-action='increment'] {
  background-image: var(--jp-icon-caret-down);
  background-size: 17px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-Widget {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
}

.lm-Widget.lm-mod-hidden {
  display: none !important;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.lm-AccordionPanel[data-orientation='horizontal'] > .lm-AccordionPanel-title {
  /* Title is rotated for horizontal accordion panel using CSS */
  display: block;
  transform-origin: top left;
  transform: rotate(-90deg) translate(-100%);
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-CommandPalette {
  display: flex;
  flex-direction: column;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-CommandPalette-search {
  flex: 0 0 auto;
}

.lm-CommandPalette-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  min-height: 0;
  overflow: auto;
  list-style-type: none;
}

.lm-CommandPalette-header {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.lm-CommandPalette-item {
  display: flex;
  flex-direction: row;
}

.lm-CommandPalette-itemIcon {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemContent {
  flex: 1 1 auto;
  overflow: hidden;
}

.lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemLabel {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.lm-close-icon {
  border: 1px solid transparent;
  background-color: transparent;
  position: absolute;
  z-index: 1;
  right: 3%;
  top: 0;
  bottom: 0;
  margin: auto;
  padding: 7px 0;
  display: none;
  vertical-align: middle;
  outline: 0;
  cursor: pointer;
}
.lm-close-icon:after {
  content: 'X';
  display: block;
  width: 15px;
  height: 15px;
  text-align: center;
  color: #000;
  font-weight: normal;
  font-size: 12px;
  cursor: pointer;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-DockPanel {
  z-index: 0;
}

.lm-DockPanel-widget {
  z-index: 0;
}

.lm-DockPanel-tabBar {
  z-index: 1;
}

.lm-DockPanel-handle {
  z-index: 2;
}

.lm-DockPanel-handle.lm-mod-hidden {
  display: none !important;
}

.lm-DockPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}

.lm-DockPanel-handle[data-orientation='horizontal'] {
  cursor: ew-resize;
}

.lm-DockPanel-handle[data-orientation='vertical'] {
  cursor: ns-resize;
}

.lm-DockPanel-handle[data-orientation='horizontal']:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}

.lm-DockPanel-handle[data-orientation='vertical']:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

.lm-DockPanel-overlay {
  z-index: 3;
  box-sizing: border-box;
  pointer-events: none;
}

.lm-DockPanel-overlay.lm-mod-hidden {
  display: none !important;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-Menu {
  z-index: 10000;
  position: absolute;
  white-space: nowrap;
  overflow-x: hidden;
  overflow-y: auto;
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-Menu-content {
  margin: 0;
  padding: 0;
  display: table;
  list-style-type: none;
}

.lm-Menu-item {
  display: table-row;
}

.lm-Menu-item.lm-mod-hidden,
.lm-Menu-item.lm-mod-collapsed {
  display: none !important;
}

.lm-Menu-itemIcon,
.lm-Menu-itemSubmenuIcon {
  display: table-cell;
  text-align: center;
}

.lm-Menu-itemLabel {
  display: table-cell;
  text-align: left;
}

.lm-Menu-itemShortcut {
  display: table-cell;
  text-align: right;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-MenuBar {
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-MenuBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: row;
  list-style-type: none;
}

.lm-MenuBar-item {
  box-sizing: border-box;
}

.lm-MenuBar-itemIcon,
.lm-MenuBar-itemLabel {
  display: inline-block;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-ScrollBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-ScrollBar[data-orientation='horizontal'] {
  flex-direction: row;
}

.lm-ScrollBar[data-orientation='vertical'] {
  flex-direction: column;
}

.lm-ScrollBar-button {
  box-sizing: border-box;
  flex: 0 0 auto;
}

.lm-ScrollBar-track {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  flex: 1 1 auto;
}

.lm-ScrollBar-thumb {
  box-sizing: border-box;
  position: absolute;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-SplitPanel-child {
  z-index: 0;
}

.lm-SplitPanel-handle {
  z-index: 1;
}

.lm-SplitPanel-handle.lm-mod-hidden {
  display: none !important;
}

.lm-SplitPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}

.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle {
  cursor: ew-resize;
}

.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle {
  cursor: ns-resize;
}

.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}

.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-TabBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-TabBar[data-orientation='horizontal'] {
  flex-direction: row;
  align-items: flex-end;
}

.lm-TabBar[data-orientation='vertical'] {
  flex-direction: column;
  align-items: flex-end;
}

.lm-TabBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex: 1 1 auto;
  list-style-type: none;
}

.lm-TabBar[data-orientation='horizontal'] > .lm-TabBar-content {
  flex-direction: row;
}

.lm-TabBar[data-orientation='vertical'] > .lm-TabBar-content {
  flex-direction: column;
}

.lm-TabBar-tab {
  display: flex;
  flex-direction: row;
  box-sizing: border-box;
  overflow: hidden;
  touch-action: none; /* Disable native Drag/Drop */
}

.lm-TabBar-tabIcon,
.lm-TabBar-tabCloseIcon {
  flex: 0 0 auto;
}

.lm-TabBar-tabLabel {
  flex: 1 1 auto;
  overflow: hidden;
  white-space: nowrap;
}

.lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing: border-box;
}

.lm-TabBar-tab.lm-mod-hidden {
  display: none !important;
}

.lm-TabBar-addButton.lm-mod-hidden {
  display: none !important;
}

.lm-TabBar.lm-mod-dragging .lm-TabBar-tab {
  position: relative;
}

.lm-TabBar.lm-mod-dragging[data-orientation='horizontal'] .lm-TabBar-tab {
  left: 0;
  transition: left 150ms ease;
}

.lm-TabBar.lm-mod-dragging[data-orientation='vertical'] .lm-TabBar-tab {
  top: 0;
  transition: top 150ms ease;
}

.lm-TabBar.lm-mod-dragging .lm-TabBar-tab.lm-mod-dragging {
  transition: none;
}

.lm-TabBar-tabLabel .lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing: border-box;
  background: inherit;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-TabPanel-tabBar {
  z-index: 1;
}

.lm-TabPanel-stackedPanel {
  z-index: 0;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapse {
  display: flex;
  flex-direction: column;
  align-items: stretch;
}

.jp-Collapse-header {
  padding: 1px 12px;
  background-color: var(--jp-layout-color1);
  border-bottom: solid var(--jp-border-width) var(--jp-border-color2);
  color: var(--jp-ui-font-color1);
  cursor: pointer;
  display: flex;
  align-items: center;
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  text-transform: uppercase;
  user-select: none;
}

.jp-Collapser-icon {
  height: 16px;
}

.jp-Collapse-header-collapsed .jp-Collapser-icon {
  transform: rotate(-90deg);
  margin: auto 0;
}

.jp-Collapser-title {
  line-height: 25px;
}

.jp-Collapse-contents {
  padding: 0 12px;
  background-color: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensureUiComponents() in @jupyterlab/buildutils */

/**
 * (DEPRECATED) Support for consuming icons as CSS background images
 */

/* Icons urls */

:root {
  --jp-icon-add-above: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPGcgY2xpcC1wYXRoPSJ1cmwoI2NsaXAwXzEzN18xOTQ5MikiPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGQ9Ik00Ljc1IDQuOTMwNjZINi42MjVWNi44MDU2NkM2LjYyNSA3LjAxMTkxIDYuNzkzNzUgNy4xODA2NiA3IDcuMTgwNjZDNy4yMDYyNSA3LjE4MDY2IDcuMzc1IDcuMDExOTEgNy4zNzUgNi44MDU2NlY0LjkzMDY2SDkuMjVDOS40NTYyNSA0LjkzMDY2IDkuNjI1IDQuNzYxOTEgOS42MjUgNC41NTU2NkM5LjYyNSA0LjM0OTQxIDkuNDU2MjUgNC4xODA2NiA5LjI1IDQuMTgwNjZINy4zNzVWMi4zMDU2NkM3LjM3NSAyLjA5OTQxIDcuMjA2MjUgMS45MzA2NiA3IDEuOTMwNjZDNi43OTM3NSAxLjkzMDY2IDYuNjI1IDIuMDk5NDEgNi42MjUgMi4zMDU2NlY0LjE4MDY2SDQuNzVDNC41NDM3NSA0LjE4MDY2IDQuMzc1IDQuMzQ5NDEgNC4zNzUgNC41NTU2NkM0LjM3NSA0Ljc2MTkxIDQuNTQzNzUgNC45MzA2NiA0Ljc1IDQuOTMwNjZaIiBmaWxsPSIjNjE2MTYxIiBzdHJva2U9IiM2MTYxNjEiIHN0cm9rZS13aWR0aD0iMC43Ii8+CjwvZz4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTExLjUgOS41VjExLjVMMi41IDExLjVWOS41TDExLjUgOS41Wk0xMiA4QzEyLjU1MjMgOCAxMyA4LjQ0NzcyIDEzIDlWMTJDMTMgMTIuNTUyMyAxMi41NTIzIDEzIDEyIDEzTDIgMTNDMS40NDc3MiAxMyAxIDEyLjU1MjMgMSAxMlY5QzEgOC40NDc3MiAxLjQ0NzcxIDggMiA4TDEyIDhaIiBmaWxsPSIjNjE2MTYxIi8+CjxkZWZzPgo8Y2xpcFBhdGggaWQ9ImNsaXAwXzEzN18xOTQ5MiI+CjxyZWN0IGNsYXNzPSJqcC1pY29uMyIgd2lkdGg9IjYiIGhlaWdodD0iNiIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0ibWF0cml4KC0xIDAgMCAxIDEwIDEuNTU1NjYpIi8+CjwvY2xpcFBhdGg+CjwvZGVmcz4KPC9zdmc+Cg==);
  --jp-icon-add-below: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPGcgY2xpcC1wYXRoPSJ1cmwoI2NsaXAwXzEzN18xOTQ5OCkiPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGQ9Ik05LjI1IDEwLjA2OTNMNy4zNzUgMTAuMDY5M0w3LjM3NSA4LjE5NDM0QzcuMzc1IDcuOTg4MDkgNy4yMDYyNSA3LjgxOTM0IDcgNy44MTkzNEM2Ljc5Mzc1IDcuODE5MzQgNi42MjUgNy45ODgwOSA2LjYyNSA4LjE5NDM0TDYuNjI1IDEwLjA2OTNMNC43NSAxMC4wNjkzQzQuNTQzNzUgMTAuMDY5MyA0LjM3NSAxMC4yMzgxIDQuMzc1IDEwLjQ0NDNDNC4zNzUgMTAuNjUwNiA0LjU0Mzc1IDEwLjgxOTMgNC43NSAxMC44MTkzTDYuNjI1IDEwLjgxOTNMNi42MjUgMTIuNjk0M0M2LjYyNSAxMi45MDA2IDYuNzkzNzUgMTMuMDY5MyA3IDEzLjA2OTNDNy4yMDYyNSAxMy4wNjkzIDcuMzc1IDEyLjkwMDYgNy4zNzUgMTIuNjk0M0w3LjM3NSAxMC44MTkzTDkuMjUgMTAuODE5M0M5LjQ1NjI1IDEwLjgxOTMgOS42MjUgMTAuNjUwNiA5LjYyNSAxMC40NDQzQzkuNjI1IDEwLjIzODEgOS40NTYyNSAxMC4wNjkzIDkuMjUgMTAuMDY5M1oiIGZpbGw9IiM2MTYxNjEiIHN0cm9rZT0iIzYxNjE2MSIgc3Ryb2tlLXdpZHRoPSIwLjciLz4KPC9nPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMi41IDUuNUwyLjUgMy41TDExLjUgMy41TDExLjUgNS41TDIuNSA1LjVaTTIgN0MxLjQ0NzcyIDcgMSA2LjU1MjI4IDEgNkwxIDNDMSAyLjQ0NzcyIDEuNDQ3NzIgMiAyIDJMMTIgMkMxMi41NTIzIDIgMTMgMi40NDc3MiAxMyAzTDEzIDZDMTMgNi41NTIyOSAxMi41NTIzIDcgMTIgN0wyIDdaIiBmaWxsPSIjNjE2MTYxIi8+CjxkZWZzPgo8Y2xpcFBhdGggaWQ9ImNsaXAwXzEzN18xOTQ5OCI+CjxyZWN0IGNsYXNzPSJqcC1pY29uMyIgd2lkdGg9IjYiIGhlaWdodD0iNiIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0ibWF0cml4KDEgMS43NDg0NmUtMDcgMS43NDg0NmUtMDcgLTEgNCAxMy40NDQzKSIvPgo8L2NsaXBQYXRoPgo8L2RlZnM+Cjwvc3ZnPgo=);
  --jp-icon-add: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDEzaC02djZoLTJ2LTZINXYtMmg2VjVoMnY2aDZ2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-bell: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE2IDE2IiB2ZXJzaW9uPSIxLjEiPgogICA8cGF0aCBjbGFzcz0ianAtaWNvbjIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMzMzMzMzIgogICAgICBkPSJtOCAwLjI5Yy0xLjQgMC0yLjcgMC43My0zLjYgMS44LTEuMiAxLjUtMS40IDMuNC0xLjUgNS4yLTAuMTggMi4yLTAuNDQgNC0yLjMgNS4zbDAuMjggMS4zaDVjMC4wMjYgMC42NiAwLjMyIDEuMSAwLjcxIDEuNSAwLjg0IDAuNjEgMiAwLjYxIDIuOCAwIDAuNTItMC40IDAuNi0xIDAuNzEtMS41aDVsMC4yOC0xLjNjLTEuOS0wLjk3LTIuMi0zLjMtMi4zLTUuMy0wLjEzLTEuOC0wLjI2LTMuNy0xLjUtNS4yLTAuODUtMS0yLjItMS44LTMuNi0xLjh6bTAgMS40YzAuODggMCAxLjkgMC41NSAyLjUgMS4zIDAuODggMS4xIDEuMSAyLjcgMS4yIDQuNCAwLjEzIDEuNyAwLjIzIDMuNiAxLjMgNS4yaC0xMGMxLjEtMS42IDEuMi0zLjQgMS4zLTUuMiAwLjEzLTEuNyAwLjMtMy4zIDEuMi00LjQgMC41OS0wLjcyIDEuNi0xLjMgMi41LTEuM3ptLTAuNzQgMTJoMS41Yy0wLjAwMTUgMC4yOCAwLjAxNSAwLjc5LTAuNzQgMC43OS0wLjczIDAuMDAxNi0wLjcyLTAuNTMtMC43NC0wLjc5eiIgLz4KPC9zdmc+Cg==);
  --jp-icon-bug-dot: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiPgogICAgICAgIDxwYXRoIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMTcuMTkgOEgyMFYxMEgxNy45MUMxNy45NiAxMC4zMyAxOCAxMC42NiAxOCAxMVYxMkgyMFYxNEgxOC41SDE4VjE0LjAyNzVDMTUuNzUgMTQuMjc2MiAxNCAxNi4xODM3IDE0IDE4LjVDMTQgMTkuMjA4IDE0LjE2MzUgMTkuODc3OSAxNC40NTQ5IDIwLjQ3MzlDMTMuNzA2MyAyMC44MTE3IDEyLjg3NTcgMjEgMTIgMjFDOS43OCAyMSA3Ljg1IDE5Ljc5IDYuODEgMThINFYxNkg2LjA5QzYuMDQgMTUuNjcgNiAxNS4zNCA2IDE1VjE0SDRWMTJINlYxMUM2IDEwLjY2IDYuMDQgMTAuMzMgNi4wOSAxMEg0VjhINi44MUM3LjI2IDcuMjIgNy44OCA2LjU1IDguNjIgNi4wNEw3IDQuNDFMOC40MSAzTDEwLjU5IDUuMTdDMTEuMDQgNS4wNiAxMS41MSA1IDEyIDVDMTIuNDkgNSAxMi45NiA1LjA2IDEzLjQyIDUuMTdMMTUuNTkgM0wxNyA0LjQxTDE1LjM3IDYuMDRDMTYuMTIgNi41NSAxNi43NCA3LjIyIDE3LjE5IDhaTTEwIDE2SDE0VjE0SDEwVjE2Wk0xMCAxMkgxNFYxMEgxMFYxMloiIGZpbGw9IiM2MTYxNjEiLz4KICAgICAgICA8cGF0aCBkPSJNMjIgMTguNUMyMiAyMC40MzMgMjAuNDMzIDIyIDE4LjUgMjJDMTYuNTY3IDIyIDE1IDIwLjQzMyAxNSAxOC41QzE1IDE2LjU2NyAxNi41NjcgMTUgMTguNSAxNUMyMC40MzMgMTUgMjIgMTYuNTY3IDIyIDE4LjVaIiBmaWxsPSIjNjE2MTYxIi8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-bug: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0yMCA4aC0yLjgxYy0uNDUtLjc4LTEuMDctMS40NS0xLjgyLTEuOTZMMTcgNC40MSAxNS41OSAzbC0yLjE3IDIuMTdDMTIuOTYgNS4wNiAxMi40OSA1IDEyIDVjLS40OSAwLS45Ni4wNi0xLjQxLjE3TDguNDEgMyA3IDQuNDFsMS42MiAxLjYzQzcuODggNi41NSA3LjI2IDcuMjIgNi44MSA4SDR2MmgyLjA5Yy0uMDUuMzMtLjA5LjY2LS4wOSAxdjFINHYyaDJ2MWMwIC4zNC4wNC42Ny4wOSAxSDR2MmgyLjgxYzEuMDQgMS43OSAyLjk3IDMgNS4xOSAzczQuMTUtMS4yMSA1LjE5LTNIMjB2LTJoLTIuMDljLjA1LS4zMy4wOS0uNjYuMDktMXYtMWgydi0yaC0ydi0xYzAtLjM0LS4wNC0uNjctLjA5LTFIMjBWOHptLTYgOGgtNHYtMmg0djJ6bTAtNGgtNHYtMmg0djJ6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-build: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE0LjkgMTcuNDVDMTYuMjUgMTcuNDUgMTcuMzUgMTYuMzUgMTcuMzUgMTVDMTcuMzUgMTMuNjUgMTYuMjUgMTIuNTUgMTQuOSAxMi41NUMxMy41NCAxMi41NSAxMi40NSAxMy42NSAxMi40NSAxNUMxMi40NSAxNi4zNSAxMy41NCAxNy40NSAxNC45IDE3LjQ1Wk0yMC4xIDE1LjY4TDIxLjU4IDE2Ljg0QzIxLjcxIDE2Ljk1IDIxLjc1IDE3LjEzIDIxLjY2IDE3LjI5TDIwLjI2IDE5LjcxQzIwLjE3IDE5Ljg2IDIwIDE5LjkyIDE5LjgzIDE5Ljg2TDE4LjA5IDE5LjE2QzE3LjczIDE5LjQ0IDE3LjMzIDE5LjY3IDE2LjkxIDE5Ljg1TDE2LjY0IDIxLjdDMTYuNjIgMjEuODcgMTYuNDcgMjIgMTYuMyAyMkgxMy41QzEzLjMyIDIyIDEzLjE4IDIxLjg3IDEzLjE1IDIxLjdMMTIuODkgMTkuODVDMTIuNDYgMTkuNjcgMTIuMDcgMTkuNDQgMTEuNzEgMTkuMTZMOS45NjAwMiAxOS44NkM5LjgxMDAyIDE5LjkyIDkuNjIwMDIgMTkuODYgOS41NDAwMiAxOS43MUw4LjE0MDAyIDE3LjI5QzguMDUwMDIgMTcuMTMgOC4wOTAwMiAxNi45NSA4LjIyMDAyIDE2Ljg0TDkuNzAwMDIgMTUuNjhMOS42NTAwMSAxNUw5LjcwMDAyIDE0LjMxTDguMjIwMDIgMTMuMTZDOC4wOTAwMiAxMy4wNSA4LjA1MDAyIDEyLjg2IDguMTQwMDIgMTIuNzFMOS41NDAwMiAxMC4yOUM5LjYyMDAyIDEwLjEzIDkuODEwMDIgMTAuMDcgOS45NjAwMiAxMC4xM0wxMS43MSAxMC44NEMxMi4wNyAxMC41NiAxMi40NiAxMC4zMiAxMi44OSAxMC4xNUwxMy4xNSA4LjI4OTk4QzEzLjE4IDguMTI5OTggMTMuMzIgNy45OTk5OCAxMy41IDcuOTk5OThIMTYuM0MxNi40NyA3Ljk5OTk4IDE2LjYyIDguMTI5OTggMTYuNjQgOC4yODk5OEwxNi45MSAxMC4xNUMxNy4zMyAxMC4zMiAxNy43MyAxMC41NiAxOC4wOSAxMC44NEwxOS44MyAxMC4xM0MyMCAxMC4wNyAyMC4xNyAxMC4xMyAyMC4yNiAxMC4yOUwyMS42NiAxMi43MUMyMS43NSAxMi44NiAyMS43MSAxMy4wNSAyMS41OCAxMy4xNkwyMC4xIDE0LjMxTDIwLjE1IDE1TDIwLjEgMTUuNjhaIi8+CiAgICA8cGF0aCBkPSJNNy4zMjk2NiA3LjQ0NDU0QzguMDgzMSA3LjAwOTU0IDguMzM5MzIgNi4wNTMzMiA3LjkwNDMyIDUuMjk5ODhDNy40NjkzMiA0LjU0NjQzIDYuNTA4MSA0LjI4MTU2IDUuNzU0NjYgNC43MTY1NkM1LjM5MTc2IDQuOTI2MDggNS4xMjY5NSA1LjI3MTE4IDUuMDE4NDkgNS42NzU5NEM0LjkxMDA0IDYuMDgwNzEgNC45NjY4MiA2LjUxMTk4IDUuMTc2MzQgNi44NzQ4OEM1LjYxMTM0IDcuNjI4MzIgNi41NzYyMiA3Ljg3OTU0IDcuMzI5NjYgNy40NDQ1NFpNOS42NTcxOCA0Ljc5NTkzTDEwLjg2NzIgNC45NTE3OUMxMC45NjI4IDQuOTc3NDEgMTEuMDQwMiA1LjA3MTMzIDExLjAzODIgNS4xODc5M0wxMS4wMzg4IDYuOTg4OTNDMTEuMDQ1NSA3LjEwMDU0IDEwLjk2MTYgNy4xOTUxOCAxMC44NTUgNy4yMTA1NEw5LjY2MDAxIDcuMzgwODNMOS4yMzkxNSA4LjEzMTg4TDkuNjY5NjEgOS4yNTc0NUM5LjcwNzI5IDkuMzYyNzEgOS42NjkzNCA5LjQ3Njk5IDkuNTc0MDggOS41MzE5OUw4LjAxNTIzIDEwLjQzMkM3LjkxMTMxIDEwLjQ5MiA3Ljc5MzM3IDEwLjQ2NzcgNy43MjEwNSAxMC4zODI0TDYuOTg3NDggOS40MzE4OEw2LjEwOTMxIDkuNDMwODNMNS4zNDcwNCAxMC4zOTA1QzUuMjg5MDkgMTAuNDcwMiA1LjE3MzgzIDEwLjQ5MDUgNS4wNzE4NyAxMC40MzM5TDMuNTEyNDUgOS41MzI5M0MzLjQxMDQ5IDkuNDc2MzMgMy4zNzY0NyA5LjM1NzQxIDMuNDEwNzUgOS4yNTY3OUwzLjg2MzQ3IDguMTQwOTNMMy42MTc0OSA3Ljc3NDg4TDMuNDIzNDcgNy4zNzg4M0wyLjIzMDc1IDcuMjEyOTdDMi4xMjY0NyA3LjE5MjM1IDIuMDQwNDkgNy4xMDM0MiAyLjA0MjQ1IDYuOTg2ODJMMi4wNDE4NyA1LjE4NTgyQzIuMDQzODMgNS4wNjkyMiAyLjExOTA5IDQuOTc5NTggMi4yMTcwNCA0Ljk2OTIyTDMuNDIwNjUgNC43OTM5M0wzLjg2NzQ5IDQuMDI3ODhMMy40MTEwNSAyLjkxNzMxQzMuMzczMzcgMi44MTIwNCAzLjQxMTMxIDIuNjk3NzYgMy41MTUyMyAyLjYzNzc2TDUuMDc0MDggMS43Mzc3NkM1LjE2OTM0IDEuNjgyNzYgNS4yODcyOSAxLjcwNzA0IDUuMzU5NjEgMS43OTIzMUw2LjExOTE1IDIuNzI3ODhMNi45ODAwMSAyLjczODkzTDcuNzI0OTYgMS43ODkyMkM3Ljc5MTU2IDEuNzA0NTggNy45MTU0OCAxLjY3OTIyIDguMDA4NzkgMS43NDA4Mkw5LjU2ODIxIDIuNjQxODJDOS42NzAxNyAyLjY5ODQyIDkuNzEyODUgMi44MTIzNCA5LjY4NzIzIDIuOTA3OTdMOS4yMTcxOCA0LjAzMzgzTDkuNDYzMTYgNC4zOTk4OEw5LjY1NzE4IDQuNzk1OTNaIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iOS45LDEzLjYgMy42LDcuNCA0LjQsNi42IDkuOSwxMi4yIDE1LjQsNi43IDE2LjEsNy40ICIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNS45TDksOS43bDMuOC0zLjhsMS4yLDEuMmwtNC45LDVsLTQuOS01TDUuMiw1Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNy41TDksMTEuMmwzLjgtMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-left: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik0xMC44LDEyLjhMNy4xLDlsMy44LTMuOGwwLDcuNkgxMC44eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-right: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik03LjIsNS4yTDEwLjksOWwtMy44LDMuOFY1LjJINy4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-up-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iMTUuNCwxMy4zIDkuOSw3LjcgNC40LDEzLjIgMy42LDEyLjUgOS45LDYuMyAxNi4xLDEyLjYgIi8+Cgk8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-up: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik01LjIsMTAuNUw5LDYuOGwzLjgsMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-case-sensitive: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgogIDxnIGNsYXNzPSJqcC1pY29uLWFjY2VudDIiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTcuNiw4aDAuOWwzLjUsOGgtMS4xTDEwLDE0SDZsLTAuOSwySDRMNy42LDh6IE04LDkuMUw2LjQsMTNoMy4yTDgsOS4xeiIvPgogICAgPHBhdGggZD0iTTE2LjYsOS44Yy0wLjIsMC4xLTAuNCwwLjEtMC43LDAuMWMtMC4yLDAtMC40LTAuMS0wLjYtMC4yYy0wLjEtMC4xLTAuMi0wLjQtMC4yLTAuNyBjLTAuMywwLjMtMC42LDAuNS0wLjksMC43Yy0wLjMsMC4xLTAuNywwLjItMS4xLDAuMmMtMC4zLDAtMC41LDAtMC43LTAuMWMtMC4yLTAuMS0wLjQtMC4yLTAuNi0wLjNjLTAuMi0wLjEtMC4zLTAuMy0wLjQtMC41IGMtMC4xLTAuMi0wLjEtMC40LTAuMS0wLjdjMC0wLjMsMC4xLTAuNiwwLjItMC44YzAuMS0wLjIsMC4zLTAuNCwwLjQtMC41QzEyLDcsMTIuMiw2LjksMTIuNSw2LjhjMC4yLTAuMSwwLjUtMC4xLDAuNy0wLjIgYzAuMy0wLjEsMC41LTAuMSwwLjctMC4xYzAuMiwwLDAuNC0wLjEsMC42LTAuMWMwLjIsMCwwLjMtMC4xLDAuNC0wLjJjMC4xLTAuMSwwLjItMC4yLDAuMi0wLjRjMC0xLTEuMS0xLTEuMy0xIGMtMC40LDAtMS40LDAtMS40LDEuMmgtMC45YzAtMC40LDAuMS0wLjcsMC4yLTFjMC4xLTAuMiwwLjMtMC40LDAuNS0wLjZjMC4yLTAuMiwwLjUtMC4zLDAuOC0wLjNDMTMuMyw0LDEzLjYsNCwxMy45LDQgYzAuMywwLDAuNSwwLDAuOCwwLjFjMC4zLDAsMC41LDAuMSwwLjcsMC4yYzAuMiwwLjEsMC40LDAuMywwLjUsMC41QzE2LDUsMTYsNS4yLDE2LDUuNnYyLjljMCwwLjIsMCwwLjQsMCwwLjUgYzAsMC4xLDAuMSwwLjIsMC4zLDAuMmMwLjEsMCwwLjIsMCwwLjMsMFY5Ljh6IE0xNS4yLDYuOWMtMS4yLDAuNi0zLjEsMC4yLTMuMSwxLjRjMCwxLjQsMy4xLDEsMy4xLTAuNVY2Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-check: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik05IDE2LjE3TDQuODMgMTJsLTEuNDIgMS40MUw5IDE5IDIxIDdsLTEuNDEtMS40MXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-circle-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDJDNi40NyAyIDIgNi40NyAyIDEyczQuNDcgMTAgMTAgMTAgMTAtNC40NyAxMC0xMFMxNy41MyAyIDEyIDJ6bTAgMThjLTQuNDEgMC04LTMuNTktOC04czMuNTktOCA4LTggOCAzLjU5IDggOC0zLjU5IDgtOCA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-circle: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iOSIgY3k9IjkiIHI9IjgiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-clear: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8bWFzayBpZD0iZG9udXRIb2xlIj4KICAgIDxyZWN0IHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgZmlsbD0id2hpdGUiIC8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSI4IiBmaWxsPSJibGFjayIvPgogIDwvbWFzaz4KCiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxyZWN0IGhlaWdodD0iMTgiIHdpZHRoPSIyIiB4PSIxMSIgeT0iMyIgdHJhbnNmb3JtPSJyb3RhdGUoMzE1LCAxMiwgMTIpIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIxMCIgbWFzaz0idXJsKCNkb251dEhvbGUpIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-close: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1ub25lIGpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIGpwLWljb24zLWhvdmVyIiBmaWxsPSJub25lIj4KICAgIDxjaXJjbGUgY3g9IjEyIiBjeT0iMTIiIHI9IjExIi8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIGpwLWljb24tYWNjZW50Mi1ob3ZlciIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMTkgNi40MUwxNy41OSA1IDEyIDEwLjU5IDYuNDEgNSA1IDYuNDEgMTAuNTkgMTIgNSAxNy41OSA2LjQxIDE5IDEyIDEzLjQxIDE3LjU5IDE5IDE5IDE3LjU5IDEzLjQxIDEyeiIvPgogIDwvZz4KCiAgPGcgY2xhc3M9ImpwLWljb24tbm9uZSBqcC1pY29uLWJ1c3kiIGZpbGw9Im5vbmUiPgogICAgPGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-code-check: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBzaGFwZS1yZW5kZXJpbmc9Imdlb21ldHJpY1ByZWNpc2lvbiI+CiAgICA8cGF0aCBkPSJNNi41OSwzLjQxTDIsOEw2LjU5LDEyLjZMOCwxMS4xOEw0LjgyLDhMOCw0LjgyTDYuNTksMy40MU0xMi40MSwzLjQxTDExLDQuODJMMTQuMTgsOEwxMSwxMS4xOEwxMi40MSwxMi42TDE3LDhMMTIuNDEsMy40MU0yMS41OSwxMS41OUwxMy41LDE5LjY4TDkuODMsMTZMOC40MiwxNy40MUwxMy41LDIyLjVMMjMsMTNMMjEuNTksMTEuNTlaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-code: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTExLjQgMTguNkw2LjggMTRMMTEuNCA5LjRMMTAgOEw0IDE0TDEwIDIwTDExLjQgMTguNlpNMTYuNiAxOC42TDIxLjIgMTRMMTYuNiA5LjRMMTggOEwyNCAxNEwxOCAyMEwxNi42IDE4LjZWMTguNloiLz4KCTwvZz4KPC9zdmc+Cg==);
  --jp-icon-collapse-all: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTggMmMxIDAgMTEgMCAxMiAwczIgMSAyIDJjMCAxIDAgMTEgMCAxMnMwIDItMiAyQzIwIDE0IDIwIDQgMjAgNFMxMCA0IDYgNGMwLTIgMS0yIDItMnoiIC8+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTE4IDhjMC0xLTEtMi0yLTJTNSA2IDQgNnMtMiAxLTIgMmMwIDEgMCAxMSAwIDEyczEgMiAyIDJjMSAwIDExIDAgMTIgMHMyLTEgMi0yYzAtMSAwLTExIDAtMTJ6bS0yIDB2MTJINFY4eiIgLz4KICAgICAgICA8cGF0aCBkPSJNNiAxM3YyaDh2LTJ6IiAvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-console: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwMCAyMDAiPgogIDxnIGNsYXNzPSJqcC1jb25zb2xlLWljb24tYmFja2dyb3VuZC1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMjg4RDEiPgogICAgPHBhdGggZD0iTTIwIDE5LjhoMTYwdjE1OS45SDIweiIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtY29uc29sZS1pY29uLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIj4KICAgIDxwYXRoIGQ9Ik0xMDUgMTI3LjNoNDB2MTIuOGgtNDB6TTUxLjEgNzdMNzQgOTkuOWwtMjMuMyAyMy4zIDEwLjUgMTAuNSAyMy4zLTIzLjNMOTUgOTkuOSA4NC41IDg5LjQgNjEuNiA2Ni41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-copy: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTExLjksMUgzLjJDMi40LDEsMS43LDEuNywxLjcsMi41djEwLjJoMS41VjIuNWg4LjdWMXogTTE0LjEsMy45aC04Yy0wLjgsMC0xLjUsMC43LTEuNSwxLjV2MTAuMmMwLDAuOCwwLjcsMS41LDEuNSwxLjVoOCBjMC44LDAsMS41LTAuNywxLjUtMS41VjUuNEMxNS41LDQuNiwxNC45LDMuOSwxNC4xLDMuOXogTTE0LjEsMTUuNWgtOFY1LjRoOFYxNS41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-copyright: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGVuYWJsZS1iYWNrZ3JvdW5kPSJuZXcgMCAwIDI0IDI0IiBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCI+CiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0xMS44OCw5LjE0YzEuMjgsMC4wNiwxLjYxLDEuMTUsMS42MywxLjY2aDEuNzljLTAuMDgtMS45OC0xLjQ5LTMuMTktMy40NS0zLjE5QzkuNjQsNy42MSw4LDksOCwxMi4xNCBjMCwxLjk0LDAuOTMsNC4yNCwzLjg0LDQuMjRjMi4yMiwwLDMuNDEtMS42NSwzLjQ0LTIuOTVoLTEuNzljLTAuMDMsMC41OS0wLjQ1LDEuMzgtMS42MywxLjQ0QzEwLjU1LDE0LjgzLDEwLDEzLjgxLDEwLDEyLjE0IEMxMCw5LjI1LDExLjI4LDkuMTYsMTEuODgsOS4xNHogTTEyLDJDNi40OCwyLDIsNi40OCwyLDEyczQuNDgsMTAsMTAsMTBzMTAtNC40OCwxMC0xMFMxNy41MiwyLDEyLDJ6IE0xMiwyMGMtNC40MSwwLTgtMy41OS04LTggczMuNTktOCw4LThzOCwzLjU5LDgsOFMxNi40MSwyMCwxMiwyMHoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-cut: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkuNjQgNy42NGMuMjMtLjUuMzYtMS4wNS4zNi0xLjY0IDAtMi4yMS0xLjc5LTQtNC00UzIgMy43OSAyIDZzMS43OSA0IDQgNGMuNTkgMCAxLjE0LS4xMyAxLjY0LS4zNkwxMCAxMmwtMi4zNiAyLjM2QzcuMTQgMTQuMTMgNi41OSAxNCA2IDE0Yy0yLjIxIDAtNCAxLjc5LTQgNHMxLjc5IDQgNCA0IDQtMS43OSA0LTRjMC0uNTktLjEzLTEuMTQtLjM2LTEuNjRMMTIgMTRsNyA3aDN2LTFMOS42NCA3LjY0ek02IDhjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTAgMTJjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTYtNy41Yy0uMjggMC0uNS0uMjItLjUtLjVzLjIyLS41LjUtLjUuNS4yMi41LjUtLjIyLjUtLjUuNXpNMTkgM2wtNiA2IDIgMiA3LTdWM3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-delete: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2cHgiIGhlaWdodD0iMTZweCI+CiAgICA8cGF0aCBkPSJNMCAwaDI0djI0SDB6IiBmaWxsPSJub25lIiAvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjI2MjYyIiBkPSJNNiAxOWMwIDEuMS45IDIgMiAyaDhjMS4xIDAgMi0uOSAyLTJWN0g2djEyek0xOSA0aC0zLjVsLTEtMWgtNWwtMSAxSDV2MmgxNFY0eiIgLz4KPC9zdmc+Cg==);
  --jp-icon-download: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDloLTRWM0g5djZINWw3IDcgNy03ek01IDE4djJoMTR2LTJINXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-duplicate: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTIuNzk5OTggMC44NzVIOC44OTU4MkM5LjIwMDYxIDAuODc1IDkuNDQ5OTggMS4xMzkxNCA5LjQ0OTk4IDEuNDYxOThDOS40NDk5OCAxLjc4NDgyIDkuMjAwNjEgMi4wNDg5NiA4Ljg5NTgyIDIuMDQ4OTZIMy4zNTQxNUMzLjA0OTM2IDIuMDQ4OTYgMi43OTk5OCAyLjMxMzEgMi43OTk5OCAyLjYzNTk0VjkuNjc5NjlDMi43OTk5OCAxMC4wMDI1IDIuNTUwNjEgMTAuMjY2NyAyLjI0NTgyIDEwLjI2NjdDMS45NDEwMyAxMC4yNjY3IDEuNjkxNjUgMTAuMDAyNSAxLjY5MTY1IDkuNjc5NjlWMi4wNDg5NkMxLjY5MTY1IDEuNDAzMjggMi4xOTA0IDAuODc1IDIuNzk5OTggMC44NzVaTTUuMzY2NjUgMTEuOVY0LjU1SDExLjA4MzNWMTEuOUg1LjM2NjY1Wk00LjE0MTY1IDQuMTQxNjdDNC4xNDE2NSAzLjY5MDYzIDQuNTA3MjggMy4zMjUgNC45NTgzMiAzLjMyNUgxMS40OTE3QzExLjk0MjcgMy4zMjUgMTIuMzA4MyAzLjY5MDYzIDEyLjMwODMgNC4xNDE2N1YxMi4zMDgzQzEyLjMwODMgMTIuNzU5NCAxMS45NDI3IDEzLjEyNSAxMS40OTE3IDEzLjEyNUg0Ljk1ODMyQzQuNTA3MjggMTMuMTI1IDQuMTQxNjUgMTIuNzU5NCA0LjE0MTY1IDEyLjMwODNWNC4xNDE2N1oiIGZpbGw9IiM2MTYxNjEiLz4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNOS40MzU3NCA4LjI2NTA3SDguMzY0MzFWOS4zMzY1QzguMzY0MzEgOS40NTQzNSA4LjI2Nzg4IDkuNTUwNzggOC4xNTAwMiA5LjU1MDc4QzguMDMyMTcgOS41NTA3OCA3LjkzNTc0IDkuNDU0MzUgNy45MzU3NCA5LjMzNjVWOC4yNjUwN0g2Ljg2NDMxQzYuNzQ2NDUgOC4yNjUwNyA2LjY1MDAyIDguMTY4NjQgNi42NTAwMiA4LjA1MDc4QzYuNjUwMDIgNy45MzI5MiA2Ljc0NjQ1IDcuODM2NSA2Ljg2NDMxIDcuODM2NUg3LjkzNTc0VjYuNzY1MDdDNy45MzU3NCA2LjY0NzIxIDguMDMyMTcgNi41NTA3OCA4LjE1MDAyIDYuNTUwNzhDOC4yNjc4OCA2LjU1MDc4IDguMzY0MzEgNi42NDcyMSA4LjM2NDMxIDYuNzY1MDdWNy44MzY1SDkuNDM1NzRDOS41NTM2IDcuODM2NSA5LjY1MDAyIDcuOTMyOTIgOS42NTAwMiA4LjA1MDc4QzkuNjUwMDIgOC4xNjg2NCA5LjU1MzYgOC4yNjUwNyA5LjQzNTc0IDguMjY1MDdaIiBmaWxsPSIjNjE2MTYxIiBzdHJva2U9IiM2MTYxNjEiIHN0cm9rZS13aWR0aD0iMC41Ii8+Cjwvc3ZnPgo=);
  --jp-icon-edit: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMgMTcuMjVWMjFoMy43NUwxNy44MSA5Ljk0bC0zLjc1LTMuNzVMMyAxNy4yNXpNMjAuNzEgNy4wNGMuMzktLjM5LjM5LTEuMDIgMC0xLjQxbC0yLjM0LTIuMzRjLS4zOS0uMzktMS4wMi0uMzktMS40MSAwbC0xLjgzIDEuODMgMy43NSAzLjc1IDEuODMtMS44M3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-ellipses: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iNSIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxOSIgY3k9IjEyIiByPSIyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-error: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj48Y2lyY2xlIGN4PSIxMiIgY3k9IjE5IiByPSIyIi8+PHBhdGggZD0iTTEwIDNoNHYxMmgtNHoiLz48L2c+CjxwYXRoIGZpbGw9Im5vbmUiIGQ9Ik0wIDBoMjR2MjRIMHoiLz4KPC9zdmc+Cg==);
  --jp-icon-expand-all: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTggMmMxIDAgMTEgMCAxMiAwczIgMSAyIDJjMCAxIDAgMTEgMCAxMnMwIDItMiAyQzIwIDE0IDIwIDQgMjAgNFMxMCA0IDYgNGMwLTIgMS0yIDItMnoiIC8+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTE4IDhjMC0xLTEtMi0yLTJTNSA2IDQgNnMtMiAxLTIgMmMwIDEgMCAxMSAwIDEyczEgMiAyIDJjMSAwIDExIDAgMTIgMHMyLTEgMi0yYzAtMSAwLTExIDAtMTJ6bS0yIDB2MTJINFY4eiIgLz4KICAgICAgICA8cGF0aCBkPSJNMTEgMTBIOXYzSDZ2MmgzdjNoMnYtM2gzdi0yaC0zeiIgLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-extension: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwLjUgMTFIMTlWN2MwLTEuMS0uOS0yLTItMmgtNFYzLjVDMTMgMi4xMiAxMS44OCAxIDEwLjUgMVM4IDIuMTIgOCAzLjVWNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAydjMuOEgzLjVjMS40OSAwIDIuNyAxLjIxIDIuNyAyLjdzLTEuMjEgMi43LTIuNyAyLjdIMlYyMGMwIDEuMS45IDIgMiAyaDMuOHYtMS41YzAtMS40OSAxLjIxLTIuNyAyLjctMi43IDEuNDkgMCAyLjcgMS4yMSAyLjcgMi43VjIySDE3YzEuMSAwIDItLjkgMi0ydi00aDEuNWMxLjM4IDAgMi41LTEuMTIgMi41LTIuNVMyMS44OCAxMSAyMC41IDExeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-fast-forward: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTQgMThsOC41LTZMNCA2djEyem05LTEydjEybDguNS02TDEzIDZ6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-file-upload: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkgMTZoNnYtNmg0bC03LTctNyA3aDR6bS00IDJoMTR2Mkg1eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-file: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuMyA4LjJsLTUuNS01LjVjLS4zLS4zLS43LS41LTEuMi0uNUgzLjljLS44LjEtMS42LjktMS42IDEuOHYxNC4xYzAgLjkuNyAxLjYgMS42IDEuNmgxNC4yYy45IDAgMS42LS43IDEuNi0xLjZWOS40Yy4xLS41LS4xLS45LS40LTEuMnptLTUuOC0zLjNsMy40IDMuNmgtMy40VjQuOXptMy45IDEyLjdINC43Yy0uMSAwLS4yIDAtLjItLjJWNC43YzAtLjIuMS0uMy4yLS4zaDcuMnY0LjRzMCAuOC4zIDEuMWMuMy4zIDEuMS4zIDEuMS4zaDQuM3Y3LjJzLS4xLjItLjIuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-filter-dot: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTE0LDEyVjE5Ljg4QzE0LjA0LDIwLjE4IDEzLjk0LDIwLjUgMTMuNzEsMjAuNzFDMTMuMzIsMjEuMSAxMi42OSwyMS4xIDEyLjMsMjAuNzFMMTAuMjksMTguN0MxMC4wNiwxOC40NyA5Ljk2LDE4LjE2IDEwLDE3Ljg3VjEySDkuOTdMNC4yMSw0LjYyQzMuODcsNC4xOSAzLjk1LDMuNTYgNC4zOCwzLjIyQzQuNTcsMy4wOCA0Ljc4LDMgNSwzVjNIMTlWM0MxOS4yMiwzIDE5LjQzLDMuMDggMTkuNjIsMy4yMkMyMC4wNSwzLjU2IDIwLjEzLDQuMTkgMTkuNzksNC42MkwxNC4wMywxMkgxNFoiIC8+CiAgPC9nPgogIDxnIGNsYXNzPSJqcC1pY29uLWRvdCIgZmlsbD0iI0ZGRiI+CiAgICA8Y2lyY2xlIGN4PSIxOCIgY3k9IjE3IiByPSIzIj48L2NpcmNsZT4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-filter-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEwIDE4aDR2LTJoLTR2MnpNMyA2djJoMThWNkgzem0zIDdoMTJ2LTJINnYyeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-filter: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTE0LDEyVjE5Ljg4QzE0LjA0LDIwLjE4IDEzLjk0LDIwLjUgMTMuNzEsMjAuNzFDMTMuMzIsMjEuMSAxMi42OSwyMS4xIDEyLjMsMjAuNzFMMTAuMjksMTguN0MxMC4wNiwxOC40NyA5Ljk2LDE4LjE2IDEwLDE3Ljg3VjEySDkuOTdMNC4yMSw0LjYyQzMuODcsNC4xOSAzLjk1LDMuNTYgNC4zOCwzLjIyQzQuNTcsMy4wOCA0Ljc4LDMgNSwzVjNIMTlWM0MxOS4yMiwzIDE5LjQzLDMuMDggMTkuNjIsMy4yMkMyMC4wNSwzLjU2IDIwLjEzLDQuMTkgMTkuNzksNC42MkwxNC4wMywxMkgxNFoiIC8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-folder-favorite: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjRweCIgdmlld0JveD0iMCAwIDI0IDI0IiB3aWR0aD0iMjRweCIgZmlsbD0iIzAwMDAwMCI+CiAgPHBhdGggZD0iTTAgMGgyNHYyNEgwVjB6IiBmaWxsPSJub25lIi8+PHBhdGggY2xhc3M9ImpwLWljb24zIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzYxNjE2MSIgZD0iTTIwIDZoLThsLTItMkg0Yy0xLjEgMC0yIC45LTIgMnYxMmMwIDEuMS45IDIgMiAyaDE2YzEuMSAwIDItLjkgMi0yVjhjMC0xLjEtLjktMi0yLTJ6bS0yLjA2IDExTDE1IDE1LjI4IDEyLjA2IDE3bC43OC0zLjMzLTIuNTktMi4yNCAzLjQxLS4yOUwxNSA4bDEuMzQgMy4xNCAzLjQxLjI5LTIuNTkgMi4yNC43OCAzLjMzeiIvPgo8L3N2Zz4K);
  --jp-icon-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY4YzAtMS4xLS45LTItMi0yaC04bC0yLTJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-home: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjRweCIgdmlld0JveD0iMCAwIDI0IDI0IiB3aWR0aD0iMjRweCIgZmlsbD0iIzAwMDAwMCI+CiAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPjxwYXRoIGNsYXNzPSJqcC1pY29uMyBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xMCAyMHYtNmg0djZoNXYtOGgzTDEyIDMgMiAxMmgzdjh6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-html5: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMDAiIGQ9Ik0xMDguNCAwaDIzdjIyLjhoMjEuMlYwaDIzdjY5aC0yM1Y0NmgtMjF2MjNoLTIzLjJNMjA2IDIzaC0yMC4zVjBoNjMuN3YyM0gyMjl2NDZoLTIzbTUzLjUtNjloMjQuMWwxNC44IDI0LjNMMzEzLjIgMGgyNC4xdjY5aC0yM1YzNC44bC0xNi4xIDI0LjgtMTYuMS0yNC44VjY5aC0yMi42bTg5LjItNjloMjN2NDYuMmgzMi42VjY5aC01NS42Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2U0NGQyNiIgZD0iTTEwNy42IDQ3MWwtMzMtMzcwLjRoMzYyLjhsLTMzIDM3MC4yTDI1NS43IDUxMiIvPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNmMTY1MjkiIGQ9Ik0yNTYgNDgwLjVWMTMxaDE0OC4zTDM3NiA0NDciLz4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNlYmViZWIiIGQ9Ik0xNDIgMTc2LjNoMTE0djQ1LjRoLTY0LjJsNC4yIDQ2LjVoNjB2NDUuM0gxNTQuNG0yIDIyLjhIMjAybDMuMiAzNi4zIDUwLjggMTMuNnY0Ny40bC05My4yLTI2Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIiBkPSJNMzY5LjYgMTc2LjNIMjU1Ljh2NDUuNGgxMDkuNm0tNC4xIDQ2LjVIMjU1Ljh2NDUuNGg1NmwtNS4zIDU5LTUwLjcgMTMuNnY0Ny4ybDkzLTI1LjgiLz4KPC9zdmc+Cg==);
  --jp-icon-image: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1icmFuZDQganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNGRkYiIGQ9Ik0yLjIgMi4yaDE3LjV2MTcuNUgyLjJ6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzNGNTFCNSIgZD0iTTIuMiAyLjJ2MTcuNWgxNy41bC4xLTE3LjVIMi4yem0xMi4xIDIuMmMxLjIgMCAyLjIgMSAyLjIgMi4ycy0xIDIuMi0yLjIgMi4yLTIuMi0xLTIuMi0yLjIgMS0yLjIgMi4yLTIuMnpNNC40IDE3LjZsMy4zLTguOCAzLjMgNi42IDIuMi0zLjIgNC40IDUuNEg0LjR6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-info: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUwLjk3OCA1MC45NzgiPgoJPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KCQk8cGF0aCBkPSJNNDMuNTIsNy40NThDMzguNzExLDIuNjQ4LDMyLjMwNywwLDI1LjQ4OSwwQzE4LjY3LDAsMTIuMjY2LDIuNjQ4LDcuNDU4LDcuNDU4CgkJCWMtOS45NDMsOS45NDEtOS45NDMsMjYuMTE5LDAsMzYuMDYyYzQuODA5LDQuODA5LDExLjIxMiw3LjQ1NiwxOC4wMzEsNy40NThjMCwwLDAuMDAxLDAsMC4wMDIsMAoJCQljNi44MTYsMCwxMy4yMjEtMi42NDgsMTguMDI5LTcuNDU4YzQuODA5LTQuODA5LDcuNDU3LTExLjIxMiw3LjQ1Ny0xOC4wM0M1MC45NzcsMTguNjcsNDguMzI4LDEyLjI2Niw0My41Miw3LjQ1OHoKCQkJIE00Mi4xMDYsNDIuMTA1Yy00LjQzMiw0LjQzMS0xMC4zMzIsNi44NzItMTYuNjE1LDYuODcyaC0wLjAwMmMtNi4yODUtMC4wMDEtMTIuMTg3LTIuNDQxLTE2LjYxNy02Ljg3MgoJCQljLTkuMTYyLTkuMTYzLTkuMTYyLTI0LjA3MSwwLTMzLjIzM0MxMy4zMDMsNC40NCwxOS4yMDQsMiwyNS40ODksMmM2LjI4NCwwLDEyLjE4NiwyLjQ0LDE2LjYxNyw2Ljg3MgoJCQljNC40MzEsNC40MzEsNi44NzEsMTAuMzMyLDYuODcxLDE2LjYxN0M0OC45NzcsMzEuNzcyLDQ2LjUzNiwzNy42NzUsNDIuMTA2LDQyLjEwNXoiLz4KCQk8cGF0aCBkPSJNMjMuNTc4LDMyLjIxOGMtMC4wMjMtMS43MzQsMC4xNDMtMy4wNTksMC40OTYtMy45NzJjMC4zNTMtMC45MTMsMS4xMS0xLjk5NywyLjI3Mi0zLjI1MwoJCQljMC40NjgtMC41MzYsMC45MjMtMS4wNjIsMS4zNjctMS41NzVjMC42MjYtMC43NTMsMS4xMDQtMS40NzgsMS40MzYtMi4xNzVjMC4zMzEtMC43MDcsMC40OTUtMS41NDEsMC40OTUtMi41CgkJCWMwLTEuMDk2LTAuMjYtMi4wODgtMC43NzktMi45NzljLTAuNTY1LTAuODc5LTEuNTAxLTEuMzM2LTIuODA2LTEuMzY5Yy0xLjgwMiwwLjA1Ny0yLjk4NSwwLjY2Ny0zLjU1LDEuODMyCgkJCWMtMC4zMDEsMC41MzUtMC41MDMsMS4xNDEtMC42MDcsMS44MTRjLTAuMTM5LDAuNzA3LTAuMjA3LDEuNDMyLTAuMjA3LDIuMTc0aC0yLjkzN2MtMC4wOTEtMi4yMDgsMC40MDctNC4xMTQsMS40OTMtNS43MTkKCQkJYzEuMDYyLTEuNjQsMi44NTUtMi40ODEsNS4zNzgtMi41MjdjMi4xNiwwLjAyMywzLjg3NCwwLjYwOCw1LjE0MSwxLjc1OGMxLjI3OCwxLjE2LDEuOTI5LDIuNzY0LDEuOTUsNC44MTEKCQkJYzAsMS4xNDItMC4xMzcsMi4xMTEtMC40MSwyLjkxMWMtMC4zMDksMC44NDUtMC43MzEsMS41OTMtMS4yNjgsMi4yNDNjLTAuNDkyLDAuNjUtMS4wNjgsMS4zMTgtMS43MywyLjAwMgoJCQljLTAuNjUsMC42OTctMS4zMTMsMS40NzktMS45ODcsMi4zNDZjLTAuMjM5LDAuMzc3LTAuNDI5LDAuNzc3LTAuNTY1LDEuMTk5Yy0wLjE2LDAuOTU5LTAuMjE3LDEuOTUxLTAuMTcxLDIuOTc5CgkJCUMyNi41ODksMzIuMjE4LDIzLjU3OCwzMi4yMTgsMjMuNTc4LDMyLjIxOHogTTIzLjU3OCwzOC4yMnYtMy40ODRoMy4wNzZ2My40ODRIMjMuNTc4eiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-inspector: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaW5zcGVjdG9yLWljb24tY29sb3IganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY2YzAtMS4xLS45LTItMi0yem0tNSAxNEg0di00aDExdjR6bTAtNUg0VjloMTF2NHptNSA1aC00VjloNHY5eiIvPgo8L3N2Zz4K);
  --jp-icon-json: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtanNvbi1pY29uLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0Y5QTgyNSI+CiAgICA8cGF0aCBkPSJNMjAuMiAxMS44Yy0xLjYgMC0xLjcuNS0xLjcgMSAwIC40LjEuOS4xIDEuMy4xLjUuMS45LjEgMS4zIDAgMS43LTEuNCAyLjMtMy41IDIuM2gtLjl2LTEuOWguNWMxLjEgMCAxLjQgMCAxLjQtLjggMC0uMyAwLS42LS4xLTEgMC0uNC0uMS0uOC0uMS0xLjIgMC0xLjMgMC0xLjggMS4zLTItMS4zLS4yLTEuMy0uNy0xLjMtMiAwLS40LjEtLjguMS0xLjIuMS0uNC4xLS43LjEtMSAwLS44LS40LS43LTEuNC0uOGgtLjVWNC4xaC45YzIuMiAwIDMuNS43IDMuNSAyLjMgMCAuNC0uMS45LS4xIDEuMy0uMS41LS4xLjktLjEgMS4zIDAgLjUuMiAxIDEuNyAxdjEuOHpNMS44IDEwLjFjMS42IDAgMS43LS41IDEuNy0xIDAtLjQtLjEtLjktLjEtMS4zLS4xLS41LS4xLS45LS4xLTEuMyAwLTEuNiAxLjQtMi4zIDMuNS0yLjNoLjl2MS45aC0uNWMtMSAwLTEuNCAwLTEuNC44IDAgLjMgMCAuNi4xIDEgMCAuMi4xLjYuMSAxIDAgMS4zIDAgMS44LTEuMyAyQzYgMTEuMiA2IDExLjcgNiAxM2MwIC40LS4xLjgtLjEgMS4yLS4xLjMtLjEuNy0uMSAxIDAgLjguMy44IDEuNC44aC41djEuOWgtLjljLTIuMSAwLTMuNS0uNi0zLjUtMi4zIDAtLjQuMS0uOS4xLTEuMy4xLS41LjEtLjkuMS0xLjMgMC0uNS0uMi0xLTEuNy0xdi0xLjl6Ii8+CiAgICA8Y2lyY2xlIGN4PSIxMSIgY3k9IjEzLjgiIHI9IjIuMSIvPgogICAgPGNpcmNsZSBjeD0iMTEiIGN5PSI4LjIiIHI9IjIuMSIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-julia: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDMyNSAzMDAiPgogIDxnIGNsYXNzPSJqcC1icmFuZDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjY2IzYzMzIj4KICAgIDxwYXRoIGQ9Ik0gMTUwLjg5ODQzOCAyMjUgQyAxNTAuODk4NDM4IDI2Ni40MjE4NzUgMTE3LjMyMDMxMiAzMDAgNzUuODk4NDM4IDMwMCBDIDM0LjQ3NjU2MiAzMDAgMC44OTg0MzggMjY2LjQyMTg3NSAwLjg5ODQzOCAyMjUgQyAwLjg5ODQzOCAxODMuNTc4MTI1IDM0LjQ3NjU2MiAxNTAgNzUuODk4NDM4IDE1MCBDIDExNy4zMjAzMTIgMTUwIDE1MC44OTg0MzggMTgzLjU3ODEyNSAxNTAuODk4NDM4IDIyNSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzM4OTgyNiI+CiAgICA8cGF0aCBkPSJNIDIzNy41IDc1IEMgMjM3LjUgMTE2LjQyMTg3NSAyMDMuOTIxODc1IDE1MCAxNjIuNSAxNTAgQyAxMjEuMDc4MTI1IDE1MCA4Ny41IDExNi40MjE4NzUgODcuNSA3NSBDIDg3LjUgMzMuNTc4MTI1IDEyMS4wNzgxMjUgMCAxNjIuNSAwIEMgMjAzLjkyMTg3NSAwIDIzNy41IDMzLjU3ODEyNSAyMzcuNSA3NSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzk1NThiMiI+CiAgICA8cGF0aCBkPSJNIDMyNC4xMDE1NjIgMjI1IEMgMzI0LjEwMTU2MiAyNjYuNDIxODc1IDI5MC41MjM0MzggMzAwIDI0OS4xMDE1NjIgMzAwIEMgMjA3LjY3OTY4OCAzMDAgMTc0LjEwMTU2MiAyNjYuNDIxODc1IDE3NC4xMDE1NjIgMjI1IEMgMTc0LjEwMTU2MiAxODMuNTc4MTI1IDIwNy42Nzk2ODggMTUwIDI0OS4xMDE1NjIgMTUwIEMgMjkwLjUyMzQzOCAxNTAgMzI0LjEwMTU2MiAxODMuNTc4MTI1IDMyNC4xMDE1NjIgMjI1Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-jupyter-favicon: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTUyIiBoZWlnaHQ9IjE2NSIgdmlld0JveD0iMCAwIDE1MiAxNjUiIHZlcnNpb249IjEuMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgPGcgY2xhc3M9ImpwLWp1cHl0ZXItaWNvbi1jb2xvciIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA3ODk0NywgMTEwLjU4MjkyNykiIGQ9Ik03NS45NDIyODQyLDI5LjU4MDQ1NjEgQzQzLjMwMjM5NDcsMjkuNTgwNDU2MSAxNC43OTY3ODMyLDE3LjY1MzQ2MzQgMCwwIEM1LjUxMDgzMjExLDE1Ljg0MDY4MjkgMTUuNzgxNTM4OSwyOS41NjY3NzMyIDI5LjM5MDQ5NDcsMzkuMjc4NDE3MSBDNDIuOTk5Nyw0OC45ODk4NTM3IDU5LjI3MzcsNTQuMjA2NzgwNSA3NS45NjA1Nzg5LDU0LjIwNjc4MDUgQzkyLjY0NzQ1NzksNTQuMjA2NzgwNSAxMDguOTIxNDU4LDQ4Ljk4OTg1MzcgMTIyLjUzMDY2MywzOS4yNzg0MTcxIEMxMzYuMTM5NDUzLDI5LjU2Njc3MzIgMTQ2LjQxMDI4NCwxNS44NDA2ODI5IDE1MS45MjExNTgsMCBDMTM3LjA4Nzg2OCwxNy42NTM0NjM0IDEwOC41ODI1ODksMjkuNTgwNDU2MSA3NS45NDIyODQyLDI5LjU4MDQ1NjEgTDc1Ljk0MjI4NDIsMjkuNTgwNDU2MSBaIiAvPgogICAgPHBhdGggdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMzczNjgsIDAuNzA0ODc4KSIgZD0iTTc1Ljk3ODQ1NzksMjQuNjI2NDA3MyBDMTA4LjYxODc2MywyNC42MjY0MDczIDEzNy4xMjQ0NTgsMzYuNTUzNDQxNSAxNTEuOTIxMTU4LDU0LjIwNjc4MDUgQzE0Ni40MTAyODQsMzguMzY2MjIyIDEzNi4xMzk0NTMsMjQuNjQwMTMxNyAxMjIuNTMwNjYzLDE0LjkyODQ4NzggQzEwOC45MjE0NTgsNS4yMTY4NDM5IDkyLjY0NzQ1NzksMCA3NS45NjA1Nzg5LDAgQzU5LjI3MzcsMCA0Mi45OTk3LDUuMjE2ODQzOSAyOS4zOTA0OTQ3LDE0LjkyODQ4NzggQzE1Ljc4MTUzODksMjQuNjQwMTMxNyA1LjUxMDgzMjExLDM4LjM2NjIyMiAwLDU0LjIwNjc4MDUgQzE0LjgzMzA4MTYsMzYuNTg5OTI5MyA0My4zMzg1Njg0LDI0LjYyNjQwNzMgNzUuOTc4NDU3OSwyNC42MjY0MDczIEw3NS45Nzg0NTc5LDI0LjYyNjQwNzMgWiIgLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-jupyter: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzkiIGhlaWdodD0iNTEiIHZpZXdCb3g9IjAgMCAzOSA1MSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTYzOCAtMjI4MSkiPgogICAgIDxnIGNsYXNzPSJqcC1qdXB5dGVyLWljb24tY29sb3IiIGZpbGw9IiNGMzc3MjYiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5Ljc0IDIzMTEuOTgpIiBkPSJNIDE4LjI2NDYgNy4xMzQxMUMgMTAuNDE0NSA3LjEzNDExIDMuNTU4NzIgNC4yNTc2IDAgMEMgMS4zMjUzOSAzLjgyMDQgMy43OTU1NiA3LjEzMDgxIDcuMDY4NiA5LjQ3MzAzQyAxMC4zNDE3IDExLjgxNTIgMTQuMjU1NyAxMy4wNzM0IDE4LjI2OSAxMy4wNzM0QyAyMi4yODIzIDEzLjA3MzQgMjYuMTk2MyAxMS44MTUyIDI5LjQ2OTQgOS40NzMwM0MgMzIuNzQyNCA3LjEzMDgxIDM1LjIxMjYgMy44MjA0IDM2LjUzOCAwQyAzMi45NzA1IDQuMjU3NiAyNi4xMTQ4IDcuMTM0MTEgMTguMjY0NiA3LjEzNDExWiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5LjczIDIyODUuNDgpIiBkPSJNIDE4LjI3MzMgNS45MzkzMUMgMjYuMTIzNSA1LjkzOTMxIDMyLjk3OTMgOC44MTU4MyAzNi41MzggMTMuMDczNEMgMzUuMjEyNiA5LjI1MzAzIDMyLjc0MjQgNS45NDI2MiAyOS40Njk0IDMuNjAwNEMgMjYuMTk2MyAxLjI1ODE4IDIyLjI4MjMgMCAxOC4yNjkgMEMgMTQuMjU1NyAwIDEwLjM0MTcgMS4yNTgxOCA3LjA2ODYgMy42MDA0QyAzLjc5NTU2IDUuOTQyNjIgMS4zMjUzOSA5LjI1MzAzIDAgMTMuMDczNEMgMy41Njc0NSA4LjgyNDYzIDEwLjQyMzIgNS45MzkzMSAxOC4yNzMzIDUuOTM5MzFaIi8+CiAgICA8L2c+CiAgICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjY5LjMgMjI4MS4zMSkiIGQ9Ik0gNS44OTM1MyAyLjg0NEMgNS45MTg4OSAzLjQzMTY1IDUuNzcwODUgNC4wMTM2NyA1LjQ2ODE1IDQuNTE2NDVDIDUuMTY1NDUgNS4wMTkyMiA0LjcyMTY4IDUuNDIwMTUgNC4xOTI5OSA1LjY2ODUxQyAzLjY2NDMgNS45MTY4OCAzLjA3NDQ0IDYuMDAxNTEgMi40OTgwNSA1LjkxMTcxQyAxLjkyMTY2IDUuODIxOSAxLjM4NDYzIDUuNTYxNyAwLjk1NDg5OCA1LjE2NDAxQyAwLjUyNTE3IDQuNzY2MzMgMC4yMjIwNTYgNC4yNDkwMyAwLjA4MzkwMzcgMy42Nzc1N0MgLTAuMDU0MjQ4MyAzLjEwNjExIC0wLjAyMTIzIDIuNTA2MTcgMC4xNzg3ODEgMS45NTM2NEMgMC4zNzg3OTMgMS40MDExIDAuNzM2ODA5IDAuOTIwODE3IDEuMjA3NTQgMC41NzM1MzhDIDEuNjc4MjYgMC4yMjYyNTkgMi4yNDA1NSAwLjAyNzU5MTkgMi44MjMyNiAwLjAwMjY3MjI5QyAzLjYwMzg5IC0wLjAzMDcxMTUgNC4zNjU3MyAwLjI0OTc4OSA0Ljk0MTQyIDAuNzgyNTUxQyA1LjUxNzExIDEuMzE1MzEgNS44NTk1NiAyLjA1Njc2IDUuODkzNTMgMi44NDRaIi8+CiAgICAgIDxwYXRoIHRyYW5zZm9ybT0idHJhbnNsYXRlKDE2MzkuOCAyMzIzLjgxKSIgZD0iTSA3LjQyNzg5IDMuNTgzMzhDIDcuNDYwMDggNC4zMjQzIDcuMjczNTUgNS4wNTgxOSA2Ljg5MTkzIDUuNjkyMTNDIDYuNTEwMzEgNi4zMjYwNyA1Ljk1MDc1IDYuODMxNTYgNS4yODQxMSA3LjE0NDZDIDQuNjE3NDcgNy40NTc2MyAzLjg3MzcxIDcuNTY0MTQgMy4xNDcwMiA3LjQ1MDYzQyAyLjQyMDMyIDcuMzM3MTIgMS43NDMzNiA3LjAwODcgMS4yMDE4NCA2LjUwNjk1QyAwLjY2MDMyOCA2LjAwNTIgMC4yNzg2MSA1LjM1MjY4IDAuMTA1MDE3IDQuNjMyMDJDIC0wLjA2ODU3NTcgMy45MTEzNSAtMC4wMjYyMzYxIDMuMTU0OTQgMC4yMjY2NzUgMi40NTg1NkMgMC40Nzk1ODcgMS43NjIxNyAwLjkzMTY5NyAxLjE1NzEzIDEuNTI1NzYgMC43MjAwMzNDIDIuMTE5ODMgMC4yODI5MzUgMi44MjkxNCAwLjAzMzQzOTUgMy41NjM4OSAwLjAwMzEzMzQ0QyA0LjU0NjY3IC0wLjAzNzQwMzMgNS41MDUyOSAwLjMxNjcwNiA2LjIyOTYxIDAuOTg3ODM1QyA2Ljk1MzkzIDEuNjU4OTYgNy4zODQ4NCAyLjU5MjM1IDcuNDI3ODkgMy41ODMzOEwgNy40Mjc4OSAzLjU4MzM4WiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM4LjM2IDIyODYuMDYpIiBkPSJNIDIuMjc0NzEgNC4zOTYyOUMgMS44NDM2MyA0LjQxNTA4IDEuNDE2NzEgNC4zMDQ0NSAxLjA0Nzk5IDQuMDc4NDNDIDAuNjc5MjY4IDMuODUyNCAwLjM4NTMyOCAzLjUyMTE0IDAuMjAzMzcxIDMuMTI2NTZDIDAuMDIxNDEzNiAyLjczMTk4IC0wLjA0MDM3OTggMi4yOTE4MyAwLjAyNTgxMTYgMS44NjE4MUMgMC4wOTIwMDMxIDEuNDMxOCAwLjI4MzIwNCAxLjAzMTI2IDAuNTc1MjEzIDAuNzEwODgzQyAwLjg2NzIyMiAwLjM5MDUxIDEuMjQ2OTEgMC4xNjQ3MDggMS42NjYyMiAwLjA2MjA1OTJDIDIuMDg1NTMgLTAuMDQwNTg5NyAyLjUyNTYxIC0wLjAxNTQ3MTQgMi45MzA3NiAwLjEzNDIzNUMgMy4zMzU5MSAwLjI4Mzk0MSAzLjY4NzkyIDAuNTUxNTA1IDMuOTQyMjIgMC45MDMwNkMgNC4xOTY1MiAxLjI1NDYyIDQuMzQxNjkgMS42NzQzNiA0LjM1OTM1IDIuMTA5MTZDIDQuMzgyOTkgMi42OTEwNyA0LjE3Njc4IDMuMjU4NjkgMy43ODU5NyAzLjY4NzQ2QyAzLjM5NTE2IDQuMTE2MjQgMi44NTE2NiA0LjM3MTE2IDIuMjc0NzEgNC4zOTYyOUwgMi4yNzQ3MSA0LjM5NjI5WiIvPgogICAgPC9nPgogIDwvZz4+Cjwvc3ZnPgo=);
  --jp-icon-jupyterlab-wordmark: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyMDAiIHZpZXdCb3g9IjAgMCAxODYwLjggNDc1Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0RTRFNEUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQ4MC4xMzY0MDEsIDY0LjI3MTQ5MykiPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMDAwMDAsIDU4Ljg3NTU2NikiPgogICAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA4NzYwMywgMC4xNDAyOTQpIj4KICAgICAgICA8cGF0aCBkPSJNLTQyNi45LDE2OS44YzAsNDguNy0zLjcsNjQuNy0xMy42LDc2LjRjLTEwLjgsMTAtMjUsMTUuNS0zOS43LDE1LjVsMy43LDI5IGMyMi44LDAuMyw0NC44LTcuOSw2MS45LTIzLjFjMTcuOC0xOC41LDI0LTQ0LjEsMjQtODMuM1YwSC00Mjd2MTcwLjFMLTQyNi45LDE2OS44TC00MjYuOSwxNjkuOHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTU1LjA0NTI5NiwgNTYuODM3MTA0KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuNTYyNDUzLCAxLjc5OTg0MikiPgogICAgICAgIDxwYXRoIGQ9Ik0tMzEyLDE0OGMwLDIxLDAsMzkuNSwxLjcsNTUuNGgtMzEuOGwtMi4xLTMzLjNoLTAuOGMtNi43LDExLjYtMTYuNCwyMS4zLTI4LDI3LjkgYy0xMS42LDYuNi0yNC44LDEwLTM4LjIsOS44Yy0zMS40LDAtNjktMTcuNy02OS04OVYwaDM2LjR2MTEyLjdjMCwzOC43LDExLjYsNjQuNyw0NC42LDY0LjdjMTAuMy0wLjIsMjAuNC0zLjUsMjguOS05LjQgYzguNS01LjksMTUuMS0xNC4zLDE4LjktMjMuOWMyLjItNi4xLDMuMy0xMi41LDMuMy0xOC45VjAuMmgzNi40VjE0OEgtMzEyTC0zMTIsMTQ4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzOTAuMDEzMzIyLCA1My40Nzk2MzgpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS43MDY0NTgsIDAuMjMxNDI1KSI+CiAgICAgICAgPHBhdGggZD0iTS00NzguNiw3MS40YzAtMjYtMC44LTQ3LTEuNy02Ni43aDMyLjdsMS43LDM0LjhoMC44YzcuMS0xMi41LDE3LjUtMjIuOCwzMC4xLTI5LjcgYzEyLjUtNywyNi43LTEwLjMsNDEtOS44YzQ4LjMsMCw4NC43LDQxLjcsODQuNywxMDMuM2MwLDczLjEtNDMuNywxMDkuMi05MSwxMDkuMmMtMTIuMSwwLjUtMjQuMi0yLjItMzUtNy44IGMtMTAuOC01LjYtMTkuOS0xMy45LTI2LjYtMjQuMmgtMC44VjI5MWgtMzZ2LTIyMEwtNDc4LjYsNzEuNEwtNDc4LjYsNzEuNHogTS00NDIuNiwxMjUuNmMwLjEsNS4xLDAuNiwxMC4xLDEuNywxNS4xIGMzLDEyLjMsOS45LDIzLjMsMTkuOCwzMS4xYzkuOSw3LjgsMjIuMSwxMi4xLDM0LjcsMTIuMWMzOC41LDAsNjAuNy0zMS45LDYwLjctNzguNWMwLTQwLjctMjEuMS03NS42LTU5LjUtNzUuNiBjLTEyLjksMC40LTI1LjMsNS4xLTM1LjMsMTMuNGMtOS45LDguMy0xNi45LDE5LjctMTkuNiwzMi40Yy0xLjUsNC45LTIuMywxMC0yLjUsMTUuMVYxMjUuNkwtNDQyLjYsMTI1LjZMLTQ0Mi42LDEyNS42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSg2MDYuNzQwNzI2LCA1Ni44MzcxMDQpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC43NTEyMjYsIDEuOTg5Mjk5KSI+CiAgICAgICAgPHBhdGggZD0iTS00NDAuOCwwbDQzLjcsMTIwLjFjNC41LDEzLjQsOS41LDI5LjQsMTIuOCw0MS43aDAuOGMzLjctMTIuMiw3LjktMjcuNywxMi44LTQyLjQgbDM5LjctMTE5LjJoMzguNUwtMzQ2LjksMTQ1Yy0yNiw2OS43LTQzLjcsMTA1LjQtNjguNiwxMjcuMmMtMTIuNSwxMS43LTI3LjksMjAtNDQuNiwyMy45bC05LjEtMzEuMSBjMTEuNy0zLjksMjIuNS0xMC4xLDMxLjgtMTguMWMxMy4yLTExLjEsMjMuNy0yNS4yLDMwLjYtNDEuMmMxLjUtMi44LDIuNS01LjcsMi45LTguOGMtMC4zLTMuMy0xLjItNi42LTIuNS05LjdMLTQ4MC4yLDAuMSBoMzkuN0wtNDQwLjgsMEwtNDQwLjgsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoODIyLjc0ODEwNCwgMC4wMDAwMDApIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS40NjQwNTAsIDAuMzc4OTE0KSI+CiAgICAgICAgPHBhdGggZD0iTS00MTMuNywwdjU4LjNoNTJ2MjguMmgtNTJWMTk2YzAsMjUsNywzOS41LDI3LjMsMzkuNWM3LjEsMC4xLDE0LjItMC43LDIxLjEtMi41IGwxLjcsMjcuN2MtMTAuMywzLjctMjEuMyw1LjQtMzIuMiw1Yy03LjMsMC40LTE0LjYtMC43LTIxLjMtMy40Yy02LjgtMi43LTEyLjktNi44LTE3LjktMTIuMWMtMTAuMy0xMC45LTE0LjEtMjktMTQuMS01Mi45IFY4Ni41aC0zMVY1OC4zaDMxVjkuNkwtNDEzLjcsMEwtNDEzLjcsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOTc0LjQzMzI4NiwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDAuOTkwMDM0LCAwLjYxMDMzOSkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDQ1LjgsMTEzYzAuOCw1MCwzMi4yLDcwLjYsNjguNiw3MC42YzE5LDAuNiwzNy45LTMsNTUuMy0xMC41bDYuMiwyNi40IGMtMjAuOSw4LjktNDMuNSwxMy4xLTY2LjIsMTIuNmMtNjEuNSwwLTk4LjMtNDEuMi05OC4zLTEwMi41Qy00ODAuMiw0OC4yLTQ0NC43LDAtMzg2LjUsMGM2NS4yLDAsODIuNyw1OC4zLDgyLjcsOTUuNyBjLTAuMSw1LjgtMC41LDExLjUtMS4yLDE3LjJoLTE0MC42SC00NDUuOEwtNDQ1LjgsMTEzeiBNLTMzOS4yLDg2LjZjMC40LTIzLjUtOS41LTYwLjEtNTAuNC02MC4xIGMtMzYuOCwwLTUyLjgsMzQuNC01NS43LDYwLjFILTMzOS4yTC0zMzkuMiw4Ni42TC0zMzkuMiw4Ni42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxMjAxLjk2MTA1OCwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuMTc5NjQwLCAwLjcwNTA2OCkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDc4LjYsNjhjMC0yMy45LTAuNC00NC41LTEuNy02My40aDMxLjhsMS4yLDM5LjloMS43YzkuMS0yNy4zLDMxLTQ0LjUsNTUuMy00NC41IGMzLjUtMC4xLDcsMC40LDEwLjMsMS4ydjM0LjhjLTQuMS0wLjktOC4yLTEuMy0xMi40LTEuMmMtMjUuNiwwLTQzLjcsMTkuNy00OC43LDQ3LjRjLTEsNS43LTEuNiwxMS41LTEuNywxNy4ydjEwOC4zaC0zNlY2OCBMLTQ3OC42LDY4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCBkPSJNMTM1Mi4zLDMyNi4yaDM3VjI4aC0zN1YzMjYuMnogTTE2MDQuOCwzMjYuMmMtMi41LTEzLjktMy40LTMxLjEtMy40LTQ4Ljd2LTc2IGMwLTQwLjctMTUuMS04My4xLTc3LjMtODMuMWMtMjUuNiwwLTUwLDcuMS02Ni44LDE4LjFsOC40LDI0LjRjMTQuMy05LjIsMzQtMTUuMSw1My0xNS4xYzQxLjYsMCw0Ni4yLDMwLjIsNDYuMiw0N3Y0LjIgYy03OC42LTAuNC0xMjIuMywyNi41LTEyMi4zLDc1LjZjMCwyOS40LDIxLDU4LjQsNjIuMiw1OC40YzI5LDAsNTAuOS0xNC4zLDYyLjItMzAuMmgxLjNsMi45LDI1LjZIMTYwNC44eiBNMTU2NS43LDI1Ny43IGMwLDMuOC0wLjgsOC0yLjEsMTEuOGMtNS45LDE3LjItMjIuNywzNC00OS4yLDM0Yy0xOC45LDAtMzQuOS0xMS4zLTM0LjktMzUuM2MwLTM5LjUsNDUuOC00Ni42LDg2LjItNDUuOFYyNTcuN3ogTTE2OTguNSwzMjYuMiBsMS43LTMzLjZoMS4zYzE1LjEsMjYuOSwzOC43LDM4LjIsNjguMSwzOC4yYzQ1LjQsMCw5MS4yLTM2LjEsOTEuMi0xMDguOGMwLjQtNjEuNy0zNS4zLTEwMy43LTg1LjctMTAzLjcgYy0zMi44LDAtNTYuMywxNC43LTY5LjMsMzcuNGgtMC44VjI4aC0zNi42djI0NS43YzAsMTguMS0wLjgsMzguNi0xLjcsNTIuNUgxNjk4LjV6IE0xNzA0LjgsMjA4LjJjMC01LjksMS4zLTEwLjksMi4xLTE1LjEgYzcuNi0yOC4xLDMxLjEtNDUuNCw1Ni4zLTQ1LjRjMzkuNSwwLDYwLjUsMzQuOSw2MC41LDc1LjZjMCw0Ni42LTIzLjEsNzguMS02MS44LDc4LjFjLTI2LjksMC00OC4zLTE3LjYtNTUuNS00My4zIGMtMC44LTQuMi0xLjctOC44LTEuNy0xMy40VjIwOC4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzYxNjE2MSIgZD0iTTE1IDlIOXY2aDZWOXptLTIgNGgtMnYtMmgydjJ6bTgtMlY5aC0yVjdjMC0xLjEtLjktMi0yLTJoLTJWM2gtMnYyaC0yVjNIOXYySDdjLTEuMSAwLTIgLjktMiAydjJIM3YyaDJ2MkgzdjJoMnYyYzAgMS4xLjkgMiAyIDJoMnYyaDJ2LTJoMnYyaDJ2LTJoMmMxLjEgMCAyLS45IDItMnYtMmgydi0yaC0ydi0yaDJ6bS00IDZIN1Y3aDEwdjEweiIvPgo8L3N2Zz4K);
  --jp-icon-keyboard: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMTdjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY3YzAtMS4xLS45LTItMi0yem0tOSAzaDJ2MmgtMlY4em0wIDNoMnYyaC0ydi0yek04IDhoMnYySDhWOHptMCAzaDJ2Mkg4di0yem0tMSAySDV2LTJoMnYyem0wLTNINVY4aDJ2MnptOSA3SDh2LTJoOHYyem0wLTRoLTJ2LTJoMnYyem0wLTNoLTJWOGgydjJ6bTMgM2gtMnYtMmgydjJ6bTAtM2gtMlY4aDJ2MnoiLz4KPC9zdmc+Cg==);
  --jp-icon-launch: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMzIgMzIiIHdpZHRoPSIzMiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0yNiwyOEg2YTIuMDAyNywyLjAwMjcsMCwwLDEtMi0yVjZBMi4wMDI3LDIuMDAyNywwLDAsMSw2LDRIMTZWNkg2VjI2SDI2VjE2aDJWMjZBMi4wMDI3LDIuMDAyNywwLDAsMSwyNiwyOFoiLz4KICAgIDxwb2x5Z29uIHBvaW50cz0iMjAgMiAyMCA0IDI2LjU4NiA0IDE4IDEyLjU4NiAxOS40MTQgMTQgMjggNS40MTQgMjggMTIgMzAgMTIgMzAgMiAyMCAyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-launcher: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkgMTlINVY1aDdWM0g1YTIgMiAwIDAwLTIgMnYxNGEyIDIgMCAwMDIgMmgxNGMxLjEgMCAyLS45IDItMnYtN2gtMnY3ek0xNCAzdjJoMy41OWwtOS44MyA5LjgzIDEuNDEgMS40MUwxOSA2LjQxVjEwaDJWM2gtN3oiLz4KPC9zdmc+Cg==);
  --jp-icon-line-form: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGZpbGw9IndoaXRlIiBkPSJNNS44OCA0LjEyTDEzLjc2IDEybC03Ljg4IDcuODhMOCAyMmwxMC0xMEw4IDJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-link: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMuOSAxMmMwLTEuNzEgMS4zOS0zLjEgMy4xLTMuMWg0VjdIN2MtMi43NiAwLTUgMi4yNC01IDVzMi4yNCA1IDUgNWg0di0xLjlIN2MtMS43MSAwLTMuMS0xLjM5LTMuMS0zLjF6TTggMTNoOHYtMkg4djJ6bTktNmgtNHYxLjloNGMxLjcxIDAgMy4xIDEuMzkgMy4xIDMuMXMtMS4zOSAzLjEtMy4xIDMuMWgtNFYxN2g0YzIuNzYgMCA1LTIuMjQgNS01cy0yLjI0LTUtNS01eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xOSA1djE0SDVWNWgxNG0xLjEtMkgzLjljLS41IDAtLjkuNC0uOS45djE2LjJjMCAuNC40LjkuOS45aDE2LjJjLjQgMCAuOS0uNS45LS45VjMuOWMwLS41LS41LS45LS45LS45ek0xMSA3aDZ2MmgtNlY3em0wIDRoNnYyaC02di0yem0wIDRoNnYyaC02ek03IDdoMnYySDd6bTAgNGgydjJIN3ptMCA0aDJ2Mkg3eiIvPgo8L3N2Zz4K);
  --jp-icon-markdown: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjN0IxRkEyIiBkPSJNNSAxNC45aDEybC02LjEgNnptOS40LTYuOGMwLTEuMy0uMS0yLjktLjEtNC41LS40IDEuNC0uOSAyLjktMS4zIDQuM2wtMS4zIDQuM2gtMkw4LjUgNy45Yy0uNC0xLjMtLjctMi45LTEtNC4zLS4xIDEuNi0uMSAzLjItLjIgNC42TDcgMTIuNEg0LjhsLjctMTFoMy4zTDEwIDVjLjQgMS4yLjcgMi43IDEgMy45LjMtMS4yLjctMi42IDEtMy45bDEuMi0zLjdoMy4zbC42IDExaC0yLjRsLS4zLTQuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-move-down: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNMTIuNDcxIDcuNTI4OTlDMTIuNzYzMiA3LjIzNjg0IDEyLjc2MzIgNi43NjMxNiAxMi40NzEgNi40NzEwMVY2LjQ3MTAxQzEyLjE3OSA2LjE3OTA1IDExLjcwNTcgNi4xNzg4NCAxMS40MTM1IDYuNDcwNTRMNy43NSAxMC4xMjc1VjEuNzVDNy43NSAxLjMzNTc5IDcuNDE0MjEgMSA3IDFWMUM2LjU4NTc5IDEgNi4yNSAxLjMzNTc5IDYuMjUgMS43NVYxMC4xMjc1TDIuNTk3MjYgNi40NjgyMkMyLjMwMzM4IDYuMTczODEgMS44MjY0MSA2LjE3MzU5IDEuNTMyMjYgNi40Njc3NFY2LjQ2Nzc0QzEuMjM4MyA2Ljc2MTcgMS4yMzgzIDcuMjM4MyAxLjUzMjI2IDcuNTMyMjZMNi4yOTI4OSAxMi4yOTI5QzYuNjgzNDIgMTIuNjgzNCA3LjMxNjU4IDEyLjY4MzQgNy43MDcxMSAxMi4yOTI5TDEyLjQ3MSA3LjUyODk5WiIgZmlsbD0iIzYxNjE2MSIvPgo8L3N2Zz4K);
  --jp-icon-move-up: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNMS41Mjg5OSA2LjQ3MTAxQzEuMjM2ODQgNi43NjMxNiAxLjIzNjg0IDcuMjM2ODQgMS41Mjg5OSA3LjUyODk5VjcuNTI4OTlDMS44MjA5NSA3LjgyMDk1IDIuMjk0MjYgNy44MjExNiAyLjU4NjQ5IDcuNTI5NDZMNi4yNSAzLjg3MjVWMTIuMjVDNi4yNSAxMi42NjQyIDYuNTg1NzkgMTMgNyAxM1YxM0M3LjQxNDIxIDEzIDcuNzUgMTIuNjY0MiA3Ljc1IDEyLjI1VjMuODcyNUwxMS40MDI3IDcuNTMxNzhDMTEuNjk2NiA3LjgyNjE5IDEyLjE3MzYgNy44MjY0MSAxMi40Njc3IDcuNTMyMjZWNy41MzIyNkMxMi43NjE3IDcuMjM4MyAxMi43NjE3IDYuNzYxNyAxMi40Njc3IDYuNDY3NzRMNy43MDcxMSAxLjcwNzExQzcuMzE2NTggMS4zMTY1OCA2LjY4MzQyIDEuMzE2NTggNi4yOTI4OSAxLjcwNzExTDEuNTI4OTkgNi40NzEwMVoiIGZpbGw9IiM2MTYxNjEiLz4KPC9zdmc+Cg==);
  --jp-icon-new-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwIDZoLThsLTItMkg0Yy0xLjExIDAtMS45OS44OS0xLjk5IDJMMiAxOGMwIDEuMTEuODkgMiAyIDJoMTZjMS4xMSAwIDItLjg5IDItMlY4YzAtMS4xMS0uODktMi0yLTJ6bS0xIDhoLTN2M2gtMnYtM2gtM3YtMmgzVjloMnYzaDN2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-not-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI1IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMTkgMTcuMTg0NCAyLjk2OTY4IDE0LjMwMzIgMS44NjA5NCAxMS40NDA5WiIvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24yIiBzdHJva2U9IiMzMzMzMzMiIHN0cm9rZS13aWR0aD0iMiIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOS4zMTU5MiA5LjMyMDMxKSIgZD0iTTcuMzY4NDIgMEwwIDcuMzY0NzkiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDkuMzE1OTIgMTYuNjgzNikgc2NhbGUoMSAtMSkiIGQ9Ik03LjM2ODQyIDBMMCA3LjM2NDc5Ii8+Cjwvc3ZnPgo=);
  --jp-icon-notebook: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtbm90ZWJvb2staWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNFRjZDMDAiPgogICAgPHBhdGggZD0iTTE4LjcgMy4zdjE1LjRIMy4zVjMuM2gxNS40bTEuNS0xLjVIMS44djE4LjNoMTguM2wuMS0xOC4zeiIvPgogICAgPHBhdGggZD0iTTE2LjUgMTYuNWwtNS40LTQuMy01LjYgNC4zdi0xMWgxMXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-numbering: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTQgMTlINlYxOS41SDVWMjAuNUg2VjIxSDRWMjJIN1YxOEg0VjE5Wk01IDEwSDZWNkg0VjdINVYxMFpNNCAxM0g1LjhMNCAxNS4xVjE2SDdWMTVINS4yTDcgMTIuOVYxMkg0VjEzWk05IDdWOUgyM1Y3SDlaTTkgMjFIMjNWMTlIOVYyMVpNOSAxNUgyM1YxM0g5VjE1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-offline-bolt: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDIuMDJjLTUuNTEgMC05Ljk4IDQuNDctOS45OCA5Ljk4czQuNDcgOS45OCA5Ljk4IDkuOTggOS45OC00LjQ3IDkuOTgtOS45OFMxNy41MSAyLjAyIDEyIDIuMDJ6TTExLjQ4IDIwdi02LjI2SDhMMTMgNHY2LjI2aDMuMzVMMTEuNDggMjB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-palette: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE4IDEzVjIwSDRWNkg5LjAyQzkuMDcgNS4yOSA5LjI0IDQuNjIgOS41IDRINEMyLjkgNCAyIDQuOSAyIDZWMjBDMiAyMS4xIDIuOSAyMiA0IDIySDE4QzE5LjEgMjIgMjAgMjEuMSAyMCAyMFYxNUwxOCAxM1pNMTkuMyA4Ljg5QzE5Ljc0IDguMTkgMjAgNy4zOCAyMCA2LjVDMjAgNC4wMSAxNy45OSAyIDE1LjUgMkMxMy4wMSAyIDExIDQuMDEgMTEgNi41QzExIDguOTkgMTMuMDEgMTEgMTUuNDkgMTFDMTYuMzcgMTEgMTcuMTkgMTAuNzQgMTcuODggMTAuM0wyMSAxMy40MkwyMi40MiAxMkwxOS4zIDguODlaTTE1LjUgOUMxNC4xMiA5IDEzIDcuODggMTMgNi41QzEzIDUuMTIgMTQuMTIgNCAxNS41IDRDMTYuODggNCAxOCA1LjEyIDE4IDYuNUMxOCA3Ljg4IDE2Ljg4IDkgMTUuNSA5WiIvPgogICAgPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik00IDZIOS4wMTg5NEM5LjAwNjM5IDYuMTY1MDIgOSA2LjMzMTc2IDkgNi41QzkgOC44MTU3NyAxMC4yMTEgMTAuODQ4NyAxMi4wMzQzIDEySDlWMTRIMTZWMTIuOTgxMUMxNi41NzAzIDEyLjkzNzcgMTcuMTIgMTIuODIwNyAxNy42Mzk2IDEyLjYzOTZMMTggMTNWMjBINFY2Wk04IDhINlYxMEg4VjhaTTYgMTJIOFYxNEg2VjEyWk04IDE2SDZWMThIOFYxNlpNOSAxNkgxNlYxOEg5VjE2WiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-paste: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE5IDJoLTQuMThDMTQuNC44NCAxMy4zIDAgMTIgMGMtMS4zIDAtMi40Ljg0LTIuODIgMkg1Yy0xLjEgMC0yIC45LTIgMnYxNmMwIDEuMS45IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjRjMC0xLjEtLjktMi0yLTJ6bS03IDBjLjU1IDAgMSAuNDUgMSAxcy0uNDUgMS0xIDEtMS0uNDUtMS0xIC40NS0xIDEtMXptNyAxOEg1VjRoMnYzaDEwVjRoMnYxNnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-pdf: url(data:image/svg+xml;base64,PHN2ZwogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyMiAyMiIgd2lkdGg9IjE2Ij4KICAgIDxwYXRoIHRyYW5zZm9ybT0icm90YXRlKDQ1KSIgY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0ZGMkEyQSIKICAgICAgIGQ9Im0gMjIuMzQ0MzY5LC0zLjAxNjM2NDIgaCA1LjYzODYwNCB2IDEuNTc5MjQzMyBoIC0zLjU0OTIyNyB2IDEuNTA4NjkyOTkgaCAzLjMzNzU3NiBWIDEuNjUwODE1NCBoIC0zLjMzNzU3NiB2IDMuNDM1MjYxMyBoIC0yLjA4OTM3NyB6IG0gLTcuMTM2NDQ0LDEuNTc5MjQzMyB2IDQuOTQzOTU0MyBoIDAuNzQ4OTIgcSAxLjI4MDc2MSwwIDEuOTUzNzAzLC0wLjYzNDk1MzUgMC42NzgzNjksLTAuNjM0OTUzNSAwLjY3ODM2OSwtMS44NDUxNjQxIDAsLTEuMjA0NzgzNTUgLTAuNjcyOTQyLC0xLjgzNDMxMDExIC0wLjY3Mjk0MiwtMC42Mjk1MjY1OSAtMS45NTkxMywtMC42Mjk1MjY1OSB6IG0gLTIuMDg5Mzc3LC0xLjU3OTI0MzMgaCAyLjIwMzM0MyBxIDEuODQ1MTY0LDAgMi43NDYwMzksMC4yNjU5MjA3IDAuOTA2MzAxLDAuMjYwNDkzNyAxLjU1MjEwOCwwLjg5MDAyMDMgMC41Njk4MywwLjU0ODEyMjMgMC44NDY2MDUsMS4yNjQ0ODAwNiAwLjI3Njc3NCwwLjcxNjM1NzgxIDAuMjc2Nzc0LDEuNjIyNjU4OTQgMCwwLjkxNzE1NTEgLTAuMjc2Nzc0LDEuNjM4OTM5OSAtMC4yNzY3NzUsMC43MTYzNTc4IC0wLjg0NjYwNSwxLjI2NDQ4IC0wLjY1MTIzNCwwLjYyOTUyNjYgLTEuNTYyOTYyLDAuODk1NDQ3MyAtMC45MTE3MjgsMC4yNjA0OTM3IC0yLjczNTE4NSwwLjI2MDQ5MzcgaCAtMi4yMDMzNDMgeiBtIC04LjE0NTg1NjUsMCBoIDMuNDY3ODIzIHEgMS41NDY2ODE2LDAgMi4zNzE1Nzg1LDAuNjg5MjIzIDAuODMwMzI0LDAuNjgzNzk2MSAwLjgzMDMyNCwxLjk1MzcwMzE0IDAsMS4yNzUzMzM5NyAtMC44MzAzMjQsMS45NjQ1NTcwNiBRIDkuOTg3MTk2MSwyLjI3NDkxNSA4LjQ0MDUxNDUsMi4yNzQ5MTUgSCA3LjA2MjA2ODQgViA1LjA4NjA3NjcgSCA0Ljk3MjY5MTUgWiBtIDIuMDg5Mzc2OSwxLjUxNDExOTkgdiAyLjI2MzAzOTQzIGggMS4xNTU5NDEgcSAwLjYwNzgxODgsMCAwLjkzODg2MjksLTAuMjkzMDU1NDcgMC4zMzEwNDQxLC0wLjI5ODQ4MjQxIDAuMzMxMDQ0MSwtMC44NDExNzc3MiAwLC0wLjU0MjY5NTMxIC0wLjMzMTA0NDEsLTAuODM1NzUwNzQgLTAuMzMxMDQ0MSwtMC4yOTMwNTU1IC0wLjkzODg2MjksLTAuMjkzMDU1NSB6IgovPgo8L3N2Zz4K);
  --jp-icon-python: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iLTEwIC0xMCAxMzEuMTYxMzYxNjk0MzM1OTQgMTMyLjM4ODk5OTkzODk2NDg0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMzA2OTk4IiBkPSJNIDU0LjkxODc4NSw5LjE5Mjc0MjFlLTQgQyA1MC4zMzUxMzIsMC4wMjIyMTcyNyA0NS45NTc4NDYsMC40MTMxMzY5NyA0Mi4xMDYyODUsMS4wOTQ2NjkzIDMwLjc2MDA2OSwzLjA5OTE3MzEgMjguNzAwMDM2LDcuMjk0NzcxNCAyOC43MDAwMzUsMTUuMDMyMTY5IHYgMTAuMjE4NzUgaCAyNi44MTI1IHYgMy40MDYyNSBoIC0yNi44MTI1IC0xMC4wNjI1IGMgLTcuNzkyNDU5LDAgLTE0LjYxNTc1ODgsNC42ODM3MTcgLTE2Ljc0OTk5OTgsMTMuNTkzNzUgLTIuNDYxODE5OTgsMTAuMjEyOTY2IC0yLjU3MTAxNTA4LDE2LjU4NjAyMyAwLDI3LjI1IDEuOTA1OTI4Myw3LjkzNzg1MiA2LjQ1NzU0MzIsMTMuNTkzNzQ4IDE0LjI0OTk5OTgsMTMuNTkzNzUgaCA5LjIxODc1IHYgLTEyLjI1IGMgMCwtOC44NDk5MDIgNy42NTcxNDQsLTE2LjY1NjI0OCAxNi43NSwtMTYuNjU2MjUgaCAyNi43ODEyNSBjIDcuNDU0OTUxLDAgMTMuNDA2MjUzLC02LjEzODE2NCAxMy40MDYyNSwtMTMuNjI1IHYgLTI1LjUzMTI1IGMgMCwtNy4yNjYzMzg2IC02LjEyOTk4LC0xMi43MjQ3NzcxIC0xMy40MDYyNSwtMTMuOTM3NDk5NyBDIDY0LjI4MTU0OCwwLjMyNzk0Mzk3IDU5LjUwMjQzOCwtMC4wMjAzNzkwMyA1NC45MTg3ODUsOS4xOTI3NDIxZS00IFogbSAtMTQuNSw4LjIxODc1MDEyNTc5IGMgMi43Njk1NDcsMCA1LjAzMTI1LDIuMjk4NjQ1NiA1LjAzMTI1LDUuMTI0OTk5NiAtMmUtNiwyLjgxNjMzNiAtMi4yNjE3MDMsNS4wOTM3NSAtNS4wMzEyNSw1LjA5Mzc1IC0yLjc3OTQ3NiwtMWUtNiAtNS4wMzEyNSwtMi4yNzc0MTUgLTUuMDMxMjUsLTUuMDkzNzUgLTEwZS03LC0yLjgyNjM1MyAyLjI1MTc3NCwtNS4xMjQ5OTk2IDUuMDMxMjUsLTUuMTI0OTk5NiB6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2ZmZDQzYiIgZD0ibSA4NS42Mzc1MzUsMjguNjU3MTY5IHYgMTEuOTA2MjUgYyAwLDkuMjMwNzU1IC03LjgyNTg5NSwxNi45OTk5OTkgLTE2Ljc1LDE3IGggLTI2Ljc4MTI1IGMgLTcuMzM1ODMzLDAgLTEzLjQwNjI0OSw2LjI3ODQ4MyAtMTMuNDA2MjUsMTMuNjI1IHYgMjUuNTMxMjQ3IGMgMCw3LjI2NjM0NCA2LjMxODU4OCwxMS41NDAzMjQgMTMuNDA2MjUsMTMuNjI1MDA0IDguNDg3MzMxLDIuNDk1NjEgMTYuNjI2MjM3LDIuOTQ2NjMgMjYuNzgxMjUsMCA2Ljc1MDE1NSwtMS45NTQzOSAxMy40MDYyNTMsLTUuODg3NjEgMTMuNDA2MjUsLTEzLjYyNTAwNCBWIDg2LjUwMDkxOSBoIC0yNi43ODEyNSB2IC0zLjQwNjI1IGggMjYuNzgxMjUgMTMuNDA2MjU0IGMgNy43OTI0NjEsMCAxMC42OTYyNTEsLTUuNDM1NDA4IDEzLjQwNjI0MSwtMTMuNTkzNzUgMi43OTkzMywtOC4zOTg4ODYgMi42ODAyMiwtMTYuNDc1Nzc2IDAsLTI3LjI1IC0xLjkyNTc4LC03Ljc1NzQ0MSAtNS42MDM4NywtMTMuNTkzNzUgLTEzLjQwNjI0MSwtMTMuNTkzNzUgeiBtIC0xNS4wNjI1LDY0LjY1NjI1IGMgMi43Nzk0NzgsM2UtNiA1LjAzMTI1LDIuMjc3NDE3IDUuMDMxMjUsNS4wOTM3NDcgLTJlLTYsMi44MjYzNTQgLTIuMjUxNzc1LDUuMTI1MDA0IC01LjAzMTI1LDUuMTI1MDA0IC0yLjc2OTU1LDAgLTUuMDMxMjUsLTIuMjk4NjUgLTUuMDMxMjUsLTUuMTI1MDA0IDJlLTYsLTIuODE2MzMgMi4yNjE2OTcsLTUuMDkzNzQ3IDUuMDMxMjUsLTUuMDkzNzQ3IHoiLz4KPC9zdmc+Cg==);
  --jp-icon-r-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjE5NkYzIiBkPSJNNC40IDIuNWMxLjItLjEgMi45LS4zIDQuOS0uMyAyLjUgMCA0LjEuNCA1LjIgMS4zIDEgLjcgMS41IDEuOSAxLjUgMy41IDAgMi0xLjQgMy41LTIuOSA0LjEgMS4yLjQgMS43IDEuNiAyLjIgMyAuNiAxLjkgMSAzLjkgMS4zIDQuNmgtMy44Yy0uMy0uNC0uOC0xLjctMS4yLTMuN3MtMS4yLTIuNi0yLjYtMi42aC0uOXY2LjRINC40VjIuNXptMy43IDYuOWgxLjRjMS45IDAgMi45LS45IDIuOS0yLjNzLTEtMi4zLTIuOC0yLjNjLS43IDAtMS4zIDAtMS42LjJ2NC41aC4xdi0uMXoiLz4KPC9zdmc+Cg==);
  --jp-icon-react: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMTUwIDE1MCA1NDEuOSAyOTUuMyI+CiAgPGcgY2xhc3M9ImpwLWljb24tYnJhbmQyIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzYxREFGQiI+CiAgICA8cGF0aCBkPSJNNjY2LjMgMjk2LjVjMC0zMi41LTQwLjctNjMuMy0xMDMuMS04Mi40IDE0LjQtNjMuNiA4LTExNC4yLTIwLjItMTMwLjQtNi41LTMuOC0xNC4xLTUuNi0yMi40LTUuNnYyMi4zYzQuNiAwIDguMy45IDExLjQgMi42IDEzLjYgNy44IDE5LjUgMzcuNSAxNC45IDc1LjctMS4xIDkuNC0yLjkgMTkuMy01LjEgMjkuNC0xOS42LTQuOC00MS04LjUtNjMuNS0xMC45LTEzLjUtMTguNS0yNy41LTM1LjMtNDEuNi01MCAzMi42LTMwLjMgNjMuMi00Ni45IDg0LTQ2LjlWNzhjLTI3LjUgMC02My41IDE5LjYtOTkuOSA1My42LTM2LjQtMzMuOC03Mi40LTUzLjItOTkuOS01My4ydjIyLjNjMjAuNyAwIDUxLjQgMTYuNSA4NCA0Ni42LTE0IDE0LjctMjggMzEuNC00MS4zIDQ5LjktMjIuNiAyLjQtNDQgNi4xLTYzLjYgMTEtMi4zLTEwLTQtMTkuNy01LjItMjktNC43LTM4LjIgMS4xLTY3LjkgMTQuNi03NS44IDMtMS44IDYuOS0yLjYgMTEuNS0yLjZWNzguNWMtOC40IDAtMTYgMS44LTIyLjYgNS42LTI4LjEgMTYuMi0zNC40IDY2LjctMTkuOSAxMzAuMS02Mi4yIDE5LjItMTAyLjcgNDkuOS0xMDIuNyA4Mi4zIDAgMzIuNSA0MC43IDYzLjMgMTAzLjEgODIuNC0xNC40IDYzLjYtOCAxMTQuMiAyMC4yIDEzMC40IDYuNSAzLjggMTQuMSA1LjYgMjIuNSA1LjYgMjcuNSAwIDYzLjUtMTkuNiA5OS45LTUzLjYgMzYuNCAzMy44IDcyLjQgNTMuMiA5OS45IDUzLjIgOC40IDAgMTYtMS44IDIyLjYtNS42IDI4LjEtMTYuMiAzNC40LTY2LjcgMTkuOS0xMzAuMSA2Mi0xOS4xIDEwMi41LTQ5LjkgMTAyLjUtODIuM3ptLTEzMC4yLTY2LjdjLTMuNyAxMi45LTguMyAyNi4yLTEzLjUgMzkuNS00LjEtOC04LjQtMTYtMTMuMS0yNC00LjYtOC05LjUtMTUuOC0xNC40LTIzLjQgMTQuMiAyLjEgMjcuOSA0LjcgNDEgNy45em0tNDUuOCAxMDYuNWMtNy44IDEzLjUtMTUuOCAyNi4zLTI0LjEgMzguMi0xNC45IDEuMy0zMCAyLTQ1LjIgMi0xNS4xIDAtMzAuMi0uNy00NS0xLjktOC4zLTExLjktMTYuNC0yNC42LTI0LjItMzgtNy42LTEzLjEtMTQuNS0yNi40LTIwLjgtMzkuOCA2LjItMTMuNCAxMy4yLTI2LjggMjAuNy0zOS45IDcuOC0xMy41IDE1LjgtMjYuMyAyNC4xLTM4LjIgMTQuOS0xLjMgMzAtMiA0NS4yLTIgMTUuMSAwIDMwLjIuNyA0NSAxLjkgOC4zIDExLjkgMTYuNCAyNC42IDI0LjIgMzggNy42IDEzLjEgMTQuNSAyNi40IDIwLjggMzkuOC02LjMgMTMuNC0xMy4yIDI2LjgtMjAuNyAzOS45em0zMi4zLTEzYzUuNCAxMy40IDEwIDI2LjggMTMuOCAzOS44LTEzLjEgMy4yLTI2LjkgNS45LTQxLjIgOCA0LjktNy43IDkuOC0xNS42IDE0LjQtMjMuNyA0LjYtOCA4LjktMTYuMSAxMy0yNC4xek00MjEuMiA0MzBjLTkuMy05LjYtMTguNi0yMC4zLTI3LjgtMzIgOSAuNCAxOC4yLjcgMjcuNS43IDkuNCAwIDE4LjctLjIgMjcuOC0uNy05IDExLjctMTguMyAyMi40LTI3LjUgMzJ6bS03NC40LTU4LjljLTE0LjItMi4xLTI3LjktNC43LTQxLTcuOSAzLjctMTIuOSA4LjMtMjYuMiAxMy41LTM5LjUgNC4xIDggOC40IDE2IDEzLjEgMjQgNC43IDggOS41IDE1LjggMTQuNCAyMy40ek00MjAuNyAxNjNjOS4zIDkuNiAxOC42IDIwLjMgMjcuOCAzMi05LS40LTE4LjItLjctMjcuNS0uNy05LjQgMC0xOC43LjItMjcuOC43IDktMTEuNyAxOC4zLTIyLjQgMjcuNS0zMnptLTc0IDU4LjljLTQuOSA3LjctOS44IDE1LjYtMTQuNCAyMy43LTQuNiA4LTguOSAxNi0xMyAyNC01LjQtMTMuNC0xMC0yNi44LTEzLjgtMzkuOCAxMy4xLTMuMSAyNi45LTUuOCA0MS4yLTcuOXptLTkwLjUgMTI1LjJjLTM1LjQtMTUuMS01OC4zLTM0LjktNTguMy01MC42IDAtMTUuNyAyMi45LTM1LjYgNTguMy01MC42IDguNi0zLjcgMTgtNyAyNy43LTEwLjEgNS43IDE5LjYgMTMuMiA0MCAyMi41IDYwLjktOS4yIDIwLjgtMTYuNiA0MS4xLTIyLjIgNjAuNi05LjktMy4xLTE5LjMtNi41LTI4LTEwLjJ6TTMxMCA0OTBjLTEzLjYtNy44LTE5LjUtMzcuNS0xNC45LTc1LjcgMS4xLTkuNCAyLjktMTkuMyA1LjEtMjkuNCAxOS42IDQuOCA0MSA4LjUgNjMuNSAxMC45IDEzLjUgMTguNSAyNy41IDM1LjMgNDEuNiA1MC0zMi42IDMwLjMtNjMuMiA0Ni45LTg0IDQ2LjktNC41LS4xLTguMy0xLTExLjMtMi43em0yMzcuMi03Ni4yYzQuNyAzOC4yLTEuMSA2Ny45LTE0LjYgNzUuOC0zIDEuOC02LjkgMi42LTExLjUgMi42LTIwLjcgMC01MS40LTE2LjUtODQtNDYuNiAxNC0xNC43IDI4LTMxLjQgNDEuMy00OS45IDIyLjYtMi40IDQ0LTYuMSA2My42LTExIDIuMyAxMC4xIDQuMSAxOS44IDUuMiAyOS4xem0zOC41LTY2LjdjLTguNiAzLjctMTggNy0yNy43IDEwLjEtNS43LTE5LjYtMTMuMi00MC0yMi41LTYwLjkgOS4yLTIwLjggMTYuNi00MS4xIDIyLjItNjAuNiA5LjkgMy4xIDE5LjMgNi41IDI4LjEgMTAuMiAzNS40IDE1LjEgNTguMyAzNC45IDU4LjMgNTAuNi0uMSAxNS43LTIzIDM1LjYtNTguNCA1MC42ek0zMjAuOCA3OC40eiIvPgogICAgPGNpcmNsZSBjeD0iNDIwLjkiIGN5PSIyOTYuNSIgcj0iNDUuNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-redo: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCBkPSJNMCAwaDI0djI0SDB6IiBmaWxsPSJub25lIi8+PHBhdGggZD0iTTE4LjQgMTAuNkMxNi41NSA4Ljk5IDE0LjE1IDggMTEuNSA4Yy00LjY1IDAtOC41OCAzLjAzLTkuOTYgNy4yMkwzLjkgMTZjMS4wNS0zLjE5IDQuMDUtNS41IDcuNi01LjUgMS45NSAwIDMuNzMuNzIgNS4xMiAxLjg4TDEzIDE2aDlWN2wtMy42IDMuNnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-refresh: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTkgMTMuNWMtMi40OSAwLTQuNS0yLjAxLTQuNS00LjVTNi41MSA0LjUgOSA0LjVjMS4yNCAwIDIuMzYuNTIgMy4xNyAxLjMzTDEwIDhoNVYzbC0xLjc2IDEuNzZDMTIuMTUgMy42OCAxMC42NiAzIDkgMyA1LjY5IDMgMy4wMSA1LjY5IDMuMDEgOVM1LjY5IDE1IDkgMTVjMi45NyAwIDUuNDMtMi4xNiA1LjktNWgtMS41MmMtLjQ2IDItMi4yNCAzLjUtNC4zOCAzLjV6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-regex: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi1hY2NlbnQyIiBmaWxsPSIjRkZGIj4KICAgIDxjaXJjbGUgY2xhc3M9InN0MiIgY3g9IjUuNSIgY3k9IjE0LjUiIHI9IjEuNSIvPgogICAgPHJlY3QgeD0iMTIiIHk9IjQiIGNsYXNzPSJzdDIiIHdpZHRoPSIxIiBoZWlnaHQ9IjgiLz4KICAgIDxyZWN0IHg9IjguNSIgeT0iNy41IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjg2NiAtMC41IDAuNSAwLjg2NiAtMi4zMjU1IDcuMzIxOSkiIGNsYXNzPSJzdDIiIHdpZHRoPSI4IiBoZWlnaHQ9IjEiLz4KICAgIDxyZWN0IHg9IjEyIiB5PSI0IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjUgLTAuODY2IDAuODY2IDAuNSAtMC42Nzc5IDE0LjgyNTIpIiBjbGFzcz0ic3QyIiB3aWR0aD0iMSIgaGVpZ2h0PSI4Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-run: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTggNXYxNGwxMS03eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-running: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMjU2IDhDMTE5IDggOCAxMTkgOCAyNTZzMTExIDI0OCAyNDggMjQ4IDI0OC0xMTEgMjQ4LTI0OFMzOTMgOCAyNTYgOHptOTYgMzI4YzAgOC44LTcuMiAxNi0xNiAxNkgxNzZjLTguOCAwLTE2LTcuMi0xNi0xNlYxNzZjMC04LjggNy4yLTE2IDE2LTE2aDE2MGM4LjggMCAxNiA3LjIgMTYgMTZ2MTYweiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-save: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE3IDNINWMtMS4xMSAwLTIgLjktMiAydjE0YzAgMS4xLjg5IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjdsLTQtNHptLTUgMTZjLTEuNjYgMC0zLTEuMzQtMy0zczEuMzQtMyAzLTMgMyAxLjM0IDMgMy0xLjM0IDMtMyAzem0zLTEwSDVWNWgxMHY0eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-search: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjEsMTAuOWgtMC43bC0wLjItMC4yYzAuOC0wLjksMS4zLTIuMiwxLjMtMy41YzAtMy0yLjQtNS40LTUuNC01LjRTMS44LDQuMiwxLjgsNy4xczIuNCw1LjQsNS40LDUuNCBjMS4zLDAsMi41LTAuNSwzLjUtMS4zbDAuMiwwLjJ2MC43bDQuMSw0LjFsMS4yLTEuMkwxMi4xLDEwLjl6IE03LjEsMTAuOWMtMi4xLDAtMy43LTEuNy0zLjctMy43czEuNy0zLjcsMy43LTMuN3MzLjcsMS43LDMuNywzLjcgUzkuMiwxMC45LDcuMSwxMC45eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-settings: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuNDMgMTIuOThjLjA0LS4zMi4wNy0uNjQuMDctLjk4cy0uMDMtLjY2LS4wNy0uOThsMi4xMS0xLjY1Yy4xOS0uMTUuMjQtLjQyLjEyLS42NGwtMi0zLjQ2Yy0uMTItLjIyLS4zOS0uMy0uNjEtLjIybC0yLjQ5IDFjLS41Mi0uNC0xLjA4LS43My0xLjY5LS45OGwtLjM4LTIuNjVBLjQ4OC40ODggMCAwMDE0IDJoLTRjLS4yNSAwLS40Ni4xOC0uNDkuNDJsLS4zOCAyLjY1Yy0uNjEuMjUtMS4xNy41OS0xLjY5Ljk4bC0yLjQ5LTFjLS4yMy0uMDktLjQ5IDAtLjYxLjIybC0yIDMuNDZjLS4xMy4yMi0uMDcuNDkuMTIuNjRsMi4xMSAxLjY1Yy0uMDQuMzItLjA3LjY1LS4wNy45OHMuMDMuNjYuMDcuOThsLTIuMTEgMS42NWMtLjE5LjE1LS4yNC40Mi0uMTIuNjRsMiAzLjQ2Yy4xMi4yMi4zOS4zLjYxLjIybDIuNDktMWMuNTIuNCAxLjA4LjczIDEuNjkuOThsLjM4IDIuNjVjLjAzLjI0LjI0LjQyLjQ5LjQyaDRjLjI1IDAgLjQ2LS4xOC40OS0uNDJsLjM4LTIuNjVjLjYxLS4yNSAxLjE3LS41OSAxLjY5LS45OGwyLjQ5IDFjLjIzLjA5LjQ5IDAgLjYxLS4yMmwyLTMuNDZjLjEyLS4yMi4wNy0uNDktLjEyLS42NGwtMi4xMS0xLjY1ek0xMiAxNS41Yy0xLjkzIDAtMy41LTEuNTctMy41LTMuNXMxLjU3LTMuNSAzLjUtMy41IDMuNSAxLjU3IDMuNSAzLjUtMS41NyAzLjUtMy41IDMuNXoiLz4KPC9zdmc+Cg==);
  --jp-icon-share: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTSAxOCAyIEMgMTYuMzU0OTkgMiAxNSAzLjM1NDk5MDQgMTUgNSBDIDE1IDUuMTkwOTUyOSAxNS4wMjE3OTEgNS4zNzcxMjI0IDE1LjA1NjY0MSA1LjU1ODU5MzggTCA3LjkyMTg3NSA5LjcyMDcwMzEgQyA3LjM5ODUzOTkgOS4yNzc4NTM5IDYuNzMyMDc3MSA5IDYgOSBDIDQuMzU0OTkwNCA5IDMgMTAuMzU0OTkgMyAxMiBDIDMgMTMuNjQ1MDEgNC4zNTQ5OTA0IDE1IDYgMTUgQyA2LjczMjA3NzEgMTUgNy4zOTg1Mzk5IDE0LjcyMjE0NiA3LjkyMTg3NSAxNC4yNzkyOTcgTCAxNS4wNTY2NDEgMTguNDM5NDUzIEMgMTUuMDIxNTU1IDE4LjYyMTUxNCAxNSAxOC44MDgzODYgMTUgMTkgQyAxNSAyMC42NDUwMSAxNi4zNTQ5OSAyMiAxOCAyMiBDIDE5LjY0NTAxIDIyIDIxIDIwLjY0NTAxIDIxIDE5IEMgMjEgMTcuMzU0OTkgMTkuNjQ1MDEgMTYgMTggMTYgQyAxNy4yNjc0OCAxNiAxNi42MDE1OTMgMTYuMjc5MzI4IDE2LjA3ODEyNSAxNi43MjI2NTYgTCA4Ljk0MzM1OTQgMTIuNTU4NTk0IEMgOC45NzgyMDk1IDEyLjM3NzEyMiA5IDEyLjE5MDk1MyA5IDEyIEMgOSAxMS44MDkwNDcgOC45NzgyMDk1IDExLjYyMjg3OCA4Ljk0MzM1OTQgMTEuNDQxNDA2IEwgMTYuMDc4MTI1IDcuMjc5Mjk2OSBDIDE2LjYwMTQ2IDcuNzIyMTQ2MSAxNy4yNjc5MjMgOCAxOCA4IEMgMTkuNjQ1MDEgOCAyMSA2LjY0NTAwOTYgMjEgNSBDIDIxIDMuMzU0OTkwNCAxOS42NDUwMSAyIDE4IDIgeiBNIDE4IDQgQyAxOC41NjQxMjkgNCAxOSA0LjQzNTg3MDYgMTkgNSBDIDE5IDUuNTY0MTI5NCAxOC41NjQxMjkgNiAxOCA2IEMgMTcuNDM1ODcxIDYgMTcgNS41NjQxMjk0IDE3IDUgQyAxNyA0LjQzNTg3MDYgMTcuNDM1ODcxIDQgMTggNCB6IE0gNiAxMSBDIDYuNTY0MTI5NCAxMSA3IDExLjQzNTg3MSA3IDEyIEMgNyAxMi41NjQxMjkgNi41NjQxMjk0IDEzIDYgMTMgQyA1LjQzNTg3MDYgMTMgNSAxMi41NjQxMjkgNSAxMiBDIDUgMTEuNDM1ODcxIDUuNDM1ODcwNiAxMSA2IDExIHogTSAxOCAxOCBDIDE4LjU2NDEyOSAxOCAxOSAxOC40MzU4NzEgMTkgMTkgQyAxOSAxOS41NjQxMjkgMTguNTY0MTI5IDIwIDE4IDIwIEMgMTcuNDM1ODcxIDIwIDE3IDE5LjU2NDEyOSAxNyAxOSBDIDE3IDE4LjQzNTg3MSAxNy40MzU4NzEgMTggMTggMTggeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-spreadsheet: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNENBRjUwIiBkPSJNMi4yIDIuMnYxNy42aDE3LjZWMi4ySDIuMnptMTUuNCA3LjdoLTUuNVY0LjRoNS41djUuNXpNOS45IDQuNHY1LjVINC40VjQuNGg1LjV6bS01LjUgNy43aDUuNXY1LjVINC40di01LjV6bTcuNyA1LjV2LTUuNWg1LjV2NS41aC01LjV6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-stop: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik02IDZoMTJ2MTJINnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tab: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIxIDNIM2MtMS4xIDAtMiAuOS0yIDJ2MTRjMCAxLjEuOSAyIDIgMmgxOGMxLjEgMCAyLS45IDItMlY1YzAtMS4xLS45LTItMi0yem0wIDE2SDNWNWgxMHY0aDh2MTB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-table-rows: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMSw4SDNWNGgxOFY4eiBNMjEsMTBIM3Y0aDE4VjEweiBNMjEsMTZIM3Y0aDE4VjE2eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-tag: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjgiIGhlaWdodD0iMjgiIHZpZXdCb3g9IjAgMCA0MyAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTI4LjgzMzIgMTIuMzM0TDMyLjk5OTggMTYuNTAwN0wzNy4xNjY1IDEyLjMzNEgyOC44MzMyWiIvPgoJCTxwYXRoIGQ9Ik0xNi4yMDk1IDIxLjYxMDRDMTUuNjg3MyAyMi4xMjk5IDE0Ljg0NDMgMjIuMTI5OSAxNC4zMjQ4IDIxLjYxMDRMNi45ODI5IDE0LjcyNDVDNi41NzI0IDE0LjMzOTQgNi4wODMxMyAxMy42MDk4IDYuMDQ3ODYgMTMuMDQ4MkM1Ljk1MzQ3IDExLjUyODggNi4wMjAwMiA4LjYxOTQ0IDYuMDY2MjEgNy4wNzY5NUM2LjA4MjgxIDYuNTE0NzcgNi41NTU0OCA2LjA0MzQ3IDcuMTE4MDQgNi4wMzA1NUM5LjA4ODYzIDUuOTg0NzMgMTMuMjYzOCA1LjkzNTc5IDEzLjY1MTggNi4zMjQyNUwyMS43MzY5IDEzLjYzOUMyMi4yNTYgMTQuMTU4NSAyMS43ODUxIDE1LjQ3MjQgMjEuMjYyIDE1Ljk5NDZMMTYuMjA5NSAyMS42MTA0Wk05Ljc3NTg1IDguMjY1QzkuMzM1NTEgNy44MjU2NiA4LjYyMzUxIDcuODI1NjYgOC4xODI4IDguMjY1QzcuNzQzNDYgOC43MDU3MSA3Ljc0MzQ2IDkuNDE3MzMgOC4xODI4IDkuODU2NjdDOC42MjM4MiAxMC4yOTY0IDkuMzM1ODIgMTAuMjk2NCA5Ljc3NTg1IDkuODU2NjdDMTAuMjE1NiA5LjQxNzMzIDEwLjIxNTYgOC43MDUzMyA5Ljc3NTg1IDguMjY1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-terminal: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0IiA+CiAgICA8cmVjdCBjbGFzcz0ianAtdGVybWluYWwtaWNvbi1iYWNrZ3JvdW5kLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZSIgd2lkdGg9IjIwIiBoZWlnaHQ9IjIwIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgyIDIpIiBmaWxsPSIjMzMzMzMzIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtdGVybWluYWwtaWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUtaW52ZXJzZSIgZD0iTTUuMDU2NjQgOC43NjE3MkM1LjA1NjY0IDguNTk3NjYgNS4wMzEyNSA4LjQ1MzEyIDQuOTgwNDcgOC4zMjgxMkM0LjkzMzU5IDguMTk5MjIgNC44NTU0NyA4LjA4MjAzIDQuNzQ2MDkgNy45NzY1NkM0LjY0MDYyIDcuODcxMDkgNC41IDcuNzc1MzkgNC4zMjQyMiA3LjY4OTQ1QzQuMTUyMzQgNy41OTk2MSAzLjk0MzM2IDcuNTExNzIgMy42OTcyNyA3LjQyNTc4QzMuMzAyNzMgNy4yODUxNiAyLjk0MzM2IDcuMTM2NzIgMi42MTkxNCA2Ljk4MDQ3QzIuMjk0OTIgNi44MjQyMiAyLjAxNzU4IDYuNjQyNTggMS43ODcxMSA2LjQzNTU1QzEuNTYwNTUgNi4yMjg1MiAxLjM4NDc3IDUuOTg4MjggMS4yNTk3NyA1LjcxNDg0QzEuMTM0NzcgNS40Mzc1IDEuMDcyMjcgNS4xMDkzOCAxLjA3MjI3IDQuNzMwNDdDMS4wNzIyNyA0LjM5ODQ0IDEuMTI4OTEgNC4wOTU3IDEuMjQyMTkgMy44MjIyN0MxLjM1NTQ3IDMuNTQ0OTIgMS41MTU2MiAzLjMwNDY5IDEuNzIyNjYgMy4xMDE1NkMxLjkyOTY5IDIuODk4NDQgMi4xNzk2OSAyLjczNDM3IDIuNDcyNjYgMi42MDkzOEMyLjc2NTYyIDIuNDg0MzggMy4wOTE4IDIuNDA0MyAzLjQ1MTE3IDIuMzY5MTRWMS4xMDkzOEg0LjM4ODY3VjIuMzgwODZDNC43NDAyMyAyLjQyNzczIDUuMDU2NjQgMi41MjM0NCA1LjMzNzg5IDIuNjY3OTdDNS42MTkxNCAyLjgxMjUgNS44NTc0MiAzLjAwMTk1IDYuMDUyNzMgMy4yMzYzM0M2LjI1MTk1IDMuNDY2OCA2LjQwNDMgMy43NDAyMyA2LjUwOTc3IDQuMDU2NjRDNi42MTkxNCA0LjM2OTE0IDYuNjczODMgNC43MjA3IDYuNjczODMgNS4xMTEzM0g1LjA0NDkyQzUuMDQ0OTIgNC42Mzg2NyA0LjkzNzUgNC4yODEyNSA0LjcyMjY2IDQuMDM5MDZDNC41MDc4MSAzLjc5Mjk3IDQuMjE2OCAzLjY2OTkyIDMuODQ5NjEgMy42Njk5MkMzLjY1MDM5IDMuNjY5OTIgMy40NzY1NiAzLjY5NzI3IDMuMzI4MTIgMy43NTE5NUMzLjE4MzU5IDMuODAyNzMgMy4wNjQ0NSAzLjg3Njk1IDIuOTcwNyAzLjk3NDYxQzIuODc2OTUgNC4wNjgzNiAyLjgwNjY0IDQuMTc5NjkgMi43NTk3NyA0LjMwODU5QzIuNzE2OCA0LjQzNzUgMi42OTUzMSA0LjU3ODEyIDIuNjk1MzEgNC43MzA0N0MyLjY5NTMxIDQuODgyODEgMi43MTY4IDUuMDE5NTMgMi43NTk3NyA1LjE0MDYyQzIuODA2NjQgNS4yNTc4MSAyLjg4MjgxIDUuMzY3MTkgMi45ODgyOCA1LjQ2ODc1QzMuMDk3NjYgNS41NzAzMSAzLjI0MDIzIDUuNjY3OTcgMy40MTYwMiA1Ljc2MTcyQzMuNTkxOCA1Ljg1MTU2IDMuODEwNTUgNS45NDMzNiA0LjA3MjI3IDYuMDM3MTFDNC40NjY4IDYuMTg1NTUgNC44MjQyMiA2LjMzOTg0IDUuMTQ0NTMgNi41QzUuNDY0ODQgNi42NTYyNSA1LjczODI4IDYuODM5ODQgNS45NjQ4NCA3LjA1MDc4QzYuMTk1MzEgNy4yNTc4MSA2LjM3MTA5IDcuNSA2LjQ5MjE5IDcuNzc3MzRDNi42MTcxOSA4LjA1MDc4IDYuNjc5NjkgOC4zNzUgNi42Nzk2OSA4Ljc1QzYuNjc5NjkgOS4wOTM3NSA2LjYyMzA1IDkuNDA0MyA2LjUwOTc3IDkuNjgxNjRDNi4zOTY0OCA5Ljk1NTA4IDYuMjM0MzggMTAuMTkxNCA2LjAyMzQ0IDEwLjM5MDZDNS44MTI1IDEwLjU4OTggNS41NTg1OSAxMC43NSA1LjI2MTcyIDEwLjg3MTFDNC45NjQ4NCAxMC45ODgzIDQuNjMyODEgMTEuMDY0NSA0LjI2NTYyIDExLjA5OTZWMTIuMjQ4SDMuMzMzOThWMTEuMDk5NkMzLjAwMTk1IDExLjA2ODQgMi42Nzk2OSAxMC45OTYxIDIuMzY3MTkgMTAuODgyOEMyLjA1NDY5IDEwLjc2NTYgMS43NzczNCAxMC41OTc3IDEuNTM1MTYgMTAuMzc4OUMxLjI5Njg4IDEwLjE2MDIgMS4xMDU0NyA5Ljg4NDc3IDAuOTYwOTM4IDkuNTUyNzNDMC44MTY0MDYgOS4yMTY4IDAuNzQ0MTQxIDguODE0NDUgMC43NDQxNDEgOC4zNDU3SDIuMzc4OTFDMi4zNzg5MSA4LjYyNjk1IDIuNDE5OTIgOC44NjMyOCAyLjUwMTk1IDkuMDU0NjlDMi41ODM5OCA5LjI0MjE5IDIuNjg5NDUgOS4zOTI1OCAyLjgxODM2IDkuNTA1ODZDMi45NTExNyA5LjYxNTIzIDMuMTAxNTYgOS42OTMzNiAzLjI2OTUzIDkuNzQwMjNDMy40Mzc1IDkuNzg3MTEgMy42MDkzOCA5LjgxMDU1IDMuNzg1MTYgOS44MTA1NUM0LjIwMzEyIDkuODEwNTUgNC41MTk1MyA5LjcxMjg5IDQuNzM0MzggOS41MTc1OEM0Ljk0OTIyIDkuMzIyMjcgNS4wNTY2NCA5LjA3MDMxIDUuMDU2NjQgOC43NjE3MlpNMTMuNDE4IDEyLjI3MTVIOC4wNzQyMlYxMUgxMy40MThWMTIuMjcxNVoiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMuOTUyNjQgNikiIGZpbGw9IndoaXRlIi8+Cjwvc3ZnPgo=);
  --jp-icon-text-editor: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtdGV4dC1lZGl0b3ItaWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xNSAxNUgzdjJoMTJ2LTJ6bTAtOEgzdjJoMTJWN3pNMyAxM2gxOHYtMkgzdjJ6bTAgOGgxOHYtMkgzdjJ6TTMgM3YyaDE4VjNIM3oiLz4KPC9zdmc+Cg==);
  --jp-icon-toc: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik03LDVIMjFWN0g3VjVNNywxM1YxMUgyMVYxM0g3TTQsNC41QTEuNSwxLjUgMCAwLDEgNS41LDZBMS41LDEuNSAwIDAsMSA0LDcuNUExLjUsMS41IDAgMCwxIDIuNSw2QTEuNSwxLjUgMCAwLDEgNCw0LjVNNCwxMC41QTEuNSwxLjUgMCAwLDEgNS41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMy41QTEuNSwxLjUgMCAwLDEgMi41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMC41TTcsMTlWMTdIMjFWMTlIN000LDE2LjVBMS41LDEuNSAwIDAsMSA1LjUsMThBMS41LDEuNSAwIDAsMSA0LDE5LjVBMS41LDEuNSAwIDAsMSAyLjUsMThBMS41LDEuNSAwIDAsMSA0LDE2LjVaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tree-view: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMiAxMVYzaC03djNIOVYzSDJ2OGg3VjhoMnYxMGg0djNoN3YtOGgtN3YzaC0yVjhoMnYzeiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMiAxNy4xODQ0IDIuOTY5NjggMTQuMzAzMiAxLjg2MDk0IDExLjQ0MDlaIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiMzMzMzMzMiIHN0cm9rZT0iIzMzMzMzMyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOCA5Ljg2NzE5KSIgZD0iTTIuODYwMTUgNC44NjUzNUwwLjcyNjU0OSAyLjk5OTU5TDAgMy42MzA0NUwyLjg2MDE1IDYuMTMxNTdMOCAwLjYzMDg3Mkw3LjI3ODU3IDBMMi44NjAxNSA0Ljg2NTM1WiIvPgo8L3N2Zz4K);
  --jp-icon-undo: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjUgOGMtMi42NSAwLTUuMDUuOTktNi45IDIuNkwyIDd2OWg5bC0zLjYyLTMuNjJjMS4zOS0xLjE2IDMuMTYtMS44OCA1LjEyLTEuODggMy41NCAwIDYuNTUgMi4zMSA3LjYgNS41bDIuMzctLjc4QzIxLjA4IDExLjAzIDE3LjE1IDggMTIuNSA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-user: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE2IDdhNCA0IDAgMTEtOCAwIDQgNCAwIDAxOCAwek0xMiAxNGE3IDcgMCAwMC03IDdoMTRhNyA3IDAgMDAtNy03eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-users: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZlcnNpb249IjEuMSIgdmlld0JveD0iMCAwIDM2IDI0IiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogPGcgY2xhc3M9ImpwLWljb24zIiB0cmFuc2Zvcm09Im1hdHJpeCgxLjczMjcgMCAwIDEuNzMyNyAtMy42MjgyIC4wOTk1NzcpIiBmaWxsPSIjNjE2MTYxIj4KICA8cGF0aCB0cmFuc2Zvcm09Im1hdHJpeCgxLjUsMCwwLDEuNSwwLC02KSIgZD0ibTEyLjE4NiA3LjUwOThjLTEuMDUzNSAwLTEuOTc1NyAwLjU2NjUtMi40Nzg1IDEuNDEwMiAwLjc1MDYxIDAuMzEyNzcgMS4zOTc0IDAuODI2NDggMS44NzMgMS40NzI3aDMuNDg2M2MwLTEuNTkyLTEuMjg4OS0yLjg4MjgtMi44ODA5LTIuODgyOHoiLz4KICA8cGF0aCBkPSJtMjAuNDY1IDIuMzg5NWEyLjE4ODUgMi4xODg1IDAgMCAxLTIuMTg4NCAyLjE4ODUgMi4xODg1IDIuMTg4NSAwIDAgMS0yLjE4ODUtMi4xODg1IDIuMTg4NSAyLjE4ODUgMCAwIDEgMi4xODg1LTIuMTg4NSAyLjE4ODUgMi4xODg1IDAgMCAxIDIuMTg4NCAyLjE4ODV6Ii8+CiAgPHBhdGggdHJhbnNmb3JtPSJtYXRyaXgoMS41LDAsMCwxLjUsMCwtNikiIGQ9Im0zLjU4OTggOC40MjE5Yy0xLjExMjYgMC0yLjAxMzcgMC45MDExMS0yLjAxMzcgMi4wMTM3aDIuODE0NWMwLjI2Nzk3LTAuMzczMDkgMC41OTA3LTAuNzA0MzUgMC45NTg5OC0wLjk3ODUyLTAuMzQ0MzMtMC42MTY4OC0xLjAwMzEtMS4wMzUyLTEuNzU5OC0xLjAzNTJ6Ii8+CiAgPHBhdGggZD0ibTYuOTE1NCA0LjYyM2ExLjUyOTQgMS41Mjk0IDAgMCAxLTEuNTI5NCAxLjUyOTQgMS41Mjk0IDEuNTI5NCAwIDAgMS0xLjUyOTQtMS41Mjk0IDEuNTI5NCAxLjUyOTQgMCAwIDEgMS41Mjk0LTEuNTI5NCAxLjUyOTQgMS41Mjk0IDAgMCAxIDEuNTI5NCAxLjUyOTR6Ii8+CiAgPHBhdGggZD0ibTYuMTM1IDEzLjUzNWMwLTMuMjM5MiAyLjYyNTktNS44NjUgNS44NjUtNS44NjUgMy4yMzkyIDAgNS44NjUgMi42MjU5IDUuODY1IDUuODY1eiIvPgogIDxjaXJjbGUgY3g9IjEyIiBjeT0iMy43Njg1IiByPSIyLjk2ODUiLz4KIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-vega: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbjEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjEyMTIxIj4KICAgIDxwYXRoIGQ9Ik0xMC42IDUuNGwyLjItMy4ySDIuMnY3LjNsNC02LjZ6Ii8+CiAgICA8cGF0aCBkPSJNMTUuOCAyLjJsLTQuNCA2LjZMNyA2LjNsLTQuOCA4djUuNWgxNy42VjIuMmgtNHptLTcgMTUuNEg1LjV2LTQuNGgzLjN2NC40em00LjQgMEg5LjhWOS44aDMuNHY3Ljh6bTQuNCAwaC0zLjRWNi41aDMuNHYxMS4xeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-word: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KIDxnIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzQxNDE0MSI+CiAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiA8L2c+CiA8ZyBjbGFzcz0ianAtaWNvbi1hY2NlbnQyIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSguNDMgLjA0MDEpIiBmaWxsPSIjZmZmIj4KICA8cGF0aCBkPSJtNC4xNCA4Ljc2cTAuMDY4Mi0xLjg5IDIuNDItMS44OSAxLjE2IDAgMS42OCAwLjQyIDAuNTY3IDAuNDEgMC41NjcgMS4xNnYzLjQ3cTAgMC40NjIgMC41MTQgMC40NjIgMC4xMDMgMCAwLjItMC4wMjMxdjAuNzE0cS0wLjM5OSAwLjEwMy0wLjY1MSAwLjEwMy0wLjQ1MiAwLTAuNjkzLTAuMjItMC4yMzEtMC4yLTAuMjg0LTAuNjYyLTAuOTU2IDAuODcyLTIgMC44NzItMC45MDMgMC0xLjQ3LTAuNDcyLTAuNTI1LTAuNDcyLTAuNTI1LTEuMjYgMC0wLjI2MiAwLjA0NTItMC40NzIgMC4wNTY3LTAuMjIgMC4xMTYtMC4zNzggMC4wNjgyLTAuMTY4IDAuMjMxLTAuMzA0IDAuMTU4LTAuMTQ3IDAuMjYyLTAuMjQyIDAuMTE2LTAuMDkxNCAwLjM2OC0wLjE2OCAwLjI2Mi0wLjA5MTQgMC4zOTktMC4xMjYgMC4xMzYtMC4wNDUyIDAuNDcyLTAuMTAzIDAuMzM2LTAuMDU3OCAwLjUwNC0wLjA3OTggMC4xNTgtMC4wMjMxIDAuNTY3LTAuMDc5OCAwLjU1Ni0wLjA2ODIgMC43NzctMC4yMjEgMC4yMi0wLjE1MiAwLjIyLTAuNDQxdi0wLjI1MnEwLTAuNDMtMC4zNTctMC42NjItMC4zMzYtMC4yMzEtMC45NzYtMC4yMzEtMC42NjIgMC0wLjk5OCAwLjI2Mi0wLjMzNiAwLjI1Mi0wLjM5OSAwLjc5OHptMS44OSAzLjY4cTAuNzg4IDAgMS4yNi0wLjQxIDAuNTA0LTAuNDIgMC41MDQtMC45MDN2LTEuMDVxLTAuMjg0IDAuMTM2LTAuODYxIDAuMjMxLTAuNTY3IDAuMDkxNC0wLjk4NyAwLjE1OC0wLjQyIDAuMDY4Mi0wLjc2NiAwLjMyNi0wLjMzNiAwLjI1Mi0wLjMzNiAwLjcwNHQwLjMwNCAwLjcwNCAwLjg2MSAwLjI1MnoiIHN0cm9rZS13aWR0aD0iMS4wNSIvPgogIDxwYXRoIGQ9Im0xMCA0LjU2aDAuOTQ1djMuMTVxMC42NTEtMC45NzYgMS44OS0wLjk3NiAxLjE2IDAgMS44OSAwLjg0IDAuNjgyIDAuODQgMC42ODIgMi4zMSAwIDEuNDctMC43MDQgMi40Mi0wLjcwNCAwLjg4Mi0xLjg5IDAuODgyLTEuMjYgMC0xLjg5LTEuMDJ2MC43NjZoLTAuODV6bTIuNjIgMy4wNHEtMC43NDYgMC0xLjE2IDAuNjQtMC40NTIgMC42My0wLjQ1MiAxLjY4IDAgMS4wNSAwLjQ1MiAxLjY4dDEuMTYgMC42M3EwLjc3NyAwIDEuMjYtMC42MyAwLjQ5NC0wLjY0IDAuNDk0LTEuNjggMC0xLjA1LTAuNDcyLTEuNjgtMC40NjItMC42NC0xLjI2LTAuNjR6IiBzdHJva2Utd2lkdGg9IjEuMDUiLz4KICA8cGF0aCBkPSJtMi43MyAxNS44IDEzLjYgMC4wMDgxYzAuMDA2OSAwIDAtMi42IDAtMi42IDAtMC4wMDc4LTEuMTUgMC0xLjE1IDAtMC4wMDY5IDAtMC4wMDgzIDEuNS0wLjAwODMgMS41LTJlLTMgLTAuMDAxNC0xMS4zLTAuMDAxNC0xMS4zLTAuMDAxNGwtMC4wMDU5Mi0xLjVjMC0wLjAwNzgtMS4xNyAwLjAwMTMtMS4xNyAwLjAwMTN6IiBzdHJva2Utd2lkdGg9Ii45NzUiLz4KIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-yaml: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1jb250cmFzdDIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjRDgxQjYwIj4KICAgIDxwYXRoIGQ9Ik03LjIgMTguNnYtNS40TDMgNS42aDMuM2wxLjQgMy4xYy4zLjkuNiAxLjYgMSAyLjUuMy0uOC42LTEuNiAxLTIuNWwxLjQtMy4xaDMuNGwtNC40IDcuNnY1LjVsLTIuOS0uMXoiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxNi41IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxMSIgcj0iMi4xIi8+CiAgPC9nPgo8L3N2Zz4K);
}

/* Icon CSS class declarations */

.jp-AddAboveIcon {
  background-image: var(--jp-icon-add-above);
}

.jp-AddBelowIcon {
  background-image: var(--jp-icon-add-below);
}

.jp-AddIcon {
  background-image: var(--jp-icon-add);
}

.jp-BellIcon {
  background-image: var(--jp-icon-bell);
}

.jp-BugDotIcon {
  background-image: var(--jp-icon-bug-dot);
}

.jp-BugIcon {
  background-image: var(--jp-icon-bug);
}

.jp-BuildIcon {
  background-image: var(--jp-icon-build);
}

.jp-CaretDownEmptyIcon {
  background-image: var(--jp-icon-caret-down-empty);
}

.jp-CaretDownEmptyThinIcon {
  background-image: var(--jp-icon-caret-down-empty-thin);
}

.jp-CaretDownIcon {
  background-image: var(--jp-icon-caret-down);
}

.jp-CaretLeftIcon {
  background-image: var(--jp-icon-caret-left);
}

.jp-CaretRightIcon {
  background-image: var(--jp-icon-caret-right);
}

.jp-CaretUpEmptyThinIcon {
  background-image: var(--jp-icon-caret-up-empty-thin);
}

.jp-CaretUpIcon {
  background-image: var(--jp-icon-caret-up);
}

.jp-CaseSensitiveIcon {
  background-image: var(--jp-icon-case-sensitive);
}

.jp-CheckIcon {
  background-image: var(--jp-icon-check);
}

.jp-CircleEmptyIcon {
  background-image: var(--jp-icon-circle-empty);
}

.jp-CircleIcon {
  background-image: var(--jp-icon-circle);
}

.jp-ClearIcon {
  background-image: var(--jp-icon-clear);
}

.jp-CloseIcon {
  background-image: var(--jp-icon-close);
}

.jp-CodeCheckIcon {
  background-image: var(--jp-icon-code-check);
}

.jp-CodeIcon {
  background-image: var(--jp-icon-code);
}

.jp-CollapseAllIcon {
  background-image: var(--jp-icon-collapse-all);
}

.jp-ConsoleIcon {
  background-image: var(--jp-icon-console);
}

.jp-CopyIcon {
  background-image: var(--jp-icon-copy);
}

.jp-CopyrightIcon {
  background-image: var(--jp-icon-copyright);
}

.jp-CutIcon {
  background-image: var(--jp-icon-cut);
}

.jp-DeleteIcon {
  background-image: var(--jp-icon-delete);
}

.jp-DownloadIcon {
  background-image: var(--jp-icon-download);
}

.jp-DuplicateIcon {
  background-image: var(--jp-icon-duplicate);
}

.jp-EditIcon {
  background-image: var(--jp-icon-edit);
}

.jp-EllipsesIcon {
  background-image: var(--jp-icon-ellipses);
}

.jp-ErrorIcon {
  background-image: var(--jp-icon-error);
}

.jp-ExpandAllIcon {
  background-image: var(--jp-icon-expand-all);
}

.jp-ExtensionIcon {
  background-image: var(--jp-icon-extension);
}

.jp-FastForwardIcon {
  background-image: var(--jp-icon-fast-forward);
}

.jp-FileIcon {
  background-image: var(--jp-icon-file);
}

.jp-FileUploadIcon {
  background-image: var(--jp-icon-file-upload);
}

.jp-FilterDotIcon {
  background-image: var(--jp-icon-filter-dot);
}

.jp-FilterIcon {
  background-image: var(--jp-icon-filter);
}

.jp-FilterListIcon {
  background-image: var(--jp-icon-filter-list);
}

.jp-FolderFavoriteIcon {
  background-image: var(--jp-icon-folder-favorite);
}

.jp-FolderIcon {
  background-image: var(--jp-icon-folder);
}

.jp-HomeIcon {
  background-image: var(--jp-icon-home);
}

.jp-Html5Icon {
  background-image: var(--jp-icon-html5);
}

.jp-ImageIcon {
  background-image: var(--jp-icon-image);
}

.jp-InfoIcon {
  background-image: var(--jp-icon-info);
}

.jp-InspectorIcon {
  background-image: var(--jp-icon-inspector);
}

.jp-JsonIcon {
  background-image: var(--jp-icon-json);
}

.jp-JuliaIcon {
  background-image: var(--jp-icon-julia);
}

.jp-JupyterFaviconIcon {
  background-image: var(--jp-icon-jupyter-favicon);
}

.jp-JupyterIcon {
  background-image: var(--jp-icon-jupyter);
}

.jp-JupyterlabWordmarkIcon {
  background-image: var(--jp-icon-jupyterlab-wordmark);
}

.jp-KernelIcon {
  background-image: var(--jp-icon-kernel);
}

.jp-KeyboardIcon {
  background-image: var(--jp-icon-keyboard);
}

.jp-LaunchIcon {
  background-image: var(--jp-icon-launch);
}

.jp-LauncherIcon {
  background-image: var(--jp-icon-launcher);
}

.jp-LineFormIcon {
  background-image: var(--jp-icon-line-form);
}

.jp-LinkIcon {
  background-image: var(--jp-icon-link);
}

.jp-ListIcon {
  background-image: var(--jp-icon-list);
}

.jp-MarkdownIcon {
  background-image: var(--jp-icon-markdown);
}

.jp-MoveDownIcon {
  background-image: var(--jp-icon-move-down);
}

.jp-MoveUpIcon {
  background-image: var(--jp-icon-move-up);
}

.jp-NewFolderIcon {
  background-image: var(--jp-icon-new-folder);
}

.jp-NotTrustedIcon {
  background-image: var(--jp-icon-not-trusted);
}

.jp-NotebookIcon {
  background-image: var(--jp-icon-notebook);
}

.jp-NumberingIcon {
  background-image: var(--jp-icon-numbering);
}

.jp-OfflineBoltIcon {
  background-image: var(--jp-icon-offline-bolt);
}

.jp-PaletteIcon {
  background-image: var(--jp-icon-palette);
}

.jp-PasteIcon {
  background-image: var(--jp-icon-paste);
}

.jp-PdfIcon {
  background-image: var(--jp-icon-pdf);
}

.jp-PythonIcon {
  background-image: var(--jp-icon-python);
}

.jp-RKernelIcon {
  background-image: var(--jp-icon-r-kernel);
}

.jp-ReactIcon {
  background-image: var(--jp-icon-react);
}

.jp-RedoIcon {
  background-image: var(--jp-icon-redo);
}

.jp-RefreshIcon {
  background-image: var(--jp-icon-refresh);
}

.jp-RegexIcon {
  background-image: var(--jp-icon-regex);
}

.jp-RunIcon {
  background-image: var(--jp-icon-run);
}

.jp-RunningIcon {
  background-image: var(--jp-icon-running);
}

.jp-SaveIcon {
  background-image: var(--jp-icon-save);
}

.jp-SearchIcon {
  background-image: var(--jp-icon-search);
}

.jp-SettingsIcon {
  background-image: var(--jp-icon-settings);
}

.jp-ShareIcon {
  background-image: var(--jp-icon-share);
}

.jp-SpreadsheetIcon {
  background-image: var(--jp-icon-spreadsheet);
}

.jp-StopIcon {
  background-image: var(--jp-icon-stop);
}

.jp-TabIcon {
  background-image: var(--jp-icon-tab);
}

.jp-TableRowsIcon {
  background-image: var(--jp-icon-table-rows);
}

.jp-TagIcon {
  background-image: var(--jp-icon-tag);
}

.jp-TerminalIcon {
  background-image: var(--jp-icon-terminal);
}

.jp-TextEditorIcon {
  background-image: var(--jp-icon-text-editor);
}

.jp-TocIcon {
  background-image: var(--jp-icon-toc);
}

.jp-TreeViewIcon {
  background-image: var(--jp-icon-tree-view);
}

.jp-TrustedIcon {
  background-image: var(--jp-icon-trusted);
}

.jp-UndoIcon {
  background-image: var(--jp-icon-undo);
}

.jp-UserIcon {
  background-image: var(--jp-icon-user);
}

.jp-UsersIcon {
  background-image: var(--jp-icon-users);
}

.jp-VegaIcon {
  background-image: var(--jp-icon-vega);
}

.jp-WordIcon {
  background-image: var(--jp-icon-word);
}

.jp-YamlIcon {
  background-image: var(--jp-icon-yaml);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * (DEPRECATED) Support for consuming icons as CSS background images
 */

.jp-Icon,
.jp-MaterialIcon {
  background-position: center;
  background-repeat: no-repeat;
  background-size: 16px;
  min-width: 16px;
  min-height: 16px;
}

.jp-Icon-cover {
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

/**
 * (DEPRECATED) Support for specific CSS icon sizes
 */

.jp-Icon-16 {
  background-size: 16px;
  min-width: 16px;
  min-height: 16px;
}

.jp-Icon-18 {
  background-size: 18px;
  min-width: 18px;
  min-height: 18px;
}

.jp-Icon-20 {
  background-size: 20px;
  min-width: 20px;
  min-height: 20px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.lm-TabBar .lm-TabBar-addButton {
  align-items: center;
  display: flex;
  padding: 4px;
  padding-bottom: 5px;
  margin-right: 1px;
  background-color: var(--jp-layout-color2);
}

.lm-TabBar .lm-TabBar-addButton:hover {
  background-color: var(--jp-layout-color1);
}

.lm-DockPanel-tabBar .lm-TabBar-tab {
  width: var(--jp-private-horizontal-tab-width);
}

.lm-DockPanel-tabBar .lm-TabBar-content {
  flex: unset;
}

.lm-DockPanel-tabBar[data-orientation='horizontal'] {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * Support for icons as inline SVG HTMLElements
 */

/* recolor the primary elements of an icon */
.jp-icon0[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon1[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon2[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon3[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon4[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon0[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon1[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon2[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon3[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon4[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/* recolor the accent elements of an icon */
.jp-icon-accent0[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-accent1[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-accent2[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-accent3[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-accent4[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-accent0[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-accent1[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-accent2[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-accent3[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-accent4[stroke] {
  stroke: var(--jp-layout-color4);
}

/* set the color of an icon to transparent */
.jp-icon-none[fill] {
  fill: none;
}

.jp-icon-none[stroke] {
  stroke: none;
}

/* brand icon colors. Same for light and dark */
.jp-icon-brand0[fill] {
  fill: var(--jp-brand-color0);
}

.jp-icon-brand1[fill] {
  fill: var(--jp-brand-color1);
}

.jp-icon-brand2[fill] {
  fill: var(--jp-brand-color2);
}

.jp-icon-brand3[fill] {
  fill: var(--jp-brand-color3);
}

.jp-icon-brand4[fill] {
  fill: var(--jp-brand-color4);
}

.jp-icon-brand0[stroke] {
  stroke: var(--jp-brand-color0);
}

.jp-icon-brand1[stroke] {
  stroke: var(--jp-brand-color1);
}

.jp-icon-brand2[stroke] {
  stroke: var(--jp-brand-color2);
}

.jp-icon-brand3[stroke] {
  stroke: var(--jp-brand-color3);
}

.jp-icon-brand4[stroke] {
  stroke: var(--jp-brand-color4);
}

/* warn icon colors. Same for light and dark */
.jp-icon-warn0[fill] {
  fill: var(--jp-warn-color0);
}

.jp-icon-warn1[fill] {
  fill: var(--jp-warn-color1);
}

.jp-icon-warn2[fill] {
  fill: var(--jp-warn-color2);
}

.jp-icon-warn3[fill] {
  fill: var(--jp-warn-color3);
}

.jp-icon-warn0[stroke] {
  stroke: var(--jp-warn-color0);
}

.jp-icon-warn1[stroke] {
  stroke: var(--jp-warn-color1);
}

.jp-icon-warn2[stroke] {
  stroke: var(--jp-warn-color2);
}

.jp-icon-warn3[stroke] {
  stroke: var(--jp-warn-color3);
}

/* icon colors that contrast well with each other and most backgrounds */
.jp-icon-contrast0[fill] {
  fill: var(--jp-icon-contrast-color0);
}

.jp-icon-contrast1[fill] {
  fill: var(--jp-icon-contrast-color1);
}

.jp-icon-contrast2[fill] {
  fill: var(--jp-icon-contrast-color2);
}

.jp-icon-contrast3[fill] {
  fill: var(--jp-icon-contrast-color3);
}

.jp-icon-contrast0[stroke] {
  stroke: var(--jp-icon-contrast-color0);
}

.jp-icon-contrast1[stroke] {
  stroke: var(--jp-icon-contrast-color1);
}

.jp-icon-contrast2[stroke] {
  stroke: var(--jp-icon-contrast-color2);
}

.jp-icon-contrast3[stroke] {
  stroke: var(--jp-icon-contrast-color3);
}

.jp-icon-dot[fill] {
  fill: var(--jp-warn-color0);
}

.jp-jupyter-icon-color[fill] {
  fill: var(--jp-jupyter-icon-color, var(--jp-warn-color0));
}

.jp-notebook-icon-color[fill] {
  fill: var(--jp-notebook-icon-color, var(--jp-warn-color0));
}

.jp-json-icon-color[fill] {
  fill: var(--jp-json-icon-color, var(--jp-warn-color1));
}

.jp-console-icon-color[fill] {
  fill: var(--jp-console-icon-color, white);
}

.jp-console-icon-background-color[fill] {
  fill: var(--jp-console-icon-background-color, var(--jp-brand-color1));
}

.jp-terminal-icon-color[fill] {
  fill: var(--jp-terminal-icon-color, var(--jp-layout-color2));
}

.jp-terminal-icon-background-color[fill] {
  fill: var(
    --jp-terminal-icon-background-color,
    var(--jp-inverse-layout-color2)
  );
}

.jp-text-editor-icon-color[fill] {
  fill: var(--jp-text-editor-icon-color, var(--jp-inverse-layout-color3));
}

.jp-inspector-icon-color[fill] {
  fill: var(--jp-inspector-icon-color, var(--jp-inverse-layout-color3));
}

/* CSS for icons in selected filebrowser listing items */
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}

.jp-DirListing-item.jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* stylelint-disable selector-max-class, selector-max-compound-selectors */

/**
* TODO: come up with non css-hack solution for showing the busy icon on top
*  of the close icon
* CSS for complex behavior of close icon of tabs in the main area tabbar
*/
.lm-DockPanel-tabBar
  .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon3[fill] {
  fill: none;
}

.lm-DockPanel-tabBar
  .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon-busy[fill] {
  fill: var(--jp-inverse-layout-color3);
}

/* stylelint-enable selector-max-class, selector-max-compound-selectors */

/* CSS for icons in status bar */
#jp-main-statusbar .jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}

#jp-main-statusbar .jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* special handling for splash icon CSS. While the theme CSS reloads during
   splash, the splash icon can loose theming. To prevent that, we set a
   default for its color variable */
:root {
  --jp-warn-color0: var(--md-orange-700);
}

/* not sure what to do with this one, used in filebrowser listing */
.jp-DragIcon {
  margin-right: 4px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * Support for alt colors for icons as inline SVG HTMLElements
 */

/* alt recolor the primary elements of an icon */
.jp-icon-alt .jp-icon0[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-alt .jp-icon1[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-alt .jp-icon2[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-alt .jp-icon3[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-alt .jp-icon4[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-alt .jp-icon0[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-alt .jp-icon1[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-alt .jp-icon2[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-alt .jp-icon3[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-alt .jp-icon4[stroke] {
  stroke: var(--jp-layout-color4);
}

/* alt recolor the accent elements of an icon */
.jp-icon-alt .jp-icon-accent0[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon-alt .jp-icon-accent1[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon-alt .jp-icon-accent2[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon-alt .jp-icon-accent3[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon-alt .jp-icon-accent4[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-alt .jp-icon-accent0[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon-alt .jp-icon-accent1[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon-alt .jp-icon-accent2[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon-alt .jp-icon-accent3[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon-alt .jp-icon-accent4[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-icon-hoverShow:not(:hover) .jp-icon-hoverShow-content {
  display: none !important;
}

/**
 * Support for hover colors for icons as inline SVG HTMLElements
 */

/**
 * regular colors
 */

/* recolor the primary elements of an icon */
.jp-icon-hover :hover .jp-icon0-hover[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon-hover :hover .jp-icon1-hover[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon-hover :hover .jp-icon2-hover[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon-hover :hover .jp-icon3-hover[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon-hover :hover .jp-icon4-hover[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover :hover .jp-icon0-hover[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon-hover :hover .jp-icon1-hover[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon-hover :hover .jp-icon2-hover[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon-hover :hover .jp-icon3-hover[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon-hover :hover .jp-icon4-hover[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/* recolor the accent elements of an icon */
.jp-icon-hover :hover .jp-icon-accent0-hover[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-hover :hover .jp-icon-accent1-hover[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-hover :hover .jp-icon-accent2-hover[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-hover :hover .jp-icon-accent3-hover[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-hover :hover .jp-icon-accent4-hover[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-hover :hover .jp-icon-accent0-hover[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-hover :hover .jp-icon-accent1-hover[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-hover :hover .jp-icon-accent2-hover[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-hover :hover .jp-icon-accent3-hover[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-hover :hover .jp-icon-accent4-hover[stroke] {
  stroke: var(--jp-layout-color4);
}

/* set the color of an icon to transparent */
.jp-icon-hover :hover .jp-icon-none-hover[fill] {
  fill: none;
}

.jp-icon-hover :hover .jp-icon-none-hover[stroke] {
  stroke: none;
}

/**
 * inverse colors
 */

/* inverse recolor the primary elements of an icon */
.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[fill] {
  fill: var(--jp-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[fill] {
  fill: var(--jp-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[fill] {
  fill: var(--jp-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[fill] {
  fill: var(--jp-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[stroke] {
  stroke: var(--jp-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[stroke] {
  stroke: var(--jp-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[stroke] {
  stroke: var(--jp-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[stroke] {
  stroke: var(--jp-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[stroke] {
  stroke: var(--jp-layout-color4);
}

/* inverse recolor the accent elements of an icon */
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[fill] {
  fill: var(--jp-inverse-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[fill] {
  fill: var(--jp-inverse-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[fill] {
  fill: var(--jp-inverse-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[fill] {
  fill: var(--jp-inverse-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-IFrame {
  width: 100%;
  height: 100%;
}

.jp-IFrame > iframe {
  border: none;
}

/*
When drag events occur, `lm-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-IFrame {
  position: relative;
}

body.lm-mod-override-cursor .jp-IFrame::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-HoverBox {
  position: fixed;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-FormGroup-content fieldset {
  border: none;
  padding: 0;
  min-width: 0;
  width: 100%;
}

/* stylelint-disable selector-max-type */

.jp-FormGroup-content fieldset .jp-inputFieldWrapper input,
.jp-FormGroup-content fieldset .jp-inputFieldWrapper select,
.jp-FormGroup-content fieldset .jp-inputFieldWrapper textarea {
  font-size: var(--jp-content-font-size2);
  border-color: var(--jp-input-border-color);
  border-style: solid;
  border-radius: var(--jp-border-radius);
  border-width: 1px;
  padding: 6px 8px;
  background: none;
  color: var(--jp-ui-font-color0);
  height: inherit;
}

.jp-FormGroup-content fieldset input[type='checkbox'] {
  position: relative;
  top: 2px;
  margin-left: 0;
}

.jp-FormGroup-content button.jp-mod-styled {
  cursor: pointer;
}

.jp-FormGroup-content .checkbox label {
  cursor: pointer;
  font-size: var(--jp-content-font-size1);
}

.jp-FormGroup-content .jp-root > fieldset > legend {
  display: none;
}

.jp-FormGroup-content .jp-root > fieldset > p {
  display: none;
}

/** copy of `input.jp-mod-styled:focus` style */
.jp-FormGroup-content fieldset input:focus,
.jp-FormGroup-content fieldset select:focus {
  -moz-outline-radius: unset;
  outline: var(--jp-border-width) solid var(--md-blue-500);
  outline-offset: -1px;
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-FormGroup-content fieldset input:hover:not(:focus),
.jp-FormGroup-content fieldset select:hover:not(:focus) {
  background-color: var(--jp-border-color2);
}

/* stylelint-enable selector-max-type */

.jp-FormGroup-content .checkbox .field-description {
  /* Disable default description field for checkbox:
   because other widgets do not have description fields,
   we add descriptions to each widget on the field level.
  */
  display: none;
}

.jp-FormGroup-content #root__description {
  display: none;
}

.jp-FormGroup-content .jp-modifiedIndicator {
  width: 5px;
  background-color: var(--jp-brand-color2);
  margin-top: 0;
  margin-left: calc(var(--jp-private-settingeditor-modifier-indent) * -1);
  flex-shrink: 0;
}

.jp-FormGroup-content .jp-modifiedIndicator.jp-errorIndicator {
  background-color: var(--jp-error-color0);
  margin-right: 0.5em;
}

/* RJSF ARRAY style */

.jp-arrayFieldWrapper legend {
  font-size: var(--jp-content-font-size2);
  color: var(--jp-ui-font-color0);
  flex-basis: 100%;
  padding: 4px 0;
  font-weight: var(--jp-content-heading-font-weight);
  border-bottom: 1px solid var(--jp-border-color2);
}

.jp-arrayFieldWrapper .field-description {
  padding: 4px 0;
  white-space: pre-wrap;
}

.jp-arrayFieldWrapper .array-item {
  width: 100%;
  border: 1px solid var(--jp-border-color2);
  border-radius: 4px;
  margin: 4px;
}

.jp-ArrayOperations {
  display: flex;
  margin-left: 8px;
}

.jp-ArrayOperationsButton {
  margin: 2px;
}

.jp-ArrayOperationsButton .jp-icon3[fill] {
  fill: var(--jp-ui-font-color0);
}

button.jp-ArrayOperationsButton.jp-mod-styled:disabled {
  cursor: not-allowed;
  opacity: 0.5;
}

/* RJSF form validation error */

.jp-FormGroup-content .validationErrors {
  color: var(--jp-error-color0);
}

/* Hide panel level error as duplicated the field level error */
.jp-FormGroup-content .panel.errors {
  display: none;
}

/* RJSF normal content (settings-editor) */

.jp-FormGroup-contentNormal {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.jp-FormGroup-contentNormal .jp-FormGroup-contentItem {
  margin-left: 7px;
  color: var(--jp-ui-font-color0);
}

.jp-FormGroup-contentNormal .jp-FormGroup-description {
  flex-basis: 100%;
  padding: 4px 7px;
}

.jp-FormGroup-contentNormal .jp-FormGroup-default {
  flex-basis: 100%;
  padding: 4px 7px;
}

.jp-FormGroup-contentNormal .jp-FormGroup-fieldLabel {
  font-size: var(--jp-content-font-size1);
  font-weight: normal;
  min-width: 120px;
}

.jp-FormGroup-contentNormal fieldset:not(:first-child) {
  margin-left: 7px;
}

.jp-FormGroup-contentNormal .field-array-of-string .array-item {
  /* Display `jp-ArrayOperations` buttons side-by-side with content except
    for small screens where flex-wrap will place them one below the other.
  */
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.jp-FormGroup-contentNormal .jp-objectFieldWrapper .form-group {
  padding: 2px 8px 2px var(--jp-private-settingeditor-modifier-indent);
  margin-top: 2px;
}

/* RJSF compact content (metadata-form) */

.jp-FormGroup-content.jp-FormGroup-contentCompact {
  width: 100%;
}

.jp-FormGroup-contentCompact .form-group {
  display: flex;
  padding: 0.5em 0.2em 0.5em 0;
}

.jp-FormGroup-contentCompact
  .jp-FormGroup-compactTitle
  .jp-FormGroup-description {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color2);
}

.jp-FormGroup-contentCompact .jp-FormGroup-fieldLabel {
  padding-bottom: 0.3em;
}

.jp-FormGroup-contentCompact .jp-inputFieldWrapper .form-control {
  width: 100%;
  box-sizing: border-box;
}

.jp-FormGroup-contentCompact .jp-arrayFieldWrapper .jp-FormGroup-compactTitle {
  padding-bottom: 7px;
}

.jp-FormGroup-contentCompact
  .jp-objectFieldWrapper
  .jp-objectFieldWrapper
  .form-group {
  padding: 2px 8px 2px var(--jp-private-settingeditor-modifier-indent);
  margin-top: 2px;
}

.jp-FormGroup-contentCompact ul.error-detail {
  margin-block-start: 0.5em;
  margin-block-end: 0.5em;
  padding-inline-start: 1em;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-SidePanel {
  display: flex;
  flex-direction: column;
  min-width: var(--jp-sidebar-min-width);
  overflow-y: auto;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  font-size: var(--jp-ui-font-size1);
}

.jp-SidePanel-header {
  flex: 0 0 auto;
  display: flex;
  border-bottom: var(--jp-border-width) solid var(--jp-border-color2);
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  letter-spacing: 1px;
  margin: 0;
  padding: 2px;
  text-transform: uppercase;
}

.jp-SidePanel-toolbar {
  flex: 0 0 auto;
}

.jp-SidePanel-content {
  flex: 1 1 auto;
}

.jp-SidePanel-toolbar,
.jp-AccordionPanel-toolbar {
  height: var(--jp-private-toolbar-height);
}

.jp-SidePanel-toolbar.jp-Toolbar-micro {
  display: none;
}

.lm-AccordionPanel .jp-AccordionPanel-title {
  box-sizing: border-box;
  line-height: 25px;
  margin: 0;
  display: flex;
  align-items: center;
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  font-size: var(--jp-ui-font-size0);
}

.jp-AccordionPanel-title {
  cursor: pointer;
  user-select: none;
  -moz-user-select: none;
  -webkit-user-select: none;
  text-transform: uppercase;
}

.lm-AccordionPanel[data-orientation='horizontal'] > .jp-AccordionPanel-title {
  /* Title is rotated for horizontal accordion panel using CSS */
  display: block;
  transform-origin: top left;
  transform: rotate(-90deg) translate(-100%);
}

.jp-AccordionPanel-title .lm-AccordionPanel-titleLabel {
  user-select: none;
  text-overflow: ellipsis;
  white-space: nowrap;
  overflow: hidden;
}

.jp-AccordionPanel-title .lm-AccordionPanel-titleCollapser {
  transform: rotate(-90deg);
  margin: auto 0;
  height: 16px;
}

.jp-AccordionPanel-title.lm-mod-expanded .lm-AccordionPanel-titleCollapser {
  transform: rotate(0deg);
}

.lm-AccordionPanel .jp-AccordionPanel-toolbar {
  background: none;
  box-shadow: none;
  border: none;
  margin-left: auto;
}

.lm-AccordionPanel .lm-SplitPanel-handle:hover {
  background: var(--jp-layout-color3);
}

.jp-text-truncated {
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Spinner {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 10;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background: var(--jp-layout-color0);
  outline: none;
}

.jp-SpinnerContent {
  font-size: 10px;
  margin: 50px auto;
  text-indent: -9999em;
  width: 3em;
  height: 3em;
  border-radius: 50%;
  background: var(--jp-brand-color3);
  background: linear-gradient(
    to right,
    #f37626 10%,
    rgba(255, 255, 255, 0) 42%
  );
  position: relative;
  animation: load3 1s infinite linear, fadeIn 1s;
}

.jp-SpinnerContent::before {
  width: 50%;
  height: 50%;
  background: #f37626;
  border-radius: 100% 0 0;
  position: absolute;
  top: 0;
  left: 0;
  content: '';
}

.jp-SpinnerContent::after {
  background: var(--jp-layout-color0);
  width: 75%;
  height: 75%;
  border-radius: 50%;
  content: '';
  margin: auto;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

@keyframes load3 {
  0% {
    transform: rotate(0deg);
  }

  100% {
    transform: rotate(360deg);
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

button.jp-mod-styled {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  border: none;
  box-sizing: border-box;
  text-align: center;
  line-height: 32px;
  height: 32px;
  padding: 0 12px;
  letter-spacing: 0.8px;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

input.jp-mod-styled {
  background: var(--jp-input-background);
  height: 28px;
  box-sizing: border-box;
  border: var(--jp-border-width) solid var(--jp-border-color1);
  padding-left: 7px;
  padding-right: 7px;
  font-size: var(--jp-ui-font-size2);
  color: var(--jp-ui-font-color0);
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

input[type='checkbox'].jp-mod-styled {
  appearance: checkbox;
  -webkit-appearance: checkbox;
  -moz-appearance: checkbox;
  height: auto;
}

input.jp-mod-styled:focus {
  border: var(--jp-border-width) solid var(--md-blue-500);
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-select-wrapper {
  display: flex;
  position: relative;
  flex-direction: column;
  padding: 1px;
  background-color: var(--jp-layout-color1);
  box-sizing: border-box;
  margin-bottom: 12px;
}

.jp-select-wrapper:not(.multiple) {
  height: 28px;
}

.jp-select-wrapper.jp-mod-focused select.jp-mod-styled {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-input-active-background);
}

select.jp-mod-styled:hover {
  cursor: pointer;
  color: var(--jp-ui-font-color0);
  background-color: var(--jp-input-hover-background);
  box-shadow: inset 0 0 1px rgba(0, 0, 0, 0.5);
}

select.jp-mod-styled {
  flex: 1 1 auto;
  width: 100%;
  font-size: var(--jp-ui-font-size2);
  background: var(--jp-input-background);
  color: var(--jp-ui-font-color0);
  padding: 0 25px 0 8px;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

select.jp-mod-styled:not([multiple]) {
  height: 32px;
}

select.jp-mod-styled[multiple] {
  max-height: 200px;
  overflow-y: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-switch {
  display: flex;
  align-items: center;
  padding-left: 4px;
  padding-right: 4px;
  font-size: var(--jp-ui-font-size1);
  background-color: transparent;
  color: var(--jp-ui-font-color1);
  border: none;
  height: 20px;
}

.jp-switch:hover {
  background-color: var(--jp-layout-color2);
}

.jp-switch-label {
  margin-right: 5px;
  font-family: var(--jp-ui-font-family);
}

.jp-switch-track {
  cursor: pointer;
  background-color: var(--jp-switch-color, var(--jp-border-color1));
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 34px;
  height: 16px;
  width: 35px;
  position: relative;
}

.jp-switch-track::before {
  content: '';
  position: absolute;
  height: 10px;
  width: 10px;
  margin: 3px;
  left: 0;
  background-color: var(--jp-ui-inverse-font-color1);
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 50%;
}

.jp-switch[aria-checked='true'] .jp-switch-track {
  background-color: var(--jp-switch-true-position-color, var(--jp-warn-color0));
}

.jp-switch[aria-checked='true'] .jp-switch-track::before {
  /* track width (35) - margins (3 + 3) - thumb width (10) */
  left: 19px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

:root {
  --jp-private-toolbar-height: calc(
    28px + var(--jp-border-width)
  ); /* leave 28px for content */
}

.jp-Toolbar {
  color: var(--jp-ui-font-color1);
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  background: var(--jp-toolbar-background);
  min-height: var(--jp-toolbar-micro-height);
  padding: 2px;
  z-index: 8;
  overflow-x: hidden;
}

/* Toolbar items */

.jp-Toolbar > .jp-Toolbar-item.jp-Toolbar-spacer {
  flex-grow: 1;
  flex-shrink: 1;
}

.jp-Toolbar-item.jp-Toolbar-kernelStatus {
  display: inline-block;
  width: 32px;
  background-repeat: no-repeat;
  background-position: center;
  background-size: 16px;
}

.jp-Toolbar > .jp-Toolbar-item {
  flex: 0 0 auto;
  display: flex;
  padding-left: 1px;
  padding-right: 1px;
  font-size: var(--jp-ui-font-size1);
  line-height: var(--jp-private-toolbar-height);
  height: 100%;
}

/* Toolbar buttons */

/* This is the div we use to wrap the react component into a Widget */
div.jp-ToolbarButton {
  color: transparent;
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0;
  margin: 0;
}

button.jp-ToolbarButtonComponent {
  background: var(--jp-layout-color1);
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0 6px;
  margin: 0;
  height: 24px;
  border-radius: var(--jp-border-radius);
  display: flex;
  align-items: center;
  text-align: center;
  font-size: 14px;
  min-width: unset;
  min-height: unset;
}

button.jp-ToolbarButtonComponent:disabled {
  opacity: 0.4;
}

button.jp-ToolbarButtonComponent > span {
  padding: 0;
  flex: 0 0 auto;
}

button.jp-ToolbarButtonComponent .jp-ToolbarButtonComponent-label {
  font-size: var(--jp-ui-font-size1);
  line-height: 100%;
  padding-left: 2px;
  color: var(--jp-ui-font-color1);
  font-family: var(--jp-ui-font-family);
}

#jp-main-dock-panel[data-mode='single-document']
  .jp-MainAreaWidget
  > .jp-Toolbar.jp-Toolbar-micro {
  padding: 0;
  min-height: 0;
}

#jp-main-dock-panel[data-mode='single-document']
  .jp-MainAreaWidget
  > .jp-Toolbar {
  border: none;
  box-shadow: none;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-WindowedPanel-outer {
  position: relative;
  overflow-y: auto;
}

.jp-WindowedPanel-inner {
  position: relative;
}

.jp-WindowedPanel-window {
  position: absolute;
  left: 0;
  right: 0;
  overflow: visible;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* Sibling imports */

body {
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
}

/* Disable native link decoration styles everywhere outside of dialog boxes */
a {
  text-decoration: unset;
  color: unset;
}

a:hover {
  text-decoration: unset;
  color: unset;
}

/* Accessibility for links inside dialog box text */
.jp-Dialog-content a {
  text-decoration: revert;
  color: var(--jp-content-link-color);
}

.jp-Dialog-content a:hover {
  text-decoration: revert;
}

/* Styles for ui-components */
.jp-Button {
  color: var(--jp-ui-font-color2);
  border-radius: var(--jp-border-radius);
  padding: 0 12px;
  font-size: var(--jp-ui-font-size1);

  /* Copy from blueprint 3 */
  display: inline-flex;
  flex-direction: row;
  border: none;
  cursor: pointer;
  align-items: center;
  justify-content: center;
  text-align: left;
  vertical-align: middle;
  min-height: 30px;
  min-width: 30px;
}

.jp-Button:disabled {
  cursor: not-allowed;
}

.jp-Button:empty {
  padding: 0 !important;
}

.jp-Button.jp-mod-small {
  min-height: 24px;
  min-width: 24px;
  font-size: 12px;
  padding: 0 7px;
}

/* Use our own theme for hover styles */
.jp-Button.jp-mod-minimal:hover {
  background-color: var(--jp-layout-color2);
}

.jp-Button.jp-mod-minimal {
  background: none;
}

.jp-InputGroup {
  display: block;
  position: relative;
}

.jp-InputGroup input {
  box-sizing: border-box;
  border: none;
  border-radius: 0;
  background-color: transparent;
  color: var(--jp-ui-font-color0);
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
  padding-bottom: 0;
  padding-top: 0;
  padding-left: 10px;
  padding-right: 28px;
  position: relative;
  width: 100%;
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
  font-size: 14px;
  font-weight: 400;
  height: 30px;
  line-height: 30px;
  outline: none;
  vertical-align: middle;
}

.jp-InputGroup input:focus {
  box-shadow: inset 0 0 0 var(--jp-border-width)
      var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-InputGroup input:disabled {
  cursor: not-allowed;
  resize: block;
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color2);
}

.jp-InputGroup input:disabled ~ span {
  cursor: not-allowed;
  color: var(--jp-ui-font-color2);
}

.jp-InputGroup input::placeholder,
input::placeholder {
  color: var(--jp-ui-font-color2);
}

.jp-InputGroupAction {
  position: absolute;
  bottom: 1px;
  right: 0;
  padding: 6px;
}

.jp-HTMLSelect.jp-DefaultStyle select {
  background-color: initial;
  border: none;
  border-radius: 0;
  box-shadow: none;
  color: var(--jp-ui-font-color0);
  display: block;
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  height: 24px;
  line-height: 14px;
  padding: 0 25px 0 10px;
  text-align: left;
  -moz-appearance: none;
  -webkit-appearance: none;
}

.jp-HTMLSelect.jp-DefaultStyle select:disabled {
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color2);
  cursor: not-allowed;
  resize: block;
}

.jp-HTMLSelect.jp-DefaultStyle select:disabled ~ span {
  cursor: not-allowed;
}

/* Use our own theme for hover and option styles */
/* stylelint-disable-next-line selector-max-type */
.jp-HTMLSelect.jp-DefaultStyle select:hover,
.jp-HTMLSelect.jp-DefaultStyle select > option {
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color0);
}

select {
  box-sizing: border-box;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-StatusBar-Widget {
  display: flex;
  align-items: center;
  background: var(--jp-layout-color2);
  min-height: var(--jp-statusbar-height);
  justify-content: space-between;
  padding: 0 10px;
}

.jp-StatusBar-Left {
  display: flex;
  align-items: center;
  flex-direction: row;
}

.jp-StatusBar-Middle {
  display: flex;
  align-items: center;
}

.jp-StatusBar-Right {
  display: flex;
  align-items: center;
  flex-direction: row-reverse;
}

.jp-StatusBar-Item {
  max-height: var(--jp-statusbar-height);
  margin: 0 2px;
  height: var(--jp-statusbar-height);
  white-space: nowrap;
  text-overflow: ellipsis;
  color: var(--jp-ui-font-color1);
  padding: 0 6px;
}

.jp-mod-highlighted:hover {
  background-color: var(--jp-layout-color3);
}

.jp-mod-clicked {
  background-color: var(--jp-brand-color1);
}

.jp-mod-clicked:hover {
  background-color: var(--jp-brand-color0);
}

.jp-mod-clicked .jp-StatusBar-TextItem {
  color: var(--jp-ui-inverse-font-color1);
}

.jp-StatusBar-HoverItem {
  box-shadow: '0px 4px 4px rgba(0, 0, 0, 0.25)';
}

.jp-StatusBar-TextItem {
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  line-height: 24px;
  color: var(--jp-ui-font-color1);
}

.jp-StatusBar-GroupItem {
  display: flex;
  align-items: center;
  flex-direction: row;
}

.jp-Statusbar-ProgressCircle svg {
  display: block;
  margin: 0 auto;
  width: 16px;
  height: 24px;
  align-self: normal;
}

.jp-Statusbar-ProgressCircle path {
  fill: var(--jp-inverse-layout-color3);
}

.jp-Statusbar-ProgressBar-progress-bar {
  height: 10px;
  width: 100px;
  border: solid 0.25px var(--jp-brand-color2);
  border-radius: 3px;
  overflow: hidden;
  align-self: center;
}

.jp-Statusbar-ProgressBar-progress-bar > div {
  background-color: var(--jp-brand-color2);
  background-image: linear-gradient(
    -45deg,
    rgba(255, 255, 255, 0.2) 25%,
    transparent 25%,
    transparent 50%,
    rgba(255, 255, 255, 0.2) 50%,
    rgba(255, 255, 255, 0.2) 75%,
    transparent 75%,
    transparent
  );
  background-size: 40px 40px;
  float: left;
  width: 0%;
  height: 100%;
  font-size: 12px;
  line-height: 14px;
  color: #fff;
  text-align: center;
  animation: jp-Statusbar-ExecutionTime-progress-bar 2s linear infinite;
}

.jp-Statusbar-ProgressBar-progress-bar p {
  color: var(--jp-ui-font-color1);
  font-family: var(--jp-ui-font-family);
  font-size: var(--jp-ui-font-size1);
  line-height: 10px;
  width: 100px;
}

@keyframes jp-Statusbar-ExecutionTime-progress-bar {
  0% {
    background-position: 0 0;
  }

  100% {
    background-position: 40px 40px;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-commandpalette-search-height: 28px;
}

/*-----------------------------------------------------------------------------
| Overall styles
|----------------------------------------------------------------------------*/

.lm-CommandPalette {
  padding-bottom: 0;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);

  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Modal variant
|----------------------------------------------------------------------------*/

.jp-ModalCommandPalette {
  position: absolute;
  z-index: 10000;
  top: 38px;
  left: 30%;
  margin: 0;
  padding: 4px;
  width: 40%;
  box-shadow: var(--jp-elevation-z4);
  border-radius: 4px;
  background: var(--jp-layout-color0);
}

.jp-ModalCommandPalette .lm-CommandPalette {
  max-height: 40vh;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-close-icon::after {
  display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-header {
  display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-item {
  margin-left: 4px;
  margin-right: 4px;
}

.jp-ModalCommandPalette
  .lm-CommandPalette
  .lm-CommandPalette-item.lm-mod-disabled {
  display: none;
}

/*-----------------------------------------------------------------------------
| Search
|----------------------------------------------------------------------------*/

.lm-CommandPalette-search {
  padding: 4px;
  background-color: var(--jp-layout-color1);
  z-index: 2;
}

.lm-CommandPalette-wrapper {
  overflow: overlay;
  padding: 0 9px;
  background-color: var(--jp-input-active-background);
  height: 30px;
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
}

.lm-CommandPalette.lm-mod-focused .lm-CommandPalette-wrapper {
  box-shadow: inset 0 0 0 1px var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-SearchIconGroup {
  color: white;
  background-color: var(--jp-brand-color1);
  position: absolute;
  top: 4px;
  right: 4px;
  padding: 5px 5px 1px;
}

.jp-SearchIconGroup svg {
  height: 20px;
  width: 20px;
}

.jp-SearchIconGroup .jp-icon3[fill] {
  fill: var(--jp-layout-color0);
}

.lm-CommandPalette-input {
  background: transparent;
  width: calc(100% - 18px);
  float: left;
  border: none;
  outline: none;
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  line-height: var(--jp-private-commandpalette-search-height);
}

.lm-CommandPalette-input::-webkit-input-placeholder,
.lm-CommandPalette-input::-moz-placeholder,
.lm-CommandPalette-input:-ms-input-placeholder {
  color: var(--jp-ui-font-color2);
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Results
|----------------------------------------------------------------------------*/

.lm-CommandPalette-header:first-child {
  margin-top: 0;
}

.lm-CommandPalette-header {
  border-bottom: solid var(--jp-border-width) var(--jp-border-color2);
  color: var(--jp-ui-font-color1);
  cursor: pointer;
  display: flex;
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  letter-spacing: 1px;
  margin-top: 8px;
  padding: 8px 0 8px 12px;
  text-transform: uppercase;
}

.lm-CommandPalette-header.lm-mod-active {
  background: var(--jp-layout-color2);
}

.lm-CommandPalette-header > mark {
  background-color: transparent;
  font-weight: bold;
  color: var(--jp-ui-font-color1);
}

.lm-CommandPalette-item {
  padding: 4px 12px 4px 4px;
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  font-weight: 400;
  display: flex;
}

.lm-CommandPalette-item.lm-mod-disabled {
  color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item.lm-mod-active {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.lm-CommandPalette-item.lm-mod-active .lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-inverse-font-color0);
}

.lm-CommandPalette-item.lm-mod-active .jp-icon-selectable[fill] {
  fill: var(--jp-layout-color0);
}

.lm-CommandPalette-item.lm-mod-active:hover:not(.lm-mod-disabled) {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.lm-CommandPalette-item:hover:not(.lm-mod-active):not(.lm-mod-disabled) {
  background: var(--jp-layout-color2);
}

.lm-CommandPalette-itemContent {
  overflow: hidden;
}

.lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-font-color0);
  background-color: transparent;
  font-weight: bold;
}

.lm-CommandPalette-item.lm-mod-disabled mark {
  color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item .lm-CommandPalette-itemIcon {
  margin: 0 4px 0 0;
  position: relative;
  width: 16px;
  top: 2px;
  flex: 0 0 auto;
}

.lm-CommandPalette-item.lm-mod-disabled .lm-CommandPalette-itemIcon {
  opacity: 0.6;
}

.lm-CommandPalette-item .lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemCaption {
  display: none;
}

.lm-CommandPalette-content {
  background-color: var(--jp-layout-color1);
}

.lm-CommandPalette-content:empty::after {
  content: 'No results';
  margin: auto;
  margin-top: 20px;
  width: 100px;
  display: block;
  font-size: var(--jp-ui-font-size2);
  font-family: var(--jp-ui-font-family);
  font-weight: lighter;
}

.lm-CommandPalette-emptyMessage {
  text-align: center;
  margin-top: 24px;
  line-height: 1.32;
  padding: 0 8px;
  color: var(--jp-content-font-color3);
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Dialog {
  position: absolute;
  z-index: 10000;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  top: 0;
  left: 0;
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
  background: var(--jp-dialog-background);
}

.jp-Dialog-content {
  display: flex;
  flex-direction: column;
  margin-left: auto;
  margin-right: auto;
  background: var(--jp-layout-color1);
  padding: 24px 24px 12px;
  min-width: 300px;
  min-height: 150px;
  max-width: 1000px;
  max-height: 500px;
  box-sizing: border-box;
  box-shadow: var(--jp-elevation-z20);
  word-wrap: break-word;
  border-radius: var(--jp-border-radius);

  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color1);
  resize: both;
}

.jp-Dialog-content.jp-Dialog-content-small {
  max-width: 500px;
}

.jp-Dialog-button {
  overflow: visible;
}

button.jp-Dialog-button:focus {
  outline: 1px solid var(--jp-brand-color1);
  outline-offset: 4px;
  -moz-outline-radius: 0;
}

button.jp-Dialog-button:focus::-moz-focus-inner {
  border: 0;
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-accept:focus,
button.jp-Dialog-button.jp-mod-styled.jp-mod-warn:focus,
button.jp-Dialog-button.jp-mod-styled.jp-mod-reject:focus {
  outline-offset: 4px;
  -moz-outline-radius: 0;
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-accept:focus {
  outline: 1px solid var(--jp-accept-color-normal, var(--jp-brand-color1));
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-warn:focus {
  outline: 1px solid var(--jp-warn-color-normal, var(--jp-error-color1));
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-reject:focus {
  outline: 1px solid var(--jp-reject-color-normal, var(--md-grey-600));
}

button.jp-Dialog-close-button {
  padding: 0;
  height: 100%;
  min-width: unset;
  min-height: unset;
}

.jp-Dialog-header {
  display: flex;
  justify-content: space-between;
  flex: 0 0 auto;
  padding-bottom: 12px;
  font-size: var(--jp-ui-font-size3);
  font-weight: 400;
  color: var(--jp-ui-font-color1);
}

.jp-Dialog-body {
  display: flex;
  flex-direction: column;
  flex: 1 1 auto;
  font-size: var(--jp-ui-font-size1);
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
}

.jp-Dialog-footer {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
  flex: 0 0 auto;
  margin-left: -12px;
  margin-right: -12px;
  padding: 12px;
}

.jp-Dialog-checkbox {
  padding-right: 5px;
}

.jp-Dialog-checkbox > input:focus-visible {
  outline: 1px solid var(--jp-input-active-border-color);
  outline-offset: 1px;
}

.jp-Dialog-spacer {
  flex: 1 1 auto;
}

.jp-Dialog-title {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.jp-Dialog-body > .jp-select-wrapper {
  width: 100%;
}

.jp-Dialog-body > button {
  padding: 0 16px;
}

.jp-Dialog-body > label {
  line-height: 1.4;
  color: var(--jp-ui-font-color0);
}

.jp-Dialog-button.jp-mod-styled:not(:last-child) {
  margin-right: 12px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-Input-Boolean-Dialog {
  flex-direction: row-reverse;
  align-items: end;
  width: 100%;
}

.jp-Input-Boolean-Dialog > label {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-MainAreaWidget > :focus {
  outline: none;
}

.jp-MainAreaWidget .jp-MainAreaWidget-error {
  padding: 6px;
}

.jp-MainAreaWidget .jp-MainAreaWidget-error > pre {
  width: auto;
  padding: 10px;
  background: var(--jp-error-color3);
  border: var(--jp-border-width) solid var(--jp-error-color1);
  border-radius: var(--jp-border-radius);
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  white-space: pre-wrap;
  word-wrap: break-word;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/**
 * google-material-color v1.2.6
 * https://github.com/danlevan/google-material-color
 */
:root {
  --md-red-50: #ffebee;
  --md-red-100: #ffcdd2;
  --md-red-200: #ef9a9a;
  --md-red-300: #e57373;
  --md-red-400: #ef5350;
  --md-red-500: #f44336;
  --md-red-600: #e53935;
  --md-red-700: #d32f2f;
  --md-red-800: #c62828;
  --md-red-900: #b71c1c;
  --md-red-A100: #ff8a80;
  --md-red-A200: #ff5252;
  --md-red-A400: #ff1744;
  --md-red-A700: #d50000;
  --md-pink-50: #fce4ec;
  --md-pink-100: #f8bbd0;
  --md-pink-200: #f48fb1;
  --md-pink-300: #f06292;
  --md-pink-400: #ec407a;
  --md-pink-500: #e91e63;
  --md-pink-600: #d81b60;
  --md-pink-700: #c2185b;
  --md-pink-800: #ad1457;
  --md-pink-900: #880e4f;
  --md-pink-A100: #ff80ab;
  --md-pink-A200: #ff4081;
  --md-pink-A400: #f50057;
  --md-pink-A700: #c51162;
  --md-purple-50: #f3e5f5;
  --md-purple-100: #e1bee7;
  --md-purple-200: #ce93d8;
  --md-purple-300: #ba68c8;
  --md-purple-400: #ab47bc;
  --md-purple-500: #9c27b0;
  --md-purple-600: #8e24aa;
  --md-purple-700: #7b1fa2;
  --md-purple-800: #6a1b9a;
  --md-purple-900: #4a148c;
  --md-purple-A100: #ea80fc;
  --md-purple-A200: #e040fb;
  --md-purple-A400: #d500f9;
  --md-purple-A700: #a0f;
  --md-deep-purple-50: #ede7f6;
  --md-deep-purple-100: #d1c4e9;
  --md-deep-purple-200: #b39ddb;
  --md-deep-purple-300: #9575cd;
  --md-deep-purple-400: #7e57c2;
  --md-deep-purple-500: #673ab7;
  --md-deep-purple-600: #5e35b1;
  --md-deep-purple-700: #512da8;
  --md-deep-purple-800: #4527a0;
  --md-deep-purple-900: #311b92;
  --md-deep-purple-A100: #b388ff;
  --md-deep-purple-A200: #7c4dff;
  --md-deep-purple-A400: #651fff;
  --md-deep-purple-A700: #6200ea;
  --md-indigo-50: #e8eaf6;
  --md-indigo-100: #c5cae9;
  --md-indigo-200: #9fa8da;
  --md-indigo-300: #7986cb;
  --md-indigo-400: #5c6bc0;
  --md-indigo-500: #3f51b5;
  --md-indigo-600: #3949ab;
  --md-indigo-700: #303f9f;
  --md-indigo-800: #283593;
  --md-indigo-900: #1a237e;
  --md-indigo-A100: #8c9eff;
  --md-indigo-A200: #536dfe;
  --md-indigo-A400: #3d5afe;
  --md-indigo-A700: #304ffe;
  --md-blue-50: #e3f2fd;
  --md-blue-100: #bbdefb;
  --md-blue-200: #90caf9;
  --md-blue-300: #64b5f6;
  --md-blue-400: #42a5f5;
  --md-blue-500: #2196f3;
  --md-blue-600: #1e88e5;
  --md-blue-700: #1976d2;
  --md-blue-800: #1565c0;
  --md-blue-900: #0d47a1;
  --md-blue-A100: #82b1ff;
  --md-blue-A200: #448aff;
  --md-blue-A400: #2979ff;
  --md-blue-A700: #2962ff;
  --md-light-blue-50: #e1f5fe;
  --md-light-blue-100: #b3e5fc;
  --md-light-blue-200: #81d4fa;
  --md-light-blue-300: #4fc3f7;
  --md-light-blue-400: #29b6f6;
  --md-light-blue-500: #03a9f4;
  --md-light-blue-600: #039be5;
  --md-light-blue-700: #0288d1;
  --md-light-blue-800: #0277bd;
  --md-light-blue-900: #01579b;
  --md-light-blue-A100: #80d8ff;
  --md-light-blue-A200: #40c4ff;
  --md-light-blue-A400: #00b0ff;
  --md-light-blue-A700: #0091ea;
  --md-cyan-50: #e0f7fa;
  --md-cyan-100: #b2ebf2;
  --md-cyan-200: #80deea;
  --md-cyan-300: #4dd0e1;
  --md-cyan-400: #26c6da;
  --md-cyan-500: #00bcd4;
  --md-cyan-600: #00acc1;
  --md-cyan-700: #0097a7;
  --md-cyan-800: #00838f;
  --md-cyan-900: #006064;
  --md-cyan-A100: #84ffff;
  --md-cyan-A200: #18ffff;
  --md-cyan-A400: #00e5ff;
  --md-cyan-A700: #00b8d4;
  --md-teal-50: #e0f2f1;
  --md-teal-100: #b2dfdb;
  --md-teal-200: #80cbc4;
  --md-teal-300: #4db6ac;
  --md-teal-400: #26a69a;
  --md-teal-500: #009688;
  --md-teal-600: #00897b;
  --md-teal-700: #00796b;
  --md-teal-800: #00695c;
  --md-teal-900: #004d40;
  --md-teal-A100: #a7ffeb;
  --md-teal-A200: #64ffda;
  --md-teal-A400: #1de9b6;
  --md-teal-A700: #00bfa5;
  --md-green-50: #e8f5e9;
  --md-green-100: #c8e6c9;
  --md-green-200: #a5d6a7;
  --md-green-300: #81c784;
  --md-green-400: #66bb6a;
  --md-green-500: #4caf50;
  --md-green-600: #43a047;
  --md-green-700: #388e3c;
  --md-green-800: #2e7d32;
  --md-green-900: #1b5e20;
  --md-green-A100: #b9f6ca;
  --md-green-A200: #69f0ae;
  --md-green-A400: #00e676;
  --md-green-A700: #00c853;
  --md-light-green-50: #f1f8e9;
  --md-light-green-100: #dcedc8;
  --md-light-green-200: #c5e1a5;
  --md-light-green-300: #aed581;
  --md-light-green-400: #9ccc65;
  --md-light-green-500: #8bc34a;
  --md-light-green-600: #7cb342;
  --md-light-green-700: #689f38;
  --md-light-green-800: #558b2f;
  --md-light-green-900: #33691e;
  --md-light-green-A100: #ccff90;
  --md-light-green-A200: #b2ff59;
  --md-light-green-A400: #76ff03;
  --md-light-green-A700: #64dd17;
  --md-lime-50: #f9fbe7;
  --md-lime-100: #f0f4c3;
  --md-lime-200: #e6ee9c;
  --md-lime-300: #dce775;
  --md-lime-400: #d4e157;
  --md-lime-500: #cddc39;
  --md-lime-600: #c0ca33;
  --md-lime-700: #afb42b;
  --md-lime-800: #9e9d24;
  --md-lime-900: #827717;
  --md-lime-A100: #f4ff81;
  --md-lime-A200: #eeff41;
  --md-lime-A400: #c6ff00;
  --md-lime-A700: #aeea00;
  --md-yellow-50: #fffde7;
  --md-yellow-100: #fff9c4;
  --md-yellow-200: #fff59d;
  --md-yellow-300: #fff176;
  --md-yellow-400: #ffee58;
  --md-yellow-500: #ffeb3b;
  --md-yellow-600: #fdd835;
  --md-yellow-700: #fbc02d;
  --md-yellow-800: #f9a825;
  --md-yellow-900: #f57f17;
  --md-yellow-A100: #ffff8d;
  --md-yellow-A200: #ff0;
  --md-yellow-A400: #ffea00;
  --md-yellow-A700: #ffd600;
  --md-amber-50: #fff8e1;
  --md-amber-100: #ffecb3;
  --md-amber-200: #ffe082;
  --md-amber-300: #ffd54f;
  --md-amber-400: #ffca28;
  --md-amber-500: #ffc107;
  --md-amber-600: #ffb300;
  --md-amber-700: #ffa000;
  --md-amber-800: #ff8f00;
  --md-amber-900: #ff6f00;
  --md-amber-A100: #ffe57f;
  --md-amber-A200: #ffd740;
  --md-amber-A400: #ffc400;
  --md-amber-A700: #ffab00;
  --md-orange-50: #fff3e0;
  --md-orange-100: #ffe0b2;
  --md-orange-200: #ffcc80;
  --md-orange-300: #ffb74d;
  --md-orange-400: #ffa726;
  --md-orange-500: #ff9800;
  --md-orange-600: #fb8c00;
  --md-orange-700: #f57c00;
  --md-orange-800: #ef6c00;
  --md-orange-900: #e65100;
  --md-orange-A100: #ffd180;
  --md-orange-A200: #ffab40;
  --md-orange-A400: #ff9100;
  --md-orange-A700: #ff6d00;
  --md-deep-orange-50: #fbe9e7;
  --md-deep-orange-100: #ffccbc;
  --md-deep-orange-200: #ffab91;
  --md-deep-orange-300: #ff8a65;
  --md-deep-orange-400: #ff7043;
  --md-deep-orange-500: #ff5722;
  --md-deep-orange-600: #f4511e;
  --md-deep-orange-700: #e64a19;
  --md-deep-orange-800: #d84315;
  --md-deep-orange-900: #bf360c;
  --md-deep-orange-A100: #ff9e80;
  --md-deep-orange-A200: #ff6e40;
  --md-deep-orange-A400: #ff3d00;
  --md-deep-orange-A700: #dd2c00;
  --md-brown-50: #efebe9;
  --md-brown-100: #d7ccc8;
  --md-brown-200: #bcaaa4;
  --md-brown-300: #a1887f;
  --md-brown-400: #8d6e63;
  --md-brown-500: #795548;
  --md-brown-600: #6d4c41;
  --md-brown-700: #5d4037;
  --md-brown-800: #4e342e;
  --md-brown-900: #3e2723;
  --md-grey-50: #fafafa;
  --md-grey-100: #f5f5f5;
  --md-grey-200: #eee;
  --md-grey-300: #e0e0e0;
  --md-grey-400: #bdbdbd;
  --md-grey-500: #9e9e9e;
  --md-grey-600: #757575;
  --md-grey-700: #616161;
  --md-grey-800: #424242;
  --md-grey-900: #212121;
  --md-blue-grey-50: #eceff1;
  --md-blue-grey-100: #cfd8dc;
  --md-blue-grey-200: #b0bec5;
  --md-blue-grey-300: #90a4ae;
  --md-blue-grey-400: #78909c;
  --md-blue-grey-500: #607d8b;
  --md-blue-grey-600: #546e7a;
  --md-blue-grey-700: #455a64;
  --md-blue-grey-800: #37474f;
  --md-blue-grey-900: #263238;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| RenderedText
|----------------------------------------------------------------------------*/

:root {
  /* This is the padding value to fill the gaps between lines containing spans with background color. */
  --jp-private-code-span-padding: calc(
    (var(--jp-code-line-height) - 1) * var(--jp-code-font-size) / 2
  );
}

.jp-RenderedText {
  text-align: left;
  padding-left: var(--jp-code-padding);
  line-height: var(--jp-code-line-height);
  font-family: var(--jp-code-font-family);
}

.jp-RenderedText pre,
.jp-RenderedJavaScript pre,
.jp-RenderedHTMLCommon pre {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-code-font-size);
  border: none;
  margin: 0;
  padding: 0;
}

.jp-RenderedText pre a:link {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

.jp-RenderedText pre a:hover {
  text-decoration: underline;
  color: var(--jp-content-link-color);
}

.jp-RenderedText pre a:visited {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

/* console foregrounds and backgrounds */
.jp-RenderedText pre .ansi-black-fg {
  color: #3e424d;
}

.jp-RenderedText pre .ansi-red-fg {
  color: #e75c58;
}

.jp-RenderedText pre .ansi-green-fg {
  color: #00a250;
}

.jp-RenderedText pre .ansi-yellow-fg {
  color: #ddb62b;
}

.jp-RenderedText pre .ansi-blue-fg {
  color: #208ffb;
}

.jp-RenderedText pre .ansi-magenta-fg {
  color: #d160c4;
}

.jp-RenderedText pre .ansi-cyan-fg {
  color: #60c6c8;
}

.jp-RenderedText pre .ansi-white-fg {
  color: #c5c1b4;
}

.jp-RenderedText pre .ansi-black-bg {
  background-color: #3e424d;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-red-bg {
  background-color: #e75c58;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-green-bg {
  background-color: #00a250;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-yellow-bg {
  background-color: #ddb62b;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-blue-bg {
  background-color: #208ffb;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-magenta-bg {
  background-color: #d160c4;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-cyan-bg {
  background-color: #60c6c8;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-white-bg {
  background-color: #c5c1b4;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-black-intense-fg {
  color: #282c36;
}

.jp-RenderedText pre .ansi-red-intense-fg {
  color: #b22b31;
}

.jp-RenderedText pre .ansi-green-intense-fg {
  color: #007427;
}

.jp-RenderedText pre .ansi-yellow-intense-fg {
  color: #b27d12;
}

.jp-RenderedText pre .ansi-blue-intense-fg {
  color: #0065ca;
}

.jp-RenderedText pre .ansi-magenta-intense-fg {
  color: #a03196;
}

.jp-RenderedText pre .ansi-cyan-intense-fg {
  color: #258f8f;
}

.jp-RenderedText pre .ansi-white-intense-fg {
  color: #a1a6b2;
}

.jp-RenderedText pre .ansi-black-intense-bg {
  background-color: #282c36;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-red-intense-bg {
  background-color: #b22b31;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-green-intense-bg {
  background-color: #007427;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-yellow-intense-bg {
  background-color: #b27d12;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-blue-intense-bg {
  background-color: #0065ca;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-magenta-intense-bg {
  background-color: #a03196;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-cyan-intense-bg {
  background-color: #258f8f;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-white-intense-bg {
  background-color: #a1a6b2;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-default-inverse-fg {
  color: var(--jp-ui-inverse-font-color0);
}

.jp-RenderedText pre .ansi-default-inverse-bg {
  background-color: var(--jp-inverse-layout-color0);
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-bold {
  font-weight: bold;
}

.jp-RenderedText pre .ansi-underline {
  text-decoration: underline;
}

.jp-RenderedText[data-mime-type='application/vnd.jupyter.stderr'] {
  background: var(--jp-rendermime-error-background);
  padding-top: var(--jp-code-padding);
}

/*-----------------------------------------------------------------------------
| RenderedLatex
|----------------------------------------------------------------------------*/

.jp-RenderedLatex {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-content-font-size1);
  line-height: var(--jp-content-line-height);
}

/* Left-justify outputs.*/
.jp-OutputArea-output.jp-RenderedLatex {
  padding: var(--jp-code-padding);
  text-align: left;
}

/*-----------------------------------------------------------------------------
| RenderedHTML
|----------------------------------------------------------------------------*/

.jp-RenderedHTMLCommon {
  color: var(--jp-content-font-color1);
  font-family: var(--jp-content-font-family);
  font-size: var(--jp-content-font-size1);
  line-height: var(--jp-content-line-height);

  /* Give a bit more R padding on Markdown text to keep line lengths reasonable */
  padding-right: 20px;
}

.jp-RenderedHTMLCommon em {
  font-style: italic;
}

.jp-RenderedHTMLCommon strong {
  font-weight: bold;
}

.jp-RenderedHTMLCommon u {
  text-decoration: underline;
}

.jp-RenderedHTMLCommon a:link {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:hover {
  text-decoration: underline;
  color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:visited {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

/* Headings */

.jp-RenderedHTMLCommon h1,
.jp-RenderedHTMLCommon h2,
.jp-RenderedHTMLCommon h3,
.jp-RenderedHTMLCommon h4,
.jp-RenderedHTMLCommon h5,
.jp-RenderedHTMLCommon h6 {
  line-height: var(--jp-content-heading-line-height);
  font-weight: var(--jp-content-heading-font-weight);
  font-style: normal;
  margin: var(--jp-content-heading-margin-top) 0
    var(--jp-content-heading-margin-bottom) 0;
}

.jp-RenderedHTMLCommon h1:first-child,
.jp-RenderedHTMLCommon h2:first-child,
.jp-RenderedHTMLCommon h3:first-child,
.jp-RenderedHTMLCommon h4:first-child,
.jp-RenderedHTMLCommon h5:first-child,
.jp-RenderedHTMLCommon h6:first-child {
  margin-top: calc(0.5 * var(--jp-content-heading-margin-top));
}

.jp-RenderedHTMLCommon h1:last-child,
.jp-RenderedHTMLCommon h2:last-child,
.jp-RenderedHTMLCommon h3:last-child,
.jp-RenderedHTMLCommon h4:last-child,
.jp-RenderedHTMLCommon h5:last-child,
.jp-RenderedHTMLCommon h6:last-child {
  margin-bottom: calc(0.5 * var(--jp-content-heading-margin-bottom));
}

.jp-RenderedHTMLCommon h1 {
  font-size: var(--jp-content-font-size5);
}

.jp-RenderedHTMLCommon h2 {
  font-size: var(--jp-content-font-size4);
}

.jp-RenderedHTMLCommon h3 {
  font-size: var(--jp-content-font-size3);
}

.jp-RenderedHTMLCommon h4 {
  font-size: var(--jp-content-font-size2);
}

.jp-RenderedHTMLCommon h5 {
  font-size: var(--jp-content-font-size1);
}

.jp-RenderedHTMLCommon h6 {
  font-size: var(--jp-content-font-size0);
}

/* Lists */

/* stylelint-disable selector-max-type, selector-max-compound-selectors */

.jp-RenderedHTMLCommon ul:not(.list-inline),
.jp-RenderedHTMLCommon ol:not(.list-inline) {
  padding-left: 2em;
}

.jp-RenderedHTMLCommon ul {
  list-style: disc;
}

.jp-RenderedHTMLCommon ul ul {
  list-style: square;
}

.jp-RenderedHTMLCommon ul ul ul {
  list-style: circle;
}

.jp-RenderedHTMLCommon ol {
  list-style: decimal;
}

.jp-RenderedHTMLCommon ol ol {
  list-style: upper-alpha;
}

.jp-RenderedHTMLCommon ol ol ol {
  list-style: lower-alpha;
}

.jp-RenderedHTMLCommon ol ol ol ol {
  list-style: lower-roman;
}

.jp-RenderedHTMLCommon ol ol ol ol ol {
  list-style: decimal;
}

.jp-RenderedHTMLCommon ol,
.jp-RenderedHTMLCommon ul {
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon ul ul,
.jp-RenderedHTMLCommon ul ol,
.jp-RenderedHTMLCommon ol ul,
.jp-RenderedHTMLCommon ol ol {
  margin-bottom: 0;
}

/* stylelint-enable selector-max-type, selector-max-compound-selectors */

.jp-RenderedHTMLCommon hr {
  color: var(--jp-border-color2);
  background-color: var(--jp-border-color1);
  margin-top: 1em;
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon > pre {
  margin: 1.5em 2em;
}

.jp-RenderedHTMLCommon pre,
.jp-RenderedHTMLCommon code {
  border: 0;
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
  font-family: var(--jp-code-font-family);
  font-size: inherit;
  line-height: var(--jp-code-line-height);
  padding: 0;
  white-space: pre-wrap;
}

.jp-RenderedHTMLCommon :not(pre) > code {
  background-color: var(--jp-layout-color2);
  padding: 1px 5px;
}

/* Tables */

.jp-RenderedHTMLCommon table {
  border-collapse: collapse;
  border-spacing: 0;
  border: none;
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  table-layout: fixed;
  margin-left: auto;
  margin-bottom: 1em;
  margin-right: auto;
}

.jp-RenderedHTMLCommon thead {
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  vertical-align: bottom;
}

.jp-RenderedHTMLCommon td,
.jp-RenderedHTMLCommon th,
.jp-RenderedHTMLCommon tr {
  vertical-align: middle;
  padding: 0.5em;
  line-height: normal;
  white-space: normal;
  max-width: none;
  border: none;
}

.jp-RenderedMarkdown.jp-RenderedHTMLCommon td,
.jp-RenderedMarkdown.jp-RenderedHTMLCommon th {
  max-width: none;
}

:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon td,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon th,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon tr {
  text-align: right;
}

.jp-RenderedHTMLCommon th {
  font-weight: bold;
}

.jp-RenderedHTMLCommon tbody tr:nth-child(odd) {
  background: var(--jp-layout-color0);
}

.jp-RenderedHTMLCommon tbody tr:nth-child(even) {
  background: var(--jp-rendermime-table-row-background);
}

.jp-RenderedHTMLCommon tbody tr:hover {
  background: var(--jp-rendermime-table-row-hover-background);
}

.jp-RenderedHTMLCommon p {
  text-align: left;
  margin: 0;
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon img {
  -moz-force-broken-image-icon: 1;
}

/* Restrict to direct children as other images could be nested in other content. */
.jp-RenderedHTMLCommon > img {
  display: block;
  margin-left: 0;
  margin-right: 0;
  margin-bottom: 1em;
}

/* Change color behind transparent images if they need it... */
[data-jp-theme-light='false'] .jp-RenderedImage img.jp-needs-light-background {
  background-color: var(--jp-inverse-layout-color1);
}

[data-jp-theme-light='true'] .jp-RenderedImage img.jp-needs-dark-background {
  background-color: var(--jp-inverse-layout-color1);
}

.jp-RenderedHTMLCommon img,
.jp-RenderedImage img,
.jp-RenderedHTMLCommon svg,
.jp-RenderedSVG svg {
  max-width: 100%;
  height: auto;
}

.jp-RenderedHTMLCommon img.jp-mod-unconfined,
.jp-RenderedImage img.jp-mod-unconfined,
.jp-RenderedHTMLCommon svg.jp-mod-unconfined,
.jp-RenderedSVG svg.jp-mod-unconfined {
  max-width: none;
}

.jp-RenderedHTMLCommon .alert {
  padding: var(--jp-notebook-padding);
  border: var(--jp-border-width) solid transparent;
  border-radius: var(--jp-border-radius);
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon .alert-info {
  color: var(--jp-info-color0);
  background-color: var(--jp-info-color3);
  border-color: var(--jp-info-color2);
}

.jp-RenderedHTMLCommon .alert-info hr {
  border-color: var(--jp-info-color3);
}

.jp-RenderedHTMLCommon .alert-info > p:last-child,
.jp-RenderedHTMLCommon .alert-info > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-warning {
  color: var(--jp-warn-color0);
  background-color: var(--jp-warn-color3);
  border-color: var(--jp-warn-color2);
}

.jp-RenderedHTMLCommon .alert-warning hr {
  border-color: var(--jp-warn-color3);
}

.jp-RenderedHTMLCommon .alert-warning > p:last-child,
.jp-RenderedHTMLCommon .alert-warning > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-success {
  color: var(--jp-success-color0);
  background-color: var(--jp-success-color3);
  border-color: var(--jp-success-color2);
}

.jp-RenderedHTMLCommon .alert-success hr {
  border-color: var(--jp-success-color3);
}

.jp-RenderedHTMLCommon .alert-success > p:last-child,
.jp-RenderedHTMLCommon .alert-success > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-danger {
  color: var(--jp-error-color0);
  background-color: var(--jp-error-color3);
  border-color: var(--jp-error-color2);
}

.jp-RenderedHTMLCommon .alert-danger hr {
  border-color: var(--jp-error-color3);
}

.jp-RenderedHTMLCommon .alert-danger > p:last-child,
.jp-RenderedHTMLCommon .alert-danger > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon blockquote {
  margin: 1em 2em;
  padding: 0 1em;
  border-left: 5px solid var(--jp-border-color2);
}

a.jp-InternalAnchorLink {
  visibility: hidden;
  margin-left: 8px;
  color: var(--md-blue-800);
}

h1:hover .jp-InternalAnchorLink,
h2:hover .jp-InternalAnchorLink,
h3:hover .jp-InternalAnchorLink,
h4:hover .jp-InternalAnchorLink,
h5:hover .jp-InternalAnchorLink,
h6:hover .jp-InternalAnchorLink {
  visibility: visible;
}

.jp-RenderedHTMLCommon kbd {
  background-color: var(--jp-rendermime-table-row-background);
  border: 1px solid var(--jp-border-color0);
  border-bottom-color: var(--jp-border-color2);
  border-radius: 3px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
  display: inline-block;
  font-size: var(--jp-ui-font-size0);
  line-height: 1em;
  padding: 0.2em 0.5em;
}

/* Most direct children of .jp-RenderedHTMLCommon have a margin-bottom of 1.0.
 * At the bottom of cells this is a bit too much as there is also spacing
 * between cells. Going all the way to 0 gets too tight between markdown and
 * code cells.
 */
.jp-RenderedHTMLCommon > *:last-child {
  margin-bottom: 0.5em;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-cursor-backdrop {
  position: fixed;
  width: 200px;
  height: 200px;
  margin-top: -100px;
  margin-left: -100px;
  will-change: transform;
  z-index: 100;
}

.lm-mod-drag-image {
  will-change: transform;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-lineFormSearch {
  padding: 4px 12px;
  background-color: var(--jp-layout-color2);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
  font-size: var(--jp-ui-font-size1);
}

.jp-lineFormCaption {
  font-size: var(--jp-ui-font-size0);
  line-height: var(--jp-ui-font-size1);
  margin-top: 4px;
  color: var(--jp-ui-font-color0);
}

.jp-baseLineForm {
  border: none;
  border-radius: 0;
  position: absolute;
  background-size: 16px;
  background-repeat: no-repeat;
  background-position: center;
  outline: none;
}

.jp-lineFormButtonContainer {
  top: 4px;
  right: 8px;
  height: 24px;
  padding: 0 12px;
  width: 12px;
}

.jp-lineFormButtonIcon {
  top: 0;
  right: 0;
  background-color: var(--jp-brand-color1);
  height: 100%;
  width: 100%;
  box-sizing: border-box;
  padding: 4px 6px;
}

.jp-lineFormButton {
  top: 0;
  right: 0;
  background-color: transparent;
  height: 100%;
  width: 100%;
  box-sizing: border-box;
}

.jp-lineFormWrapper {
  overflow: hidden;
  padding: 0 8px;
  border: 1px solid var(--jp-border-color0);
  background-color: var(--jp-input-active-background);
  height: 22px;
}

.jp-lineFormWrapperFocusWithin {
  border: var(--jp-border-width) solid var(--md-blue-500);
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-lineFormInput {
  background: transparent;
  width: 200px;
  height: 100%;
  border: none;
  outline: none;
  color: var(--jp-ui-font-color0);
  line-height: 28px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-JSONEditor {
  display: flex;
  flex-direction: column;
  width: 100%;
}

.jp-JSONEditor-host {
  flex: 1 1 auto;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0;
  background: var(--jp-layout-color0);
  min-height: 50px;
  padding: 1px;
}

.jp-JSONEditor.jp-mod-error .jp-JSONEditor-host {
  border-color: red;
  outline-color: red;
}

.jp-JSONEditor-header {
  display: flex;
  flex: 1 0 auto;
  padding: 0 0 0 12px;
}

.jp-JSONEditor-header label {
  flex: 0 0 auto;
}

.jp-JSONEditor-commitButton {
  height: 16px;
  width: 16px;
  background-size: 18px;
  background-repeat: no-repeat;
  background-position: center;
}

.jp-JSONEditor-host.jp-mod-focused {
  background-color: var(--jp-input-active-background);
  border: 1px solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
}

.jp-Editor.jp-mod-dropTarget {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/
.jp-DocumentSearch-input {
  border: none;
  outline: none;
  color: var(--jp-ui-font-color0);
  font-size: var(--jp-ui-font-size1);
  background-color: var(--jp-layout-color0);
  font-family: var(--jp-ui-font-family);
  padding: 2px 1px;
  resize: none;
}

.jp-DocumentSearch-overlay {
  position: absolute;
  background-color: var(--jp-toolbar-background);
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  border-left: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  top: 0;
  right: 0;
  z-index: 7;
  min-width: 405px;
  padding: 2px;
  font-size: var(--jp-ui-font-size1);

  --jp-private-document-search-button-height: 20px;
}

.jp-DocumentSearch-overlay button {
  background-color: var(--jp-toolbar-background);
  outline: 0;
}

.jp-DocumentSearch-overlay button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-overlay button:active {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-overlay-row {
  display: flex;
  align-items: center;
  margin-bottom: 2px;
}

.jp-DocumentSearch-button-content {
  display: inline-block;
  cursor: pointer;
  box-sizing: border-box;
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-button-content svg {
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-input-wrapper {
  border: var(--jp-border-width) solid var(--jp-border-color0);
  display: flex;
  background-color: var(--jp-layout-color0);
  margin: 2px;
}

.jp-DocumentSearch-input-wrapper:focus-within {
  border-color: var(--jp-cell-editor-active-border-color);
}

.jp-DocumentSearch-toggle-wrapper,
.jp-DocumentSearch-button-wrapper {
  all: initial;
  overflow: hidden;
  display: inline-block;
  border: none;
  box-sizing: border-box;
}

.jp-DocumentSearch-toggle-wrapper {
  width: 14px;
  height: 14px;
}

.jp-DocumentSearch-button-wrapper {
  width: var(--jp-private-document-search-button-height);
  height: var(--jp-private-document-search-button-height);
}

.jp-DocumentSearch-toggle-wrapper:focus,
.jp-DocumentSearch-button-wrapper:focus {
  outline: var(--jp-border-width) solid
    var(--jp-cell-editor-active-border-color);
  outline-offset: -1px;
}

.jp-DocumentSearch-toggle-wrapper,
.jp-DocumentSearch-button-wrapper,
.jp-DocumentSearch-button-content:focus {
  outline: none;
}

.jp-DocumentSearch-toggle-placeholder {
  width: 5px;
}

.jp-DocumentSearch-input-button::before {
  display: block;
  padding-top: 100%;
}

.jp-DocumentSearch-input-button-off {
  opacity: var(--jp-search-toggle-off-opacity);
}

.jp-DocumentSearch-input-button-off:hover {
  opacity: var(--jp-search-toggle-hover-opacity);
}

.jp-DocumentSearch-input-button-on {
  opacity: var(--jp-search-toggle-on-opacity);
}

.jp-DocumentSearch-index-counter {
  padding-left: 10px;
  padding-right: 10px;
  user-select: none;
  min-width: 35px;
  display: inline-block;
}

.jp-DocumentSearch-up-down-wrapper {
  display: inline-block;
  padding-right: 2px;
  margin-left: auto;
  white-space: nowrap;
}

.jp-DocumentSearch-spacer {
  margin-left: auto;
}

.jp-DocumentSearch-up-down-wrapper button {
  outline: 0;
  border: none;
  width: var(--jp-private-document-search-button-height);
  height: var(--jp-private-document-search-button-height);
  vertical-align: middle;
  margin: 1px 5px 2px;
}

.jp-DocumentSearch-up-down-button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-up-down-button:active {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-filter-button {
  border-radius: var(--jp-border-radius);
}

.jp-DocumentSearch-filter-button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-filter-button-enabled {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-filter-button-enabled:hover {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-search-options {
  padding: 0 8px;
  margin-left: 3px;
  width: 100%;
  display: grid;
  justify-content: start;
  grid-template-columns: 1fr 1fr;
  align-items: center;
  justify-items: stretch;
}

.jp-DocumentSearch-search-filter-disabled {
  color: var(--jp-ui-font-color2);
}

.jp-DocumentSearch-search-filter {
  display: flex;
  align-items: center;
  user-select: none;
}

.jp-DocumentSearch-regex-error {
  color: var(--jp-error-color0);
}

.jp-DocumentSearch-replace-button-wrapper {
  overflow: hidden;
  display: inline-block;
  box-sizing: border-box;
  border: var(--jp-border-width) solid var(--jp-border-color0);
  margin: auto 2px;
  padding: 1px 4px;
  height: calc(var(--jp-private-document-search-button-height) + 2px);
}

.jp-DocumentSearch-replace-button-wrapper:focus {
  border: var(--jp-border-width) solid var(--jp-cell-editor-active-border-color);
}

.jp-DocumentSearch-replace-button {
  display: inline-block;
  text-align: center;
  cursor: pointer;
  box-sizing: border-box;
  color: var(--jp-ui-font-color1);

  /* height - 2 * (padding of wrapper) */
  line-height: calc(var(--jp-private-document-search-button-height) - 2px);
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-replace-button:focus {
  outline: none;
}

.jp-DocumentSearch-replace-wrapper-class {
  margin-left: 14px;
  display: flex;
}

.jp-DocumentSearch-replace-toggle {
  border: none;
  background-color: var(--jp-toolbar-background);
  border-radius: var(--jp-border-radius);
}

.jp-DocumentSearch-replace-toggle:hover {
  background-color: var(--jp-layout-color2);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.cm-editor {
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  border: 0;
  border-radius: 0;
  height: auto;

  /* Changed to auto to autogrow */
}

.cm-editor pre {
  padding: 0 var(--jp-code-padding);
}

.jp-CodeMirrorEditor[data-type='inline'] .cm-dialog {
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
}

.jp-CodeMirrorEditor {
  cursor: text;
}

/* When zoomed out 67% and 33% on a screen of 1440 width x 900 height */
@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .jp-CodeMirrorEditor[data-type='inline'] .cm-cursor {
    border-left: var(--jp-code-cursor-width1) solid
      var(--jp-editor-cursor-color);
  }
}

/* When zoomed out less than 33% */
@media screen and (min-width: 4320px) {
  .jp-CodeMirrorEditor[data-type='inline'] .cm-cursor {
    border-left: var(--jp-code-cursor-width2) solid
      var(--jp-editor-cursor-color);
  }
}

.cm-editor.jp-mod-readOnly .cm-cursor {
  display: none;
}

.jp-CollaboratorCursor {
  border-left: 5px solid transparent;
  border-right: 5px solid transparent;
  border-top: none;
  border-bottom: 3px solid;
  background-clip: content-box;
  margin-left: -5px;
  margin-right: -5px;
}

.cm-searching,
.cm-searching span {
  /* `.cm-searching span`: we need to override syntax highlighting */
  background-color: var(--jp-search-unselected-match-background-color);
  color: var(--jp-search-unselected-match-color);
}

.cm-searching::selection,
.cm-searching span::selection {
  background-color: var(--jp-search-unselected-match-background-color);
  color: var(--jp-search-unselected-match-color);
}

.jp-current-match > .cm-searching,
.jp-current-match > .cm-searching span,
.cm-searching > .jp-current-match,
.cm-searching > .jp-current-match span {
  background-color: var(--jp-search-selected-match-background-color);
  color: var(--jp-search-selected-match-color);
}

.jp-current-match > .cm-searching::selection,
.cm-searching > .jp-current-match::selection,
.jp-current-match > .cm-searching span::selection {
  background-color: var(--jp-search-selected-match-background-color);
  color: var(--jp-search-selected-match-color);
}

.cm-trailingspace {
  background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAgAAAAFCAYAAAB4ka1VAAAAsElEQVQIHQGlAFr/AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA7+r3zKmT0/+pk9P/7+r3zAAAAAAAAAAABAAAAAAAAAAA6OPzM+/q9wAAAAAA6OPzMwAAAAAAAAAAAgAAAAAAAAAAGR8NiRQaCgAZIA0AGR8NiQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAQyoYJ/SY80UAAAAASUVORK5CYII=);
  background-position: center left;
  background-repeat: repeat-x;
}

.jp-CollaboratorCursor-hover {
  position: absolute;
  z-index: 1;
  transform: translateX(-50%);
  color: white;
  border-radius: 3px;
  padding-left: 4px;
  padding-right: 4px;
  padding-top: 1px;
  padding-bottom: 1px;
  text-align: center;
  font-size: var(--jp-ui-font-size1);
  white-space: nowrap;
}

.jp-CodeMirror-ruler {
  border-left: 1px dashed var(--jp-border-color2);
}

/* Styles for shared cursors (remote cursor locations and selected ranges) */
.jp-CodeMirrorEditor .cm-ySelectionCaret {
  position: relative;
  border-left: 1px solid black;
  margin-left: -1px;
  margin-right: -1px;
  box-sizing: border-box;
}

.jp-CodeMirrorEditor .cm-ySelectionCaret > .cm-ySelectionInfo {
  white-space: nowrap;
  position: absolute;
  top: -1.15em;
  padding-bottom: 0.05em;
  left: -1px;
  font-size: 0.95em;
  font-family: var(--jp-ui-font-family);
  font-weight: bold;
  line-height: normal;
  user-select: none;
  color: white;
  padding-left: 2px;
  padding-right: 2px;
  z-index: 101;
  transition: opacity 0.3s ease-in-out;
}

.jp-CodeMirrorEditor .cm-ySelectionInfo {
  transition-delay: 0.7s;
  opacity: 0;
}

.jp-CodeMirrorEditor .cm-ySelectionCaret:hover > .cm-ySelectionInfo {
  opacity: 1;
  transition-delay: 0s;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-MimeDocument {
  outline: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-filebrowser-button-height: 28px;
  --jp-private-filebrowser-button-width: 48px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-FileBrowser .jp-SidePanel-content {
  display: flex;
  flex-direction: column;
}

.jp-FileBrowser-toolbar.jp-Toolbar {
  flex-wrap: wrap;
  row-gap: 12px;
  border-bottom: none;
  height: auto;
  margin: 8px 12px 0;
  box-shadow: none;
  padding: 0;
  justify-content: flex-start;
}

.jp-FileBrowser-Panel {
  flex: 1 1 auto;
  display: flex;
  flex-direction: column;
}

.jp-BreadCrumbs {
  flex: 0 0 auto;
  margin: 8px 12px;
}

.jp-BreadCrumbs-item {
  margin: 0 2px;
  padding: 0 2px;
  border-radius: var(--jp-border-radius);
  cursor: pointer;
}

.jp-BreadCrumbs-item:hover {
  background-color: var(--jp-layout-color2);
}

.jp-BreadCrumbs-item:first-child {
  margin-left: 0;
}

.jp-BreadCrumbs-item.jp-mod-dropTarget {
  background-color: var(--jp-brand-color2);
  opacity: 0.7;
}

/*-----------------------------------------------------------------------------
| Buttons
|----------------------------------------------------------------------------*/

.jp-FileBrowser-toolbar > .jp-Toolbar-item {
  flex: 0 0 auto;
  padding-left: 0;
  padding-right: 2px;
  align-items: center;
  height: unset;
}

.jp-FileBrowser-toolbar > .jp-Toolbar-item .jp-ToolbarButtonComponent {
  width: 40px;
}

/*-----------------------------------------------------------------------------
| Other styles
|----------------------------------------------------------------------------*/

.jp-FileDialog.jp-mod-conflict input {
  color: var(--jp-error-color1);
}

.jp-FileDialog .jp-new-name-title {
  margin-top: 12px;
}

.jp-LastModified-hidden {
  display: none;
}

.jp-FileSize-hidden {
  display: none;
}

.jp-FileBrowser .lm-AccordionPanel > h3:first-child {
  display: none;
}

/*-----------------------------------------------------------------------------
| DirListing
|----------------------------------------------------------------------------*/

.jp-DirListing {
  flex: 1 1 auto;
  display: flex;
  flex-direction: column;
  outline: 0;
}

.jp-DirListing-header {
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  align-items: center;
  overflow: hidden;
  border-top: var(--jp-border-width) solid var(--jp-border-color2);
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
}

.jp-DirListing-headerItem {
  padding: 4px 12px 2px;
  font-weight: 500;
}

.jp-DirListing-headerItem:hover {
  background: var(--jp-layout-color2);
}

.jp-DirListing-headerItem.jp-id-name {
  flex: 1 0 84px;
}

.jp-DirListing-headerItem.jp-id-modified {
  flex: 0 0 112px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
}

.jp-DirListing-headerItem.jp-id-filesize {
  flex: 0 0 75px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
}

.jp-id-narrow {
  display: none;
  flex: 0 0 5px;
  padding: 4px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
  color: var(--jp-border-color2);
}

.jp-DirListing-narrow .jp-id-narrow {
  display: block;
}

.jp-DirListing-narrow .jp-id-modified,
.jp-DirListing-narrow .jp-DirListing-itemModified {
  display: none;
}

.jp-DirListing-headerItem.jp-mod-selected {
  font-weight: 600;
}

/* increase specificity to override bundled default */
.jp-DirListing-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  list-style-type: none;
  overflow: auto;
  background-color: var(--jp-layout-color1);
}

.jp-DirListing-content mark {
  color: var(--jp-ui-font-color0);
  background-color: transparent;
  font-weight: bold;
}

.jp-DirListing-content .jp-DirListing-item.jp-mod-selected mark {
  color: var(--jp-ui-inverse-font-color0);
}

/* Style the directory listing content when a user drops a file to upload */
.jp-DirListing.jp-mod-native-drop .jp-DirListing-content {
  outline: 5px dashed rgba(128, 128, 128, 0.5);
  outline-offset: -10px;
  cursor: copy;
}

.jp-DirListing-item {
  display: flex;
  flex-direction: row;
  align-items: center;
  padding: 4px 12px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-DirListing-checkboxWrapper {
  /* Increases hit area of checkbox. */
  padding: 4px;
}

.jp-DirListing-header
  .jp-DirListing-checkboxWrapper
  + .jp-DirListing-headerItem {
  padding-left: 4px;
}

.jp-DirListing-content .jp-DirListing-checkboxWrapper {
  position: relative;
  left: -4px;
  margin: -4px 0 -4px -8px;
}

.jp-DirListing-checkboxWrapper.jp-mod-visible {
  visibility: visible;
}

/* For devices that support hovering, hide checkboxes until hovered, selected...
*/
@media (hover: hover) {
  .jp-DirListing-checkboxWrapper {
    visibility: hidden;
  }

  .jp-DirListing-item:hover .jp-DirListing-checkboxWrapper,
  .jp-DirListing-item.jp-mod-selected .jp-DirListing-checkboxWrapper {
    visibility: visible;
  }
}

.jp-DirListing-item[data-is-dot] {
  opacity: 75%;
}

.jp-DirListing-item.jp-mod-selected {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.jp-DirListing-item.jp-mod-dropTarget {
  background: var(--jp-brand-color3);
}

.jp-DirListing-item:hover:not(.jp-mod-selected) {
  background: var(--jp-layout-color2);
}

.jp-DirListing-itemIcon {
  flex: 0 0 20px;
  margin-right: 4px;
}

.jp-DirListing-itemText {
  flex: 1 0 64px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  user-select: none;
}

.jp-DirListing-itemText:focus {
  outline-width: 2px;
  outline-color: var(--jp-inverse-layout-color1);
  outline-style: solid;
  outline-offset: 1px;
}

.jp-DirListing-item.jp-mod-selected .jp-DirListing-itemText:focus {
  outline-color: var(--jp-layout-color1);
}

.jp-DirListing-itemModified {
  flex: 0 0 125px;
  text-align: right;
}

.jp-DirListing-itemFileSize {
  flex: 0 0 90px;
  text-align: right;
}

.jp-DirListing-editor {
  flex: 1 0 64px;
  outline: none;
  border: none;
  color: var(--jp-ui-font-color1);
  background-color: var(--jp-layout-color1);
}

.jp-DirListing-item.jp-mod-running .jp-DirListing-itemIcon::before {
  color: var(--jp-success-color1);
  content: '\25CF';
  font-size: 8px;
  position: absolute;
  left: -8px;
}

.jp-DirListing-item.jp-mod-running.jp-mod-selected
  .jp-DirListing-itemIcon::before {
  color: var(--jp-ui-inverse-font-color1);
}

.jp-DirListing-item.lm-mod-drag-image,
.jp-DirListing-item.jp-mod-selected.lm-mod-drag-image {
  font-size: var(--jp-ui-font-size1);
  padding-left: 4px;
  margin-left: 4px;
  width: 160px;
  background-color: var(--jp-ui-inverse-font-color2);
  box-shadow: var(--jp-elevation-z2);
  border-radius: 0;
  color: var(--jp-ui-font-color1);
  transform: translateX(-40%) translateY(-58%);
}

.jp-Document {
  min-width: 120px;
  min-height: 120px;
  outline: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Main OutputArea
| OutputArea has a list of Outputs
|----------------------------------------------------------------------------*/

.jp-OutputArea {
  overflow-y: auto;
}

.jp-OutputArea-child {
  display: table;
  table-layout: fixed;
  width: 100%;
  overflow: hidden;
}

.jp-OutputPrompt {
  width: var(--jp-cell-prompt-width);
  color: var(--jp-cell-outprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
  opacity: var(--jp-cell-prompt-opacity);

  /* Right align prompt text, don't wrap to handle large prompt numbers */
  text-align: right;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;

  /* Disable text selection */
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-OutputArea-prompt {
  display: table-cell;
  vertical-align: top;
}

.jp-OutputArea-output {
  display: table-cell;
  width: 100%;
  height: auto;
  overflow: auto;
  user-select: text;
  -moz-user-select: text;
  -webkit-user-select: text;
  -ms-user-select: text;
}

.jp-OutputArea .jp-RenderedText {
  padding-left: 1ch;
}

/**
 * Prompt overlay.
 */

.jp-OutputArea-promptOverlay {
  position: absolute;
  top: 0;
  width: var(--jp-cell-prompt-width);
  height: 100%;
  opacity: 0.5;
}

.jp-OutputArea-promptOverlay:hover {
  background: var(--jp-layout-color2);
  box-shadow: inset 0 0 1px var(--jp-inverse-layout-color0);
  cursor: zoom-out;
}

.jp-mod-outputsScrolled .jp-OutputArea-promptOverlay:hover {
  cursor: zoom-in;
}

/**
 * Isolated output.
 */
.jp-OutputArea-output.jp-mod-isolated {
  width: 100%;
  display: block;
}

/*
When drag events occur, `lm-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated {
  position: relative;
}

body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

/* pre */

.jp-OutputArea-output pre {
  border: none;
  margin: 0;
  padding: 0;
  overflow-x: auto;
  overflow-y: auto;
  word-break: break-all;
  word-wrap: break-word;
  white-space: pre-wrap;
}

/* tables */

.jp-OutputArea-output.jp-RenderedHTMLCommon table {
  margin-left: 0;
  margin-right: 0;
}

/* description lists */

.jp-OutputArea-output dl,
.jp-OutputArea-output dt,
.jp-OutputArea-output dd {
  display: block;
}

.jp-OutputArea-output dl {
  width: 100%;
  overflow: hidden;
  padding: 0;
  margin: 0;
}

.jp-OutputArea-output dt {
  font-weight: bold;
  float: left;
  width: 20%;
  padding: 0;
  margin: 0;
}

.jp-OutputArea-output dd {
  float: left;
  width: 80%;
  padding: 0;
  margin: 0;
}

.jp-TrimmedOutputs pre {
  background: var(--jp-layout-color3);
  font-size: calc(var(--jp-code-font-size) * 1.4);
  text-align: center;
  text-transform: uppercase;
}

/* Hide the gutter in case of
 *  - nested output areas (e.g. in the case of output widgets)
 *  - mirrored output areas
 */
.jp-OutputArea .jp-OutputArea .jp-OutputArea-prompt {
  display: none;
}

/* Hide empty lines in the output area, for instance due to cleared widgets */
.jp-OutputArea-prompt:empty {
  padding: 0;
  border: 0;
}

/*-----------------------------------------------------------------------------
| executeResult is added to any Output-result for the display of the object
| returned by a cell
|----------------------------------------------------------------------------*/

.jp-OutputArea-output.jp-OutputArea-executeResult {
  margin-left: 0;
  width: 100%;
}

/* Text output with the Out[] prompt needs a top padding to match the
 * alignment of the Out[] prompt itself.
 */
.jp-OutputArea-executeResult .jp-RenderedText.jp-OutputArea-output {
  padding-top: var(--jp-code-padding);
  border-top: var(--jp-border-width) solid transparent;
}

/*-----------------------------------------------------------------------------
| The Stdin output
|----------------------------------------------------------------------------*/

.jp-Stdin-prompt {
  color: var(--jp-content-font-color0);
  padding-right: var(--jp-code-padding);
  vertical-align: baseline;
  flex: 0 0 auto;
}

.jp-Stdin-input {
  font-family: var(--jp-code-font-family);
  font-size: inherit;
  color: inherit;
  background-color: inherit;
  width: 42%;
  min-width: 200px;

  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;

  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0 0.25em;
  margin: 0 0.25em;
  flex: 0 0 70%;
}

.jp-Stdin-input::placeholder {
  opacity: 0;
}

.jp-Stdin-input:focus {
  box-shadow: none;
}

.jp-Stdin-input:focus::placeholder {
  opacity: 1;
}

/*-----------------------------------------------------------------------------
| Output Area View
|----------------------------------------------------------------------------*/

.jp-LinkedOutputView .jp-OutputArea {
  height: 100%;
  display: block;
}

.jp-LinkedOutputView .jp-OutputArea-output:only-child {
  height: 100%;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

@media print {
  .jp-OutputArea-child {
    break-inside: avoid-page;
  }
}

/*-----------------------------------------------------------------------------
| Mobile
|----------------------------------------------------------------------------*/
@media only screen and (max-width: 760px) {
  .jp-OutputPrompt {
    display: table-row;
    text-align: left;
  }

  .jp-OutputArea-child .jp-OutputArea-output {
    display: table-row;
    margin-left: var(--jp-notebook-padding);
  }
}

/* Trimmed outputs warning */
.jp-TrimmedOutputs > a {
  margin: 10px;
  text-decoration: none;
  cursor: pointer;
}

.jp-TrimmedOutputs > a:hover {
  text-decoration: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Table of Contents
|----------------------------------------------------------------------------*/

:root {
  --jp-private-toc-active-width: 4px;
}

.jp-TableOfContents {
  display: flex;
  flex-direction: column;
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  height: 100%;
}

.jp-TableOfContents-placeholder {
  text-align: center;
}

.jp-TableOfContents-placeholderContent {
  color: var(--jp-content-font-color2);
  padding: 8px;
}

.jp-TableOfContents-placeholderContent > h3 {
  margin-bottom: var(--jp-content-heading-margin-bottom);
}

.jp-TableOfContents .jp-SidePanel-content {
  overflow-y: auto;
}

.jp-TableOfContents-tree {
  margin: 4px;
}

.jp-TableOfContents ol {
  list-style-type: none;
}

/* stylelint-disable-next-line selector-max-type */
.jp-TableOfContents li > ol {
  /* Align left border with triangle icon center */
  padding-left: 11px;
}

.jp-TableOfContents-content {
  /* left margin for the active heading indicator */
  margin: 0 0 0 var(--jp-private-toc-active-width);
  padding: 0;
  background-color: var(--jp-layout-color1);
}

.jp-tocItem {
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-tocItem-heading {
  display: flex;
  cursor: pointer;
}

.jp-tocItem-heading:hover {
  background-color: var(--jp-layout-color2);
}

.jp-tocItem-content {
  display: block;
  padding: 4px 0;
  white-space: nowrap;
  text-overflow: ellipsis;
  overflow-x: hidden;
}

.jp-tocItem-collapser {
  height: 20px;
  margin: 2px 2px 0;
  padding: 0;
  background: none;
  border: none;
  cursor: pointer;
}

.jp-tocItem-collapser:hover {
  background-color: var(--jp-layout-color3);
}

/* Active heading indicator */

.jp-tocItem-heading::before {
  content: ' ';
  background: transparent;
  width: var(--jp-private-toc-active-width);
  height: 24px;
  position: absolute;
  left: 0;
  border-radius: var(--jp-border-radius);
}

.jp-tocItem-heading.jp-tocItem-active::before {
  background-color: var(--jp-brand-color1);
}

.jp-tocItem-heading:hover.jp-tocItem-active::before {
  background: var(--jp-brand-color0);
  opacity: 1;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapser {
  flex: 0 0 var(--jp-cell-collapser-width);
  padding: 0;
  margin: 0;
  border: none;
  outline: none;
  background: transparent;
  border-radius: var(--jp-border-radius);
  opacity: 1;
}

.jp-Collapser-child {
  display: block;
  width: 100%;
  box-sizing: border-box;

  /* height: 100% doesn't work because the height of its parent is computed from content */
  position: absolute;
  top: 0;
  bottom: 0;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

/*
Hiding collapsers in print mode.

Note: input and output wrappers have "display: block" propery in print mode.
*/

@media print {
  .jp-Collapser {
    display: none;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Header/Footer
|----------------------------------------------------------------------------*/

/* Hidden by zero height by default */
.jp-CellHeader,
.jp-CellFooter {
  height: 0;
  width: 100%;
  padding: 0;
  margin: 0;
  border: none;
  outline: none;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Input
|----------------------------------------------------------------------------*/

/* All input areas */
.jp-InputArea {
  display: table;
  table-layout: fixed;
  width: 100%;
  overflow: hidden;
}

.jp-InputArea-editor {
  display: table-cell;
  overflow: hidden;
  vertical-align: top;

  /* This is the non-active, default styling */
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0;
  background: var(--jp-cell-editor-background);
}

.jp-InputPrompt {
  display: table-cell;
  vertical-align: top;
  width: var(--jp-cell-prompt-width);
  color: var(--jp-cell-inprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  opacity: var(--jp-cell-prompt-opacity);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;

  /* Right align prompt text, don't wrap to handle large prompt numbers */
  text-align: right;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;

  /* Disable text selection */
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

/*-----------------------------------------------------------------------------
| Mobile
|----------------------------------------------------------------------------*/
@media only screen and (max-width: 760px) {
  .jp-InputArea-editor {
    display: table-row;
    margin-left: var(--jp-notebook-padding);
  }

  .jp-InputPrompt {
    display: table-row;
    text-align: left;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Placeholder {
  display: table;
  table-layout: fixed;
  width: 100%;
}

.jp-Placeholder-prompt {
  display: table-cell;
  box-sizing: border-box;
}

.jp-Placeholder-content {
  display: table-cell;
  padding: 4px 6px;
  border: 1px solid transparent;
  border-radius: 0;
  background: none;
  box-sizing: border-box;
  cursor: pointer;
}

.jp-Placeholder-contentContainer {
  display: flex;
}

.jp-Placeholder-content:hover,
.jp-InputPlaceholder > .jp-Placeholder-content:hover {
  border-color: var(--jp-layout-color3);
}

.jp-Placeholder-content .jp-MoreHorizIcon {
  width: 32px;
  height: 16px;
  border: 1px solid transparent;
  border-radius: var(--jp-border-radius);
}

.jp-Placeholder-content .jp-MoreHorizIcon:hover {
  border: 1px solid var(--jp-border-color1);
  box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.25);
  background-color: var(--jp-layout-color0);
}

.jp-PlaceholderText {
  white-space: nowrap;
  overflow-x: hidden;
  color: var(--jp-inverse-layout-color3);
  font-family: var(--jp-code-font-family);
}

.jp-InputPlaceholder > .jp-Placeholder-content {
  border-color: var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-cell-scrolling-output-offset: 5px;
}

/*-----------------------------------------------------------------------------
| Cell
|----------------------------------------------------------------------------*/

.jp-Cell {
  padding: var(--jp-cell-padding);
  margin: 0;
  border: none;
  outline: none;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Common input/output
|----------------------------------------------------------------------------*/

.jp-Cell-inputWrapper,
.jp-Cell-outputWrapper {
  display: flex;
  flex-direction: row;
  padding: 0;
  margin: 0;

  /* Added to reveal the box-shadow on the input and output collapsers. */
  overflow: visible;
}

/* Only input/output areas inside cells */
.jp-Cell-inputArea,
.jp-Cell-outputArea {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Collapser
|----------------------------------------------------------------------------*/

/* Make the output collapser disappear when there is not output, but do so
 * in a manner that leaves it in the layout and preserves its width.
 */
.jp-Cell.jp-mod-noOutputs .jp-Cell-outputCollapser {
  border: none !important;
  background: transparent !important;
}

.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputCollapser {
  min-height: var(--jp-cell-collapser-min-height);
}

/*-----------------------------------------------------------------------------
| Output
|----------------------------------------------------------------------------*/

/* Put a space between input and output when there IS output */
.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputWrapper {
  margin-top: 5px;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea {
  overflow-y: auto;
  max-height: 24em;
  margin-left: var(--jp-private-cell-scrolling-output-offset);
  resize: vertical;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea[style*='height'] {
  max-height: unset;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea::after {
  content: ' ';
  box-shadow: inset 0 0 6px 2px rgb(0 0 0 / 30%);
  width: 100%;
  height: 100%;
  position: sticky;
  bottom: 0;
  top: 0;
  margin-top: -50%;
  float: left;
  display: block;
  pointer-events: none;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-child {
  padding-top: 6px;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
  width: calc(
    var(--jp-cell-prompt-width) - var(--jp-private-cell-scrolling-output-offset)
  );
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-promptOverlay {
  left: calc(-1 * var(--jp-private-cell-scrolling-output-offset));
}

/*-----------------------------------------------------------------------------
| CodeCell
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| MarkdownCell
|----------------------------------------------------------------------------*/

.jp-MarkdownOutput {
  display: table-cell;
  width: 100%;
  margin-top: 0;
  margin-bottom: 0;
  padding-left: var(--jp-code-padding);
}

.jp-MarkdownOutput.jp-RenderedHTMLCommon {
  overflow: auto;
}

/* collapseHeadingButton (show always if hiddenCellsButton is _not_ shown) */
.jp-collapseHeadingButton {
  display: flex;
  min-height: var(--jp-cell-collapser-min-height);
  font-size: var(--jp-code-font-size);
  position: absolute;
  background-color: transparent;
  background-size: 25px;
  background-repeat: no-repeat;
  background-position-x: center;
  background-position-y: top;
  background-image: var(--jp-icon-caret-down);
  right: 0;
  top: 0;
  bottom: 0;
}

.jp-collapseHeadingButton.jp-mod-collapsed {
  background-image: var(--jp-icon-caret-right);
}

/*
 set the container font size to match that of content
 so that the nested collapse buttons have the right size
*/
.jp-MarkdownCell .jp-InputPrompt {
  font-size: var(--jp-content-font-size1);
}

/*
  Align collapseHeadingButton with cell top header
  The font sizes are identical to the ones in packages/rendermime/style/base.css
*/
.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='1'] {
  font-size: var(--jp-content-font-size5);
  background-position-y: calc(0.3 * var(--jp-content-font-size5));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='2'] {
  font-size: var(--jp-content-font-size4);
  background-position-y: calc(0.3 * var(--jp-content-font-size4));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='3'] {
  font-size: var(--jp-content-font-size3);
  background-position-y: calc(0.3 * var(--jp-content-font-size3));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='4'] {
  font-size: var(--jp-content-font-size2);
  background-position-y: calc(0.3 * var(--jp-content-font-size2));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='5'] {
  font-size: var(--jp-content-font-size1);
  background-position-y: top;
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='6'] {
  font-size: var(--jp-content-font-size0);
  background-position-y: top;
}

/* collapseHeadingButton (show only on (hover,active) if hiddenCellsButton is shown) */
.jp-Notebook.jp-mod-showHiddenCellsButton .jp-collapseHeadingButton {
  display: none;
}

.jp-Notebook.jp-mod-showHiddenCellsButton
  :is(.jp-MarkdownCell:hover, .jp-mod-active)
  .jp-collapseHeadingButton {
  display: flex;
}

/* showHiddenCellsButton (only show if jp-mod-showHiddenCellsButton is set, which
is a consequence of the showHiddenCellsButton option in Notebook Settings)*/
.jp-Notebook.jp-mod-showHiddenCellsButton .jp-showHiddenCellsButton {
  margin-left: calc(var(--jp-cell-prompt-width) + 2 * var(--jp-code-padding));
  margin-top: var(--jp-code-padding);
  border: 1px solid var(--jp-border-color2);
  background-color: var(--jp-border-color3) !important;
  color: var(--jp-content-font-color0) !important;
  display: flex;
}

.jp-Notebook.jp-mod-showHiddenCellsButton .jp-showHiddenCellsButton:hover {
  background-color: var(--jp-border-color2) !important;
}

.jp-showHiddenCellsButton {
  display: none;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

/*
Using block instead of flex to allow the use of the break-inside CSS property for
cell outputs.
*/

@media print {
  .jp-Cell-inputWrapper,
  .jp-Cell-outputWrapper {
    display: block;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-notebook-toolbar-padding: 2px 5px 2px 2px;
}

/*-----------------------------------------------------------------------------

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-NotebookPanel-toolbar {
  padding: var(--jp-notebook-toolbar-padding);

  /* disable paint containment from lumino 2.0 default strict CSS containment */
  contain: style size !important;
}

.jp-Toolbar-item.jp-Notebook-toolbarCellType .jp-select-wrapper.jp-mod-focused {
  border: none;
  box-shadow: none;
}

.jp-Notebook-toolbarCellTypeDropdown select {
  height: 24px;
  font-size: var(--jp-ui-font-size1);
  line-height: 14px;
  border-radius: 0;
  display: block;
}

.jp-Notebook-toolbarCellTypeDropdown span {
  top: 5px !important;
}

.jp-Toolbar-responsive-popup {
  position: absolute;
  height: fit-content;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: flex-end;
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  background: var(--jp-toolbar-background);
  min-height: var(--jp-toolbar-micro-height);
  padding: var(--jp-notebook-toolbar-padding);
  z-index: 1;
  right: 0;
  top: 0;
}

.jp-Toolbar > .jp-Toolbar-responsive-opener {
  margin-left: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-Notebook-ExecutionIndicator {
  position: relative;
  display: inline-block;
  height: 100%;
  z-index: 9997;
}

.jp-Notebook-ExecutionIndicator-tooltip {
  visibility: hidden;
  height: auto;
  width: max-content;
  width: -moz-max-content;
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color1);
  text-align: justify;
  border-radius: 6px;
  padding: 0 5px;
  position: fixed;
  display: table;
}

.jp-Notebook-ExecutionIndicator-tooltip.up {
  transform: translateX(-50%) translateY(-100%) translateY(-32px);
}

.jp-Notebook-ExecutionIndicator-tooltip.down {
  transform: translateX(calc(-100% + 16px)) translateY(5px);
}

.jp-Notebook-ExecutionIndicator-tooltip.hidden {
  display: none;
}

.jp-Notebook-ExecutionIndicator:hover .jp-Notebook-ExecutionIndicator-tooltip {
  visibility: visible;
}

.jp-Notebook-ExecutionIndicator span {
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  color: var(--jp-ui-font-color1);
  line-height: 24px;
  display: block;
}

.jp-Notebook-ExecutionIndicator-progress-bar {
  display: flex;
  justify-content: center;
  height: 100%;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*
 * Execution indicator
 */
.jp-tocItem-content::after {
  content: '';

  /* Must be identical to form a circle */
  width: 12px;
  height: 12px;
  background: none;
  border: none;
  position: absolute;
  right: 0;
}

.jp-tocItem-content[data-running='0']::after {
  border-radius: 50%;
  border: var(--jp-border-width) solid var(--jp-inverse-layout-color3);
  background: none;
}

.jp-tocItem-content[data-running='1']::after {
  border-radius: 50%;
  border: var(--jp-border-width) solid var(--jp-inverse-layout-color3);
  background-color: var(--jp-inverse-layout-color3);
}

.jp-tocItem-content[data-running='0'],
.jp-tocItem-content[data-running='1'] {
  margin-right: 12px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-Notebook-footer {
  height: 27px;
  margin-left: calc(
    var(--jp-cell-prompt-width) + var(--jp-cell-collapser-width) +
      var(--jp-cell-padding)
  );
  width: calc(
    100% -
      (
        var(--jp-cell-prompt-width) + var(--jp-cell-collapser-width) +
          var(--jp-cell-padding) + var(--jp-cell-padding)
      )
  );
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  color: var(--jp-ui-font-color3);
  margin-top: 6px;
  background: none;
  cursor: pointer;
}

.jp-Notebook-footer:focus {
  border-color: var(--jp-cell-editor-active-border-color);
}

/* For devices that support hovering, hide footer until hover */
@media (hover: hover) {
  .jp-Notebook-footer {
    opacity: 0;
  }

  .jp-Notebook-footer:focus,
  .jp-Notebook-footer:hover {
    opacity: 1;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Imports
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-side-by-side-output-size: 1fr;
  --jp-side-by-side-resized-cell: var(--jp-side-by-side-output-size);
  --jp-private-notebook-dragImage-width: 304px;
  --jp-private-notebook-dragImage-height: 36px;
  --jp-private-notebook-selected-color: var(--md-blue-400);
  --jp-private-notebook-active-color: var(--md-green-400);
}

/*-----------------------------------------------------------------------------
| Notebook
|----------------------------------------------------------------------------*/

/* stylelint-disable selector-max-class */

.jp-NotebookPanel {
  display: block;
  height: 100%;
}

.jp-NotebookPanel.jp-Document {
  min-width: 240px;
  min-height: 120px;
}

.jp-Notebook {
  padding: var(--jp-notebook-padding);
  outline: none;
  overflow: auto;
  background: var(--jp-layout-color0);
}

.jp-Notebook.jp-mod-scrollPastEnd::after {
  display: block;
  content: '';
  min-height: var(--jp-notebook-scroll-padding);
}

.jp-MainAreaWidget-ContainStrict .jp-Notebook * {
  contain: strict;
}

.jp-Notebook .jp-Cell {
  overflow: visible;
}

.jp-Notebook .jp-Cell .jp-InputPrompt {
  cursor: move;
}

/*-----------------------------------------------------------------------------
| Notebook state related styling
|
| The notebook and cells each have states, here are the possibilities:
|
| - Notebook
|   - Command
|   - Edit
| - Cell
|   - None
|   - Active (only one can be active)
|   - Selected (the cells actions are applied to)
|   - Multiselected (when multiple selected, the cursor)
|   - No outputs
|----------------------------------------------------------------------------*/

/* Command or edit modes */

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-InputPrompt {
  opacity: var(--jp-cell-prompt-not-active-opacity);
  color: var(--jp-cell-prompt-not-active-font-color);
}

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-OutputPrompt {
  opacity: var(--jp-cell-prompt-not-active-opacity);
  color: var(--jp-cell-prompt-not-active-font-color);
}

/* cell is active */
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser {
  background: var(--jp-brand-color1);
}

/* cell is dirty */
.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt {
  color: var(--jp-warn-color1);
}

.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt::before {
  color: var(--jp-warn-color1);
  content: '•';
}

.jp-Notebook .jp-Cell.jp-mod-active.jp-mod-dirty .jp-Collapser {
  background: var(--jp-warn-color1);
}

/* collapser is hovered */
.jp-Notebook .jp-Cell .jp-Collapser:hover {
  box-shadow: var(--jp-elevation-z2);
  background: var(--jp-brand-color1);
  opacity: var(--jp-cell-collapser-not-active-hover-opacity);
}

/* cell is active and collapser is hovered */
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser:hover {
  background: var(--jp-brand-color0);
  opacity: 1;
}

/* Command mode */

.jp-Notebook.jp-mod-commandMode .jp-Cell.jp-mod-selected {
  background: var(--jp-notebook-multiselected-color);
}

.jp-Notebook.jp-mod-commandMode
  .jp-Cell.jp-mod-active.jp-mod-selected:not(.jp-mod-multiSelected) {
  background: transparent;
}

/* Edit mode */

.jp-Notebook.jp-mod-editMode .jp-Cell.jp-mod-active .jp-InputArea-editor {
  border: var(--jp-border-width) solid var(--jp-cell-editor-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-cell-editor-active-background);
}

/*-----------------------------------------------------------------------------
| Notebook drag and drop
|----------------------------------------------------------------------------*/

.jp-Notebook-cell.jp-mod-dropSource {
  opacity: 0.5;
}

.jp-Notebook-cell.jp-mod-dropTarget,
.jp-Notebook.jp-mod-commandMode
  .jp-Notebook-cell.jp-mod-active.jp-mod-selected.jp-mod-dropTarget {
  border-top-color: var(--jp-private-notebook-selected-color);
  border-top-style: solid;
  border-top-width: 2px;
}

.jp-dragImage {
  display: block;
  flex-direction: row;
  width: var(--jp-private-notebook-dragImage-width);
  height: var(--jp-private-notebook-dragImage-height);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background);
  overflow: visible;
}

.jp-dragImage-singlePrompt {
  box-shadow: 2px 2px 4px 0 rgba(0, 0, 0, 0.12);
}

.jp-dragImage .jp-dragImage-content {
  flex: 1 1 auto;
  z-index: 2;
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  line-height: var(--jp-code-line-height);
  padding: var(--jp-code-padding);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background-color);
  color: var(--jp-content-font-color3);
  text-align: left;
  margin: 4px 4px 4px 0;
}

.jp-dragImage .jp-dragImage-prompt {
  flex: 0 0 auto;
  min-width: 36px;
  color: var(--jp-cell-inprompt-font-color);
  padding: var(--jp-code-padding);
  padding-left: 12px;
  font-family: var(--jp-cell-prompt-font-family);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  line-height: 1.9;
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
}

.jp-dragImage-multipleBack {
  z-index: -1;
  position: absolute;
  height: 32px;
  width: 300px;
  top: 8px;
  left: 8px;
  background: var(--jp-layout-color2);
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  box-shadow: 2px 2px 4px 0 rgba(0, 0, 0, 0.12);
}

/*-----------------------------------------------------------------------------
| Cell toolbar
|----------------------------------------------------------------------------*/

.jp-NotebookTools {
  display: block;
  min-width: var(--jp-sidebar-min-width);
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);

  /* This is needed so that all font sizing of children done in ems is
    * relative to this base size */
  font-size: var(--jp-ui-font-size1);
  overflow: auto;
}

.jp-ActiveCellTool {
  padding: 12px 0;
  display: flex;
}

.jp-ActiveCellTool-Content {
  flex: 1 1 auto;
}

.jp-ActiveCellTool .jp-ActiveCellTool-CellContent {
  background: var(--jp-cell-editor-background);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0;
  min-height: 29px;
}

.jp-ActiveCellTool .jp-InputPrompt {
  min-width: calc(var(--jp-cell-prompt-width) * 0.75);
}

.jp-ActiveCellTool-CellContent > pre {
  padding: 5px 4px;
  margin: 0;
  white-space: normal;
}

.jp-MetadataEditorTool {
  flex-direction: column;
  padding: 12px 0;
}

.jp-RankedPanel > :not(:first-child) {
  margin-top: 12px;
}

.jp-KeySelector select.jp-mod-styled {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  border: var(--jp-border-width) solid var(--jp-border-color1);
}

.jp-KeySelector label,
.jp-MetadataEditorTool label,
.jp-NumberSetter label {
  line-height: 1.4;
}

.jp-NotebookTools .jp-select-wrapper {
  margin-top: 4px;
  margin-bottom: 0;
}

.jp-NumberSetter input {
  width: 100%;
  margin-top: 4px;
}

.jp-NotebookTools .jp-Collapse {
  margin-top: 16px;
}

/*-----------------------------------------------------------------------------
| Presentation Mode (.jp-mod-presentationMode)
|----------------------------------------------------------------------------*/

.jp-mod-presentationMode .jp-Notebook {
  --jp-content-font-size1: var(--jp-content-presentation-font-size1);
  --jp-code-font-size: var(--jp-code-presentation-font-size);
}

.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-InputPrompt,
.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-OutputPrompt {
  flex: 0 0 110px;
}

/*-----------------------------------------------------------------------------
| Side-by-side Mode (.jp-mod-sideBySide)
|----------------------------------------------------------------------------*/
.jp-mod-sideBySide.jp-Notebook .jp-Notebook-cell {
  margin-top: 3em;
  margin-bottom: 3em;
  margin-left: 5%;
  margin-right: 5%;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell {
  display: grid;
  grid-template-columns: minmax(0, 1fr) min-content minmax(
      0,
      var(--jp-side-by-side-output-size)
    );
  grid-template-rows: auto minmax(0, 1fr) auto;
  grid-template-areas:
    'header header header'
    'input handle output'
    'footer footer footer';
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell.jp-mod-resizedCell {
  grid-template-columns: minmax(0, 1fr) min-content minmax(
      0,
      var(--jp-side-by-side-resized-cell)
    );
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellHeader {
  grid-area: header;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-Cell-inputWrapper {
  grid-area: input;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-Cell-outputWrapper {
  /* overwrite the default margin (no vertical separation needed in side by side move */
  margin-top: 0;
  grid-area: output;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellFooter {
  grid-area: footer;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellResizeHandle {
  grid-area: handle;
  user-select: none;
  display: block;
  height: 100%;
  cursor: ew-resize;
  padding: 0 var(--jp-cell-padding);
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellResizeHandle::after {
  content: '';
  display: block;
  background: var(--jp-border-color2);
  height: 100%;
  width: 5px;
}

.jp-mod-sideBySide.jp-Notebook
  .jp-CodeCell.jp-mod-resizedCell
  .jp-CellResizeHandle::after {
  background: var(--jp-border-color0);
}

.jp-CellResizeHandle {
  display: none;
}

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Cell-Placeholder {
  padding-left: 55px;
}

.jp-Cell-Placeholder-wrapper {
  background: #fff;
  border: 1px solid;
  border-color: #e5e6e9 #dfe0e4 #d0d1d5;
  border-radius: 4px;
  -webkit-border-radius: 4px;
  margin: 10px 15px;
}

.jp-Cell-Placeholder-wrapper-inner {
  padding: 15px;
  position: relative;
}

.jp-Cell-Placeholder-wrapper-body {
  background-repeat: repeat;
  background-size: 50% auto;
}

.jp-Cell-Placeholder-wrapper-body div {
  background: #f6f7f8;
  background-image: -webkit-linear-gradient(
    left,
    #f6f7f8 0%,
    #edeef1 20%,
    #f6f7f8 40%,
    #f6f7f8 100%
  );
  background-repeat: no-repeat;
  background-size: 800px 104px;
  height: 104px;
  position: absolute;
  right: 15px;
  left: 15px;
  top: 15px;
}

div.jp-Cell-Placeholder-h1 {
  top: 20px;
  height: 20px;
  left: 15px;
  width: 150px;
}

div.jp-Cell-Placeholder-h2 {
  left: 15px;
  top: 50px;
  height: 10px;
  width: 100px;
}

div.jp-Cell-Placeholder-content-1,
div.jp-Cell-Placeholder-content-2,
div.jp-Cell-Placeholder-content-3 {
  left: 15px;
  right: 15px;
  height: 10px;
}

div.jp-Cell-Placeholder-content-1 {
  top: 100px;
}

div.jp-Cell-Placeholder-content-2 {
  top: 120px;
}

div.jp-Cell-Placeholder-content-3 {
  top: 140px;
}

</style>
<style type="text/css">
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*
The following CSS variables define the main, public API for styling JupyterLab.
These variables should be used by all plugins wherever possible. In other
words, plugins should not define custom colors, sizes, etc unless absolutely
necessary. This enables users to change the visual theme of JupyterLab
by changing these variables.

Many variables appear in an ordered sequence (0,1,2,3). These sequences
are designed to work well together, so for example, `--jp-border-color1` should
be used with `--jp-layout-color1`. The numbers have the following meanings:

* 0: super-primary, reserved for special emphasis
* 1: primary, most important under normal situations
* 2: secondary, next most important under normal situations
* 3: tertiary, next most important under normal situations

Throughout JupyterLab, we are mostly following principles from Google's
Material Design when selecting colors. We are not, however, following
all of MD as it is not optimized for dense, information rich UIs.
*/

:root {
  /* Elevation
   *
   * We style box-shadows using Material Design's idea of elevation. These particular numbers are taken from here:
   *
   * https://github.com/material-components/material-components-web
   * https://material-components-web.appspot.com/elevation.html
   */

  --jp-shadow-base-lightness: 0;
  --jp-shadow-umbra-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.2
  );
  --jp-shadow-penumbra-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.14
  );
  --jp-shadow-ambient-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.12
  );
  --jp-elevation-z0: none;
  --jp-elevation-z1: 0 2px 1px -1px var(--jp-shadow-umbra-color),
    0 1px 1px 0 var(--jp-shadow-penumbra-color),
    0 1px 3px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z2: 0 3px 1px -2px var(--jp-shadow-umbra-color),
    0 2px 2px 0 var(--jp-shadow-penumbra-color),
    0 1px 5px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z4: 0 2px 4px -1px var(--jp-shadow-umbra-color),
    0 4px 5px 0 var(--jp-shadow-penumbra-color),
    0 1px 10px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z6: 0 3px 5px -1px var(--jp-shadow-umbra-color),
    0 6px 10px 0 var(--jp-shadow-penumbra-color),
    0 1px 18px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z8: 0 5px 5px -3px var(--jp-shadow-umbra-color),
    0 8px 10px 1px var(--jp-shadow-penumbra-color),
    0 3px 14px 2px var(--jp-shadow-ambient-color);
  --jp-elevation-z12: 0 7px 8px -4px var(--jp-shadow-umbra-color),
    0 12px 17px 2px var(--jp-shadow-penumbra-color),
    0 5px 22px 4px var(--jp-shadow-ambient-color);
  --jp-elevation-z16: 0 8px 10px -5px var(--jp-shadow-umbra-color),
    0 16px 24px 2px var(--jp-shadow-penumbra-color),
    0 6px 30px 5px var(--jp-shadow-ambient-color);
  --jp-elevation-z20: 0 10px 13px -6px var(--jp-shadow-umbra-color),
    0 20px 31px 3px var(--jp-shadow-penumbra-color),
    0 8px 38px 7px var(--jp-shadow-ambient-color);
  --jp-elevation-z24: 0 11px 15px -7px var(--jp-shadow-umbra-color),
    0 24px 38px 3px var(--jp-shadow-penumbra-color),
    0 9px 46px 8px var(--jp-shadow-ambient-color);

  /* Borders
   *
   * The following variables, specify the visual styling of borders in JupyterLab.
   */

  --jp-border-width: 1px;
  --jp-border-color0: var(--md-grey-400);
  --jp-border-color1: var(--md-grey-400);
  --jp-border-color2: var(--md-grey-300);
  --jp-border-color3: var(--md-grey-200);
  --jp-inverse-border-color: var(--md-grey-600);
  --jp-border-radius: 2px;

  /* UI Fonts
   *
   * The UI font CSS variables are used for the typography all of the JupyterLab
   * user interface elements that are not directly user generated content.
   *
   * The font sizing here is done assuming that the body font size of --jp-ui-font-size1
   * is applied to a parent element. When children elements, such as headings, are sized
   * in em all things will be computed relative to that body size.
   */

  --jp-ui-font-scale-factor: 1.2;
  --jp-ui-font-size0: 0.83333em;
  --jp-ui-font-size1: 13px; /* Base font size */
  --jp-ui-font-size2: 1.2em;
  --jp-ui-font-size3: 1.44em;
  --jp-ui-font-family: system-ui, -apple-system, blinkmacsystemfont, 'Segoe UI',
    helvetica, arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
    'Segoe UI Symbol';

  /*
   * Use these font colors against the corresponding main layout colors.
   * In a light theme, these go from dark to light.
   */

  /* Defaults use Material Design specification */
  --jp-ui-font-color0: rgba(0, 0, 0, 1);
  --jp-ui-font-color1: rgba(0, 0, 0, 0.87);
  --jp-ui-font-color2: rgba(0, 0, 0, 0.54);
  --jp-ui-font-color3: rgba(0, 0, 0, 0.38);

  /*
   * Use these against the brand/accent/warn/error colors.
   * These will typically go from light to darker, in both a dark and light theme.
   */

  --jp-ui-inverse-font-color0: rgba(255, 255, 255, 1);
  --jp-ui-inverse-font-color1: rgba(255, 255, 255, 1);
  --jp-ui-inverse-font-color2: rgba(255, 255, 255, 0.7);
  --jp-ui-inverse-font-color3: rgba(255, 255, 255, 0.5);

  /* Content Fonts
   *
   * Content font variables are used for typography of user generated content.
   *
   * The font sizing here is done assuming that the body font size of --jp-content-font-size1
   * is applied to a parent element. When children elements, such as headings, are sized
   * in em all things will be computed relative to that body size.
   */

  --jp-content-line-height: 1.6;
  --jp-content-font-scale-factor: 1.2;
  --jp-content-font-size0: 0.83333em;
  --jp-content-font-size1: 14px; /* Base font size */
  --jp-content-font-size2: 1.2em;
  --jp-content-font-size3: 1.44em;
  --jp-content-font-size4: 1.728em;
  --jp-content-font-size5: 2.0736em;

  /* This gives a magnification of about 125% in presentation mode over normal. */
  --jp-content-presentation-font-size1: 17px;
  --jp-content-heading-line-height: 1;
  --jp-content-heading-margin-top: 1.2em;
  --jp-content-heading-margin-bottom: 0.8em;
  --jp-content-heading-font-weight: 500;

  /* Defaults use Material Design specification */
  --jp-content-font-color0: rgba(0, 0, 0, 1);
  --jp-content-font-color1: rgba(0, 0, 0, 0.87);
  --jp-content-font-color2: rgba(0, 0, 0, 0.54);
  --jp-content-font-color3: rgba(0, 0, 0, 0.38);
  --jp-content-link-color: var(--md-blue-900);
  --jp-content-font-family: system-ui, -apple-system, blinkmacsystemfont,
    'Segoe UI', helvetica, arial, sans-serif, 'Apple Color Emoji',
    'Segoe UI Emoji', 'Segoe UI Symbol';

  /*
   * Code Fonts
   *
   * Code font variables are used for typography of code and other monospaces content.
   */

  --jp-code-font-size: 13px;
  --jp-code-line-height: 1.3077; /* 17px for 13px base */
  --jp-code-padding: 5px; /* 5px for 13px base, codemirror highlighting needs integer px value */
  --jp-code-font-family-default: menlo, consolas, 'DejaVu Sans Mono', monospace;
  --jp-code-font-family: var(--jp-code-font-family-default);

  /* This gives a magnification of about 125% in presentation mode over normal. */
  --jp-code-presentation-font-size: 16px;

  /* may need to tweak cursor width if you change font size */
  --jp-code-cursor-width0: 1.4px;
  --jp-code-cursor-width1: 2px;
  --jp-code-cursor-width2: 4px;

  /* Layout
   *
   * The following are the main layout colors use in JupyterLab. In a light
   * theme these would go from light to dark.
   */

  --jp-layout-color0: white;
  --jp-layout-color1: white;
  --jp-layout-color2: var(--md-grey-200);
  --jp-layout-color3: var(--md-grey-400);
  --jp-layout-color4: var(--md-grey-600);

  /* Inverse Layout
   *
   * The following are the inverse layout colors use in JupyterLab. In a light
   * theme these would go from dark to light.
   */

  --jp-inverse-layout-color0: #111;
  --jp-inverse-layout-color1: var(--md-grey-900);
  --jp-inverse-layout-color2: var(--md-grey-800);
  --jp-inverse-layout-color3: var(--md-grey-700);
  --jp-inverse-layout-color4: var(--md-grey-600);

  /* Brand/accent */

  --jp-brand-color0: var(--md-blue-900);
  --jp-brand-color1: var(--md-blue-700);
  --jp-brand-color2: var(--md-blue-300);
  --jp-brand-color3: var(--md-blue-100);
  --jp-brand-color4: var(--md-blue-50);
  --jp-accent-color0: var(--md-green-900);
  --jp-accent-color1: var(--md-green-700);
  --jp-accent-color2: var(--md-green-300);
  --jp-accent-color3: var(--md-green-100);

  /* State colors (warn, error, success, info) */

  --jp-warn-color0: var(--md-orange-900);
  --jp-warn-color1: var(--md-orange-700);
  --jp-warn-color2: var(--md-orange-300);
  --jp-warn-color3: var(--md-orange-100);
  --jp-error-color0: var(--md-red-900);
  --jp-error-color1: var(--md-red-700);
  --jp-error-color2: var(--md-red-300);
  --jp-error-color3: var(--md-red-100);
  --jp-success-color0: var(--md-green-900);
  --jp-success-color1: var(--md-green-700);
  --jp-success-color2: var(--md-green-300);
  --jp-success-color3: var(--md-green-100);
  --jp-info-color0: var(--md-cyan-900);
  --jp-info-color1: var(--md-cyan-700);
  --jp-info-color2: var(--md-cyan-300);
  --jp-info-color3: var(--md-cyan-100);

  /* Cell specific styles */

  --jp-cell-padding: 5px;
  --jp-cell-collapser-width: 8px;
  --jp-cell-collapser-min-height: 20px;
  --jp-cell-collapser-not-active-hover-opacity: 0.6;
  --jp-cell-editor-background: var(--md-grey-100);
  --jp-cell-editor-border-color: var(--md-grey-300);
  --jp-cell-editor-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-cell-editor-active-background: var(--jp-layout-color0);
  --jp-cell-editor-active-border-color: var(--jp-brand-color1);
  --jp-cell-prompt-width: 64px;
  --jp-cell-prompt-font-family: var(--jp-code-font-family-default);
  --jp-cell-prompt-letter-spacing: 0;
  --jp-cell-prompt-opacity: 1;
  --jp-cell-prompt-not-active-opacity: 0.5;
  --jp-cell-prompt-not-active-font-color: var(--md-grey-700);

  /* A custom blend of MD grey and blue 600
   * See https://meyerweb.com/eric/tools/color-blend/#546E7A:1E88E5:5:hex */
  --jp-cell-inprompt-font-color: #307fc1;

  /* A custom blend of MD grey and orange 600
   * https://meyerweb.com/eric/tools/color-blend/#546E7A:F4511E:5:hex */
  --jp-cell-outprompt-font-color: #bf5b3d;

  /* Notebook specific styles */

  --jp-notebook-padding: 10px;
  --jp-notebook-select-background: var(--jp-layout-color1);
  --jp-notebook-multiselected-color: var(--md-blue-50);

  /* The scroll padding is calculated to fill enough space at the bottom of the
  notebook to show one single-line cell (with appropriate padding) at the top
  when the notebook is scrolled all the way to the bottom. We also subtract one
  pixel so that no scrollbar appears if we have just one single-line cell in the
  notebook. This padding is to enable a 'scroll past end' feature in a notebook.
  */
  --jp-notebook-scroll-padding: calc(
    100% - var(--jp-code-font-size) * var(--jp-code-line-height) -
      var(--jp-code-padding) - var(--jp-cell-padding) - 1px
  );

  /* Rendermime styles */

  --jp-rendermime-error-background: #fdd;
  --jp-rendermime-table-row-background: var(--md-grey-100);
  --jp-rendermime-table-row-hover-background: var(--md-light-blue-50);

  /* Dialog specific styles */

  --jp-dialog-background: rgba(0, 0, 0, 0.25);

  /* Console specific styles */

  --jp-console-padding: 10px;

  /* Toolbar specific styles */

  --jp-toolbar-border-color: var(--jp-border-color1);
  --jp-toolbar-micro-height: 8px;
  --jp-toolbar-background: var(--jp-layout-color1);
  --jp-toolbar-box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.24);
  --jp-toolbar-header-margin: 4px 4px 0 4px;
  --jp-toolbar-active-background: var(--md-grey-300);

  /* Statusbar specific styles */

  --jp-statusbar-height: 24px;

  /* Input field styles */

  --jp-input-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-input-active-background: var(--jp-layout-color1);
  --jp-input-hover-background: var(--jp-layout-color1);
  --jp-input-background: var(--md-grey-100);
  --jp-input-border-color: var(--jp-inverse-border-color);
  --jp-input-active-border-color: var(--jp-brand-color1);
  --jp-input-active-box-shadow-color: rgba(19, 124, 189, 0.3);

  /* General editor styles */

  --jp-editor-selected-background: #d9d9d9;
  --jp-editor-selected-focused-background: #d7d4f0;
  --jp-editor-cursor-color: var(--jp-ui-font-color0);

  /* Code mirror specific styles */

  --jp-mirror-editor-keyword-color: #008000;
  --jp-mirror-editor-atom-color: #88f;
  --jp-mirror-editor-number-color: #080;
  --jp-mirror-editor-def-color: #00f;
  --jp-mirror-editor-variable-color: var(--md-grey-900);
  --jp-mirror-editor-variable-2-color: rgb(0, 54, 109);
  --jp-mirror-editor-variable-3-color: #085;
  --jp-mirror-editor-punctuation-color: #05a;
  --jp-mirror-editor-property-color: #05a;
  --jp-mirror-editor-operator-color: #a2f;
  --jp-mirror-editor-comment-color: #408080;
  --jp-mirror-editor-string-color: #ba2121;
  --jp-mirror-editor-string-2-color: #708;
  --jp-mirror-editor-meta-color: #a2f;
  --jp-mirror-editor-qualifier-color: #555;
  --jp-mirror-editor-builtin-color: #008000;
  --jp-mirror-editor-bracket-color: #997;
  --jp-mirror-editor-tag-color: #170;
  --jp-mirror-editor-attribute-color: #00c;
  --jp-mirror-editor-header-color: blue;
  --jp-mirror-editor-quote-color: #090;
  --jp-mirror-editor-link-color: #00c;
  --jp-mirror-editor-error-color: #f00;
  --jp-mirror-editor-hr-color: #999;

  /*
    RTC user specific colors.
    These colors are used for the cursor, username in the editor,
    and the icon of the user.
  */

  --jp-collaborator-color1: #ffad8e;
  --jp-collaborator-color2: #dac83d;
  --jp-collaborator-color3: #72dd76;
  --jp-collaborator-color4: #00e4d0;
  --jp-collaborator-color5: #45d4ff;
  --jp-collaborator-color6: #e2b1ff;
  --jp-collaborator-color7: #ff9de6;

  /* Vega extension styles */

  --jp-vega-background: white;

  /* Sidebar-related styles */

  --jp-sidebar-min-width: 250px;

  /* Search-related styles */

  --jp-search-toggle-off-opacity: 0.5;
  --jp-search-toggle-hover-opacity: 0.8;
  --jp-search-toggle-on-opacity: 1;
  --jp-search-selected-match-background-color: rgb(245, 200, 0);
  --jp-search-selected-match-color: black;
  --jp-search-unselected-match-background-color: var(
    --jp-inverse-layout-color0
  );
  --jp-search-unselected-match-color: var(--jp-ui-inverse-font-color0);

  /* Icon colors that work well with light or dark backgrounds */
  --jp-icon-contrast-color0: var(--md-purple-600);
  --jp-icon-contrast-color1: var(--md-green-600);
  --jp-icon-contrast-color2: var(--md-pink-600);
  --jp-icon-contrast-color3: var(--md-blue-600);

  /* Button colors */
  --jp-accept-color-normal: var(--md-blue-700);
  --jp-accept-color-hover: var(--md-blue-800);
  --jp-accept-color-active: var(--md-blue-900);
  --jp-warn-color-normal: var(--md-red-700);
  --jp-warn-color-hover: var(--md-red-800);
  --jp-warn-color-active: var(--md-red-900);
  --jp-reject-color-normal: var(--md-grey-600);
  --jp-reject-color-hover: var(--md-grey-700);
  --jp-reject-color-active: var(--md-grey-800);

  /* File or activity icons and switch semantic variables */
  --jp-jupyter-icon-color: #f37626;
  --jp-notebook-icon-color: #f37626;
  --jp-json-icon-color: var(--md-orange-700);
  --jp-console-icon-background-color: var(--md-blue-700);
  --jp-console-icon-color: white;
  --jp-terminal-icon-background-color: var(--md-grey-800);
  --jp-terminal-icon-color: var(--md-grey-200);
  --jp-text-editor-icon-color: var(--md-grey-700);
  --jp-inspector-icon-color: var(--md-grey-700);
  --jp-switch-color: var(--md-grey-400);
  --jp-switch-true-position-color: var(--md-orange-900);
}
</style>
<style type="text/css">
/* Force rendering true colors when outputing to pdf */
* {
  -webkit-print-color-adjust: exact;
}

/* Misc */
a.anchor-link {
  display: none;
}

/* Input area styling */
.jp-InputArea {
  overflow: hidden;
}

.jp-InputArea-editor {
  overflow: hidden;
}

.cm-editor.cm-s-jupyter .highlight pre {
/* weird, but --jp-code-padding defined to be 5px but 4px horizontal padding is hardcoded for pre.cm-line */
  padding: var(--jp-code-padding) 4px;
  margin: 0;

  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
  color: inherit;

}

.jp-OutputArea-output pre {
  line-height: inherit;
  font-family: inherit;
}

.jp-RenderedText pre {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-code-font-size);
}

/* Hiding the collapser by default */
.jp-Collapser {
  display: none;
}

@page {
    margin: 0.5in; /* Margin for each printed piece of paper */
}

@media print {
  .jp-Cell-inputWrapper,
  .jp-Cell-outputWrapper {
    display: block;
  }
}
</style>
<!-- Load mathjax -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"> </script>
<!-- MathJax configuration -->
<script type="text/x-mathjax-config">
    init_mathjax = function() {
        if (window.MathJax) {
        // MathJax loaded
            MathJax.Hub.Config({
                TeX: {
                    equationNumbers: {
                    autoNumber: "AMS",
                    useLabelIds: true
                    }
                },
                tex2jax: {
                    inlineMath: [ ['$','$'], ["\\(","\\)"] ],
                    displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
                    processEscapes: true,
                    processEnvironments: true
                },
                displayAlign: 'center',
                CommonHTML: {
                    linebreaks: {
                    automatic: true
                    }
                }
            });

            MathJax.Hub.Queue(["Typeset", MathJax.Hub]);
        }
    }
    init_mathjax();
    </script>
<!-- End of mathjax configuration --><script type="module">
  document.addEventListener("DOMContentLoaded", async () => {
    const diagrams = document.querySelectorAll(".jp-Mermaid > pre.mermaid");
    // do not load mermaidjs if not needed
    if (!diagrams.length) {
      return;
    }
    const mermaid = (await import("https://cdnjs.cloudflare.com/ajax/libs/mermaid/10.5.0/mermaid.esm.min.mjs")).default;
    const parser = new DOMParser();

    mermaid.initialize({
      maxTextSize: 100000,
      startOnLoad: false,
      fontFamily: window
        .getComputedStyle(document.body)
        .getPropertyValue("--jp-ui-font-family"),
      theme: document.querySelector("body[data-jp-theme-light='true']")
        ? "default"
        : "dark",
    });

    let _nextMermaidId = 0;

    function makeMermaidImage(svg) {
      const img = document.createElement("img");
      const doc = parser.parseFromString(svg, "image/svg+xml");
      const svgEl = doc.querySelector("svg");
      const { maxWidth } = svgEl?.style || {};
      const firstTitle = doc.querySelector("title");
      const firstDesc = doc.querySelector("desc");

      img.setAttribute("src", `data:image/svg+xml,${encodeURIComponent(svg)}`);
      if (maxWidth) {
        img.width = parseInt(maxWidth);
      }
      if (firstTitle) {
        img.setAttribute("alt", firstTitle.textContent);
      }
      if (firstDesc) {
        const caption = document.createElement("figcaption");
        caption.className = "sr-only";
        caption.textContent = firstDesc.textContent;
        return [img, caption];
      }
      return [img];
    }

    async function makeMermaidError(text) {
      let errorMessage = "";
      try {
        await mermaid.parse(text);
      } catch (err) {
        errorMessage = `${err}`;
      }

      const result = document.createElement("details");
      result.className = 'jp-RenderedMermaid-Details';
      const summary = document.createElement("summary");
      summary.className = 'jp-RenderedMermaid-Summary';
      const pre = document.createElement("pre");
      const code = document.createElement("code");
      code.innerText = text;
      pre.appendChild(code);
      summary.appendChild(pre);
      result.appendChild(summary);

      const warning = document.createElement("pre");
      warning.innerText = errorMessage;
      result.appendChild(warning);
      return [result];
    }

    async function renderOneMarmaid(src) {
      const id = `jp-mermaid-${_nextMermaidId++}`;
      const parent = src.parentNode;
      let raw = src.textContent.trim();
      const el = document.createElement("div");
      el.style.visibility = "hidden";
      document.body.appendChild(el);
      let results = null;
      let output = null;
      try {
        const { svg } = await mermaid.render(id, raw, el);
        results = makeMermaidImage(svg);
        output = document.createElement("figure");
        results.map(output.appendChild, output);
      } catch (err) {
        parent.classList.add("jp-mod-warning");
        results = await makeMermaidError(raw);
        output = results[0];
      } finally {
        el.remove();
      }
      parent.classList.add("jp-RenderedMermaid");
      parent.appendChild(output);
    }

    void Promise.all([...diagrams].map(renderOneMarmaid));
  });
</script>
<style>
  .jp-Mermaid:not(.jp-RenderedMermaid) {
    display: none;
  }

  .jp-RenderedMermaid {
    overflow: auto;
    display: flex;
  }

  .jp-RenderedMermaid.jp-mod-warning {
    width: auto;
    padding: 0.5em;
    margin-top: 0.5em;
    border: var(--jp-border-width) solid var(--jp-warn-color2);
    border-radius: var(--jp-border-radius);
    color: var(--jp-ui-font-color1);
    font-size: var(--jp-ui-font-size1);
    white-space: pre-wrap;
    word-wrap: break-word;
  }

  .jp-RenderedMermaid figure {
    margin: 0;
    overflow: auto;
    max-width: 100%;
  }

  .jp-RenderedMermaid img {
    max-width: 100%;
  }

  .jp-RenderedMermaid-Details > pre {
    margin-top: 1em;
  }

  .jp-RenderedMermaid-Summary {
    color: var(--jp-warn-color2);
  }

  .jp-RenderedMermaid:not(.jp-mod-warning) pre {
    display: none;
  }

  .jp-RenderedMermaid-Summary > pre {
    display: inline-block;
    white-space: normal;
  }
</style>
<!-- End of mermaid configuration --></head>
<body class="jp-Notebook" data-jp-theme-light="true" data-jp-theme-name="JupyterLab Light">
<main><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=40915e6f-63ff-43f7-aca0-ffff5a6ebe07">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [1]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Model design</span>
<span class="kn">import</span> <span class="nn">agentpy</span> <span class="k">as</span> <span class="nn">ap</span>
<span class="kn">import</span> <span class="nn">networkx</span> <span class="k">as</span> <span class="nn">nx</span>
<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
<span class="kn">import</span> <span class="nn">random</span> 

<span class="c1"># Visualization</span>
<span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span> 
<span class="kn">import</span> <span class="nn">seaborn</span> <span class="k">as</span> <span class="nn">sns</span>
<span class="kn">import</span> <span class="nn">IPython</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=7f04a421">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Introduction">Introduction<a class="anchor-link" href="#Introduction">¶</a></h2><p>This is a very simple world model to explore the tech adoption in a population. I plan to extend this to include additional resources in the future including resources, types of AI, and community resource pooling, however this is just a start.</p>
<p>A logical place to start when modeling technology adoption is Rogers' model of innovation diffusion:</p>
<p><strong>Diffusion of Innovations (5th Edition)</strong> by Everett M. Rogers</p>
<ul>
<li><strong>Publisher</strong>: Free Press</li>
<li><strong>Year</strong>: 2003 (latest edition)</li>
<li><strong>ISBN</strong>: 978-0743222099</li>
</ul>
<p>This book is the definitive work on the subject, presenting the theory and the five stages of the diffusion process:</p>
<ol>
<li>Knowledge</li>
<li>Persuasion</li>
<li>Decision</li>
<li>Implementation</li>
<li>Confirmation</li>
</ol>
<p>Key factors affecting the adoption of innovations include:</p>
<ul>
<li><strong>Innovation attributes</strong>: Relative advantage, compatibility, complexity, trialability, and observability.</li>
<li><strong>Adopter categories</strong>: Innovators, early adopters, early majority, late majority, and laggards.</li>
</ul>
<p>The book also includes case studies and practical applications across disciplines, making it a comprehensive resource for understanding how innovations spread in societies.</p>
<p>This model will begin with a simple exploration of the adopter categories and be expanded in future iterations.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=4beadf44">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Simple-Exploration">Simple Exploration<a class="anchor-link" href="#Simple-Exploration">¶</a></h2><p>Lets start with just 2 attributes of each agent, 1) what their category is and 2) if they have adopted the technology or not.</p>
<p>I will model the category with numpy.model.choice according to a non-uniform distribution</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=47c7c196">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [2]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">categories</span> <span class="o">=</span> <span class="p">[</span><span class="s1">'innovator'</span><span class="p">,</span> <span class="s1">'early_adopter'</span><span class="p">,</span> <span class="s1">'early_majority'</span><span class="p">,</span> <span class="s1">'late_majority'</span><span class="p">,</span> <span class="s1">'laggard'</span><span class="p">]</span> <span class="c1"># tech adoption categories</span>
<span class="n">probabilities</span> <span class="o">=</span> <span class="p">[</span><span class="mf">0.05</span><span class="p">,</span> <span class="mf">0.1</span><span class="p">,</span> <span class="mf">0.35</span><span class="p">,</span> <span class="mf">0.35</span><span class="p">,</span> <span class="mf">0.15</span><span class="p">]</span> <span class="c1"># fraction of the population that falls into each category</span>
<span class="n">thresholds</span> <span class="o">=</span> <span class="p">[</span><span class="mf">0.0</span><span class="p">,</span> <span class="mf">0.3</span><span class="p">,</span> <span class="mf">0.7</span><span class="p">,</span> <span class="mf">0.8</span><span class="p">,</span> <span class="mf">0.9</span><span class="p">]</span> <span class="c1"># threshold above which fraction of adopted neighbors will cause agent to adopt</span>

<span class="n">rng</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">random</span><span class="o">.</span><span class="n">default_rng</span><span class="p">()</span>

<span class="n">samples</span> <span class="o">=</span> <span class="n">rng</span><span class="o">.</span><span class="n">choice</span><span class="p">(</span><span class="n">categories</span><span class="p">,</span> <span class="n">p</span><span class="o">=</span><span class="n">probabilities</span><span class="p">)</span>
<span class="n">samples</span>

<span class="k">def</span> <span class="nf">tech_categorical</span><span class="p">(</span><span class="n">categories</span><span class="p">,</span><span class="n">probabilities</span><span class="p">,</span><span class="n">population_size</span><span class="o">=</span><span class="mi">100</span><span class="p">,</span> <span class="n">rng</span><span class="o">=</span><span class="n">np</span><span class="o">.</span><span class="n">random</span><span class="o">.</span><span class="n">default_rng</span><span class="p">()):</span>
    <span class="n">rng</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">random</span><span class="o">.</span><span class="n">default_rng</span><span class="p">()</span>

    <span class="n">samples</span> <span class="o">=</span> <span class="n">rng</span><span class="o">.</span><span class="n">choice</span><span class="p">(</span><span class="n">categories</span><span class="p">,</span> <span class="n">size</span><span class="o">=</span><span class="n">population_size</span><span class="p">,</span><span class="n">p</span><span class="o">=</span><span class="n">probabilities</span><span class="p">)</span>
    <span class="k">return</span> <span class="n">samples</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=52ab2ac4">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Agentpy-Agent-definition">Agentpy Agent definition<a class="anchor-link" href="#Agentpy-Agent-definition">¶</a></h2><p>I will use <a href="https://agentpy.readthedocs.io/en/latest/">Agentpy</a> as my python based agent modeling framework.</p>
<p>We will start by defining the attributes and behaviour of the agent or in this case person adopting the tech.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=69cfd271">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [3]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="k">class</span> <span class="nc">InnovationAgent</span><span class="p">(</span><span class="n">ap</span><span class="o">.</span><span class="n">Agent</span><span class="p">):</span>
    <span class="k">def</span> <span class="nf">setup</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
<span class="w">        </span><span class="sd">"""</span>
<span class="sd">        Initializes the agent's adoption state and assigns it to a category based on predefined probabilities.</span>
<span class="sd">        """</span>
        <span class="c1"># Everyone starts as having not adopted the technology</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">adopted</span> <span class="o">=</span> <span class="kc">False</span>

        <span class="c1"># Select a category for the agent using the given probabilities</span>
        <span class="n">rng</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">random</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">category_idx</span> <span class="o">=</span> <span class="n">rng</span><span class="o">.</span><span class="n">choice</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">p</span><span class="o">.</span><span class="n">categories</span><span class="p">),</span> <span class="n">p</span><span class="o">=</span><span class="bp">self</span><span class="o">.</span><span class="n">p</span><span class="o">.</span><span class="n">probabilities</span><span class="p">)</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">category</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">p</span><span class="o">.</span><span class="n">categories</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">category_idx</span><span class="p">]</span>

    <span class="k">def</span> <span class="nf">num_adopted_neighbors</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
<span class="w">        </span><span class="sd">"""</span>
<span class="sd">        Calculates the number of neighboring agents who have adopted the innovation.</span>
<span class="sd">        Returns:</span>
<span class="sd">            int: The count of neighbors who have adopted.</span>
<span class="sd">        """</span>
        <span class="c1"># Get the neighbors of the current agent</span>
        <span class="n">neighbors</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">network</span><span class="o">.</span><span class="n">neighbors</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
        
        <span class="c1"># Check adoption status for each neighbor</span>
        <span class="n">adopted</span> <span class="o">=</span> <span class="p">[</span><span class="n">n</span><span class="o">.</span><span class="n">adopted</span> <span class="k">for</span> <span class="n">n</span> <span class="ow">in</span> <span class="n">neighbors</span><span class="p">]</span>
        
        <span class="c1"># Count the number of adopters</span>
        <span class="k">return</span> <span class="nb">sum</span><span class="p">(</span><span class="n">adopted</span><span class="p">)</span>

    <span class="k">def</span> <span class="nf">neighbor_adopted_frac</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
<span class="w">        </span><span class="sd">"""</span>
<span class="sd">        Calculates the fraction of neighboring agents who have adopted the innovation.</span>
<span class="sd">        Returns:</span>
<span class="sd">            float: Fraction of neighbors who have adopted, or 0 if there are no neighbors.</span>
<span class="sd">        """</span>
        <span class="c1"># Get the neighbors of the current agent</span>
        <span class="n">neighbors</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">network</span><span class="o">.</span><span class="n">neighbors</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span>
        
        <span class="c1"># Check adoption status for each neighbor</span>
        <span class="n">adopted</span> <span class="o">=</span> <span class="p">[</span><span class="n">n</span><span class="o">.</span><span class="n">adopted</span> <span class="k">for</span> <span class="n">n</span> <span class="ow">in</span> <span class="n">neighbors</span><span class="p">]</span>
        <span class="n">len_neighbors</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">adopted</span><span class="p">)</span>

        <span class="c1"># Handle case where there are no neighbors</span>
        <span class="k">if</span> <span class="n">len_neighbors</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
            <span class="k">return</span> <span class="mi">0</span>

        <span class="c1"># Calculate and return the fraction of adopters</span>
        <span class="n">num_adopters</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="n">adopted</span><span class="p">)</span>
        <span class="k">return</span> <span class="n">num_adopters</span> <span class="o">/</span> <span class="n">len_neighbors</span>

    <span class="k">def</span> <span class="nf">adopt_innovation</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
<span class="w">        </span><span class="sd">"""</span>
<span class="sd">        Determines whether the agent adopts the innovation based on its category</span>
<span class="sd">        and the adoption status of its neighbors.</span>
<span class="sd">        """</span>
        <span class="c1"># Only proceed if the agent has not already adopted the innovation</span>
        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">adopted</span><span class="p">:</span>
            <span class="c1"># Innovators adopt unconditionally</span>
            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">category</span> <span class="o">==</span> <span class="s1">'innovator'</span><span class="p">:</span>
                <span class="bp">self</span><span class="o">.</span><span class="n">adopted</span> <span class="o">=</span> <span class="kc">True</span>
            <span class="c1"># Other categories adopt based on a threshold of neighbor adoption</span>
            <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">category</span> <span class="ow">in</span> <span class="p">[</span><span class="s1">'early_adopter'</span><span class="p">,</span> <span class="s1">'early_majority'</span><span class="p">,</span> <span class="s1">'late_majority'</span><span class="p">,</span> <span class="s1">'laggard'</span><span class="p">]:</span>
                <span class="c1"># Calculate the fraction of neighbors who have adopted</span>
                <span class="n">adopted_frac</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">neighbor_adopted_frac</span><span class="p">()</span>

                <span class="c1"># Get the threshold for the agent's category</span>
                <span class="n">threshold</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">p</span><span class="o">.</span><span class="n">thresholds</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">category_idx</span><span class="p">]</span>

                <span class="c1"># Adopt if the fraction meets or exceeds the threshold</span>
                <span class="k">if</span> <span class="n">adopted_frac</span> <span class="o">&gt;=</span> <span class="n">threshold</span><span class="p">:</span>
                    <span class="bp">self</span><span class="o">.</span><span class="n">adopted</span> <span class="o">=</span> <span class="kc">True</span>
</pre></div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=e6dd0ada">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [4]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="k">class</span> <span class="nc">InnovationModel</span><span class="p">(</span><span class="n">ap</span><span class="o">.</span><span class="n">Model</span><span class="p">):</span>
<span class="w">    </span><span class="sd">"""</span>
<span class="sd">    This class represents the overall model for innovation diffusion. It manages the setup,</span>
<span class="sd">    simulation steps, and final results.</span>
<span class="sd">    """</span>

    <span class="k">def</span> <span class="nf">setup</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
<span class="w">        </span><span class="sd">"""</span>
<span class="sd">        Initializes the network and agents for the simulation. A small-world network is</span>
<span class="sd">        created using the Watts-Strogatz model, and agents are assigned to it.</span>
<span class="sd">        """</span>
        <span class="n">graph</span> <span class="o">=</span> <span class="n">nx</span><span class="o">.</span><span class="n">watts_strogatz_graph</span><span class="p">(</span>
            <span class="bp">self</span><span class="o">.</span><span class="n">p</span><span class="o">.</span><span class="n">population</span><span class="p">,</span>
            <span class="bp">self</span><span class="o">.</span><span class="n">p</span><span class="o">.</span><span class="n">number_of_connections</span><span class="p">,</span>
            <span class="bp">self</span><span class="o">.</span><span class="n">p</span><span class="o">.</span><span class="n">network_rewire_probability</span><span class="p">,</span>
        <span class="p">)</span>

        <span class="c1"># Create agents and a network</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">agents</span> <span class="o">=</span> <span class="n">ap</span><span class="o">.</span><span class="n">AgentList</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">p</span><span class="o">.</span><span class="n">population</span><span class="p">,</span> <span class="n">InnovationAgent</span><span class="p">)</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">network</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">agents</span><span class="o">.</span><span class="n">network</span> <span class="o">=</span> <span class="n">ap</span><span class="o">.</span><span class="n">Network</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">graph</span><span class="p">)</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">network</span><span class="o">.</span><span class="n">add_agents</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">agents</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">network</span><span class="o">.</span><span class="n">nodes</span><span class="p">)</span>

    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
<span class="w">        </span><span class="sd">"""</span>
<span class="sd">        Calculates the fraction of agents who have adopted the innovation and records it.</span>
<span class="sd">        Stops the simulation if all agents have adopted.</span>
<span class="sd">        """</span>
        <span class="n">frac_adopted</span> <span class="o">=</span> <span class="nb">sum</span><span class="p">(</span><span class="mi">1</span> <span class="k">for</span> <span class="n">a</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">agents</span> <span class="k">if</span> <span class="n">a</span><span class="o">.</span><span class="n">adopted</span><span class="p">)</span> <span class="o">/</span> <span class="bp">self</span><span class="o">.</span><span class="n">p</span><span class="o">.</span><span class="n">population</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">record</span><span class="p">(</span><span class="s2">"fraction adopted"</span><span class="p">,</span> <span class="n">frac_adopted</span><span class="p">)</span>

        <span class="c1"># Stop if everyone has adopted the tech</span>
        <span class="k">if</span> <span class="n">frac_adopted</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
            <span class="bp">self</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>

    <span class="k">def</span> <span class="nf">step</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
<span class="w">        </span><span class="sd">"""</span>
<span class="sd">        Executes a single step of the simulation. During each step, agents decide</span>
<span class="sd">        whether to adopt the innovation based on their category and network connections.</span>
<span class="sd">        """</span>
        <span class="k">for</span> <span class="n">agent</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">agents</span><span class="p">:</span>
            <span class="n">agent</span><span class="o">.</span><span class="n">adopt_innovation</span><span class="p">()</span> <span class="c1"># Agents adopt innovations based on their category and network connections</span>
    
    <span class="k">def</span> <span class="nf">end</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
<span class="w">        </span><span class="sd">"""</span>
<span class="sd">        Finalizes the simulation. Additional computations or outputs can be added here if needed.</span>
<span class="sd">        """</span>
        <span class="k">pass</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=727fa456-42a8-4331-a1a5-d386b89eaae7">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Running-The-Model">Running The Model<a class="anchor-link" href="#Running-The-Model">¶</a></h2><p>Now that we have the agent model and the innovation model, we can perform a simple run using the parameters below.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=4419d665">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [5]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">parameters</span> <span class="o">=</span> <span class="p">{</span>
    <span class="s1">'population'</span><span class="p">:</span> <span class="mi">100</span><span class="p">,</span>
    <span class="s2">"categories"</span><span class="p">:</span> <span class="p">[</span><span class="s1">'innovator'</span><span class="p">,</span> <span class="s1">'early_adopter'</span><span class="p">,</span> <span class="s1">'early_majority'</span><span class="p">,</span> <span class="s1">'late_majority'</span><span class="p">,</span> <span class="s1">'laggard'</span><span class="p">],</span>
    <span class="s2">"probabilities"</span><span class="p">:</span> <span class="p">[</span><span class="mf">0.05</span><span class="p">,</span> <span class="mf">0.1</span><span class="p">,</span> <span class="mf">0.35</span><span class="p">,</span> <span class="mf">0.35</span><span class="p">,</span> <span class="mf">0.15</span><span class="p">],</span>
    <span class="s2">"thresholds"</span><span class="p">:</span> <span class="p">[</span><span class="mf">0.0</span><span class="p">,</span> <span class="mf">0.1</span><span class="p">,</span> <span class="mf">0.25</span><span class="p">,</span> <span class="mf">0.5</span><span class="p">,</span> <span class="mf">0.9</span><span class="p">],</span>
    <span class="s2">"number_of_connections"</span><span class="p">:</span> <span class="mi">4</span><span class="p">,</span>
    <span class="s2">"network_rewire_probability"</span><span class="p">:</span> <span class="mf">0.1</span><span class="p">,</span>
    <span class="s2">"steps"</span><span class="p">:</span><span class="mi">100</span><span class="p">,</span>
<span class="p">}</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>Completed: 100 steps
Run time: 0:00:00.014400
Simulation finished
</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=8c9b76b2-3585-443e-880a-e45cb6842847">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Forshadowing a bit, I asked gpt4o to describe this set of parameters in terms of what they represent, and what are the benefits and drawbacks of this model in terms of realism - this is the output:</p>
<h3 id="Prompt-to-4o"><strong>Prompt to 4o</strong><a class="anchor-link" href="#Prompt-to-4o">¶</a></h3><p>tell me in words what this configuration means for our ai adoption model</p>
<pre><code>parameters = {
    'population': 100,
    "categories": ['innovator', 'early_adopter', 'early_majority', 'late_majority', 'laggard'],
    "probabilities": [0.05, 0.1, 0.35, 0.35, 0.15],
    "thresholds": [0.0, 0.1, 0.25, 0.5, 0.9],
    "number_of_connections": 4,
    "network_rewire_probability": 0.1,
    "steps":100,
}
</code></pre>
<h3 id="Output"><strong>Output</strong><a class="anchor-link" href="#Output">¶</a></h3><p>This configuration outlines the structure and dynamics of an AI adoption model, reflecting how a population adopts AI technology over time. Here's a breakdown of the parameters and their implications:</p>
<ol>
<li><p><strong><code>population</code>: 100</strong></p>
<ul>
<li>The total number of individuals in the simulation. The model assumes there are 100 entities (people, organizations, etc.) interacting within the network.</li>
</ul>
</li>
<li><p><strong><code>categories</code>: ['innovator', 'early_adopter', 'early_majority', 'late_majority', 'laggard']</strong></p>
<ul>
<li>These are the adoption categories based on the diffusion of innovations theory. Individuals are classified into groups reflecting their likelihood to adopt the AI:<ul>
<li><strong>Innovators</strong>: The earliest adopters, willing to take risks.</li>
<li><strong>Early adopters</strong>: Next in line, more cautious but still ahead of the curve.</li>
<li><strong>Early majority</strong>: A large group adopting after initial success is evident.</li>
<li><strong>Late majority</strong>: More skeptical, adopting only after widespread acceptance.</li>
<li><strong>Laggards</strong>: The last to adopt, resistant to change.</li>
</ul>
</li>
</ul>
</li>
<li><p><strong><code>probabilities</code>: [0.05, 0.1, 0.35, 0.35, 0.15]</strong></p>
<ul>
<li>These are the proportions of the population belonging to each category:<ul>
<li>5% are innovators.</li>
<li>10% are early adopters.</li>
<li>35% are in the early majority.</li>
<li>35% are in the late majority.</li>
<li>15% are laggards.</li>
</ul>
</li>
</ul>
</li>
<li><p><strong><code>thresholds</code>: [0.0, 0.1, 0.25, 0.5, 0.9]</strong></p>
<ul>
<li>Each category has a specific threshold value that determines how much influence they need from their network to adopt AI:<ul>
<li>Innovators have no threshold (0.0); they adopt immediately.</li>
<li>Early adopters adopt once they see 10% of their connections adopt.</li>
<li>Early majority need 25% of their connections to adopt.</li>
<li>Late majority need 50% of their connections to adopt.</li>
<li>Laggards require 90% of their connections to adopt.</li>
</ul>
</li>
</ul>
</li>
<li><p><strong><code>number_of_connections</code>: 4</strong></p>
<ul>
<li>Each individual in the network connects to 4 others on average. This reflects the local interaction structure, where adoption decisions are influenced by these connections.</li>
</ul>
</li>
<li><p><strong><code>network_rewire_probability</code>: 0.1</strong></p>
<ul>
<li>A 10% chance exists for a connection in the network to rewire randomly. This introduces small-world or random network features, increasing the likelihood of influence spreading more widely across the population.</li>
</ul>
</li>
<li><p><strong><code>steps</code>: 100</strong></p>
<ul>
<li>The simulation runs for 100 steps, representing the time over which adoption spreads.</li>
</ul>
</li>
</ol>
<h3 id="Summary-of-the-Model:">Summary of the Model:<a class="anchor-link" href="#Summary-of-the-Model:">¶</a></h3><p>This configuration models how a population of 100 individuals, distributed across adoption categories with specific thresholds, interacts in a network to adopt AI. Adoption begins with the innovators and spreads based on network influences and thresholds over 100 time steps. The network's structure (connections and rewiring probability) plays a significant role in determining how quickly adoption propagates.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=fe7cdf70-57d8-4bf1-a202-529012dcc29f">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="Further-Prompt"><strong>Further Prompt</strong><a class="anchor-link" href="#Further-Prompt">¶</a></h3><p>how realistic is this configuration for exploring ai technology adoption</p>
<h3 id="Response"><strong>Response</strong><a class="anchor-link" href="#Response">¶</a></h3><p>This configuration is a reasonable starting point for exploring AI technology adoption but has some limitations and simplifications. Here's an assessment of its realism and how it could be improved for better accuracy:</p>
<hr/>
<h3 id="Strengths-of-the-Configuration"><strong>Strengths of the Configuration</strong><a class="anchor-link" href="#Strengths-of-the-Configuration">¶</a></h3><ol>
<li><p><strong>Diffusion of Innovation Framework</strong></p>
<ul>
<li>The use of categories (innovator, early adopter, etc.) and adoption thresholds is consistent with established theories like Rogers' Diffusion of Innovations, making it a good conceptual foundation.</li>
</ul>
</li>
<li><p><strong>Population Distribution</strong></p>
<ul>
<li>The probabilities (e.g., 5% innovators, 35% early/late majority) align with historical observations of technology adoption curves. These proportions provide a realistic basis for modeling.</li>
</ul>
</li>
<li><p><strong>Network Effects</strong></p>
<ul>
<li>The model includes a network structure and a rewire probability, capturing how social interactions and random connections influence adoption.</li>
</ul>
</li>
<li><p><strong>Threshold-Based Behavior</strong></p>
<ul>
<li>Adoption thresholds for each category realistically mimic the varying levels of influence required to convince individuals to adopt AI.</li>
</ul>
</li>
</ol>
<hr/>
<h3 id="Limitations-of-Realism"><strong>Limitations of Realism</strong><a class="anchor-link" href="#Limitations-of-Realism">¶</a></h3><ol>
<li><p><strong>Small Population Size</strong></p>
<ul>
<li>A population of 100 is manageable for simulations but may oversimplify real-world dynamics. Larger populations with more complex structures might yield insights closer to real-world scenarios.</li>
</ul>
</li>
<li><p><strong>Fixed Number of Connections</strong></p>
<ul>
<li>A uniform number of 4 connections per individual may not capture the diversity in social or organizational networks. In reality, some entities (e.g., thought leaders or enterprises) are highly connected, while others are isolated.</li>
</ul>
</li>
<li><p><strong>Static Probabilities and Thresholds</strong></p>
<ul>
<li>The thresholds and category probabilities are fixed, but real-world behavior evolves:<ul>
<li>Thresholds may decrease over time as AI becomes more familiar or trusted.</li>
<li>Probabilities might shift due to cultural, economic, or policy changes.</li>
</ul>
</li>
</ul>
</li>
<li><p><strong>Simplified Network Rewiring</strong></p>
<ul>
<li>A 10% rewiring probability adds randomness but doesn't account for structured randomness in real-world networks, such as geographic clustering, industry focus, or social media dynamics.</li>
</ul>
</li>
<li><p><strong>No Feedback Effects</strong></p>
<ul>
<li>The model assumes adoption is influenced only by immediate connections, without accounting for external feedback like marketing, policy interventions, or mass media effects.</li>
</ul>
</li>
<li><p><strong>Single Technology Assumption</strong></p>
<ul>
<li>The model assumes a single AI technology is being adopted uniformly. In reality, different AI solutions (e.g., chatbots, predictive analytics, robotics) will have distinct adoption paths.</li>
</ul>
</li>
<li><p><strong>No Cost or Risk Considerations</strong></p>
<ul>
<li>Adoption decisions often depend on perceived costs, risks, and benefits. This model doesn't account for these factors, which are crucial in AI adoption.</li>
</ul>
</li>
</ol>
<hr/>
<h3 id="Suggestions-to-Improve-Realism"><strong>Suggestions to Improve Realism</strong><a class="anchor-link" href="#Suggestions-to-Improve-Realism">¶</a></h3><ol>
<li><p><strong>Expand Population Size and Diversity</strong></p>
<ul>
<li>Increase the population and introduce heterogeneity in demographics, industries, or geographies to mimic real-world dynamics.</li>
</ul>
</li>
<li><p><strong>Vary Connection Numbers</strong></p>
<ul>
<li>Use a distribution (e.g., power law or exponential) for connections to simulate highly connected hubs and sparsely connected nodes.</li>
</ul>
</li>
<li><p><strong>Dynamic Thresholds and Probabilities</strong></p>
<ul>
<li>Allow thresholds and category probabilities to evolve based on cumulative adoption, external events, or technological improvements.</li>
</ul>
</li>
<li><p><strong>Introduce Feedback Mechanisms</strong></p>
<ul>
<li>Add external drivers like advertising, government incentives, or media influence to simulate broader societal effects on adoption.</li>
</ul>
</li>
<li><p><strong>Multiple AI Technologies</strong></p>
<ul>
<li>Model adoption for several AI technologies, with interactions and dependencies among them.</li>
</ul>
</li>
<li><p><strong>Incorporate Cost-Benefit Analysis</strong></p>
<ul>
<li>Include factors such as costs, risks, and perceived benefits in individual adoption decisions.</li>
</ul>
</li>
<li><p><strong>Refine Network Structure</strong></p>
<ul>
<li>Use real-world-inspired network models (e.g., small-world, scale-free) to better capture how social and organizational networks function.</li>
</ul>
</li>
</ol>
<hr/>
<h3 id="Conclusion"><strong>Conclusion</strong><a class="anchor-link" href="#Conclusion">¶</a></h3><p>The configuration is a reasonable approximation for studying AI adoption in a controlled, theoretical setting. However, to make the model more realistic and applicable to real-world scenarios, enhancements such as dynamic thresholds, diverse network structures, and feedback effects are recommended.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=9b50bbdf-db78-468f-b359-89667126cac3">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Actual-Model-Run">Actual Model Run<a class="anchor-link" href="#Actual-Model-Run">¶</a></h2>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=11c28a7e-b712-43e8-8f39-32752d8122e9">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [28]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">model</span> <span class="o">=</span> <span class="n">InnovationModel</span><span class="p">(</span><span class="n">parameters</span><span class="p">)</span>
<span class="n">results</span> <span class="o">=</span> <span class="n">model</span><span class="o">.</span><span class="n">run</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>Completed: 100 steps
Run time: 0:00:00.011041
Simulation finished
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=ffd44556">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [29]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="o">%</span><span class="k">matplotlib</span> inline
<span class="n">data</span> <span class="o">=</span> <span class="n">results</span><span class="o">.</span><span class="n">variables</span><span class="o">.</span><span class="n">InnovationModel</span>
<span class="n">ax</span> <span class="o">=</span> <span class="n">data</span><span class="o">.</span><span class="n">plot</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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"/>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=b8c0c072-df88-4a50-8f84-9f6a87ed47ab">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="Interpretation">Interpretation<a class="anchor-link" href="#Interpretation">¶</a></h3><p>This shows that the fraction of total population adoption increased pretty dramatically and then plateaued at a fairly early epooch at around 89% adoption.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=54102808-4aba-4c7c-910f-089d76629243">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [30]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="o">%</span><span class="k">matplotlib</span> inline  
<span class="c1"># Enable interactive widgets for matplotlib (e.g., zooming and panning).</span>

<span class="c1"># Get the network and agent data from the model.</span>
<span class="n">network</span> <span class="o">=</span> <span class="n">model</span><span class="o">.</span><span class="n">network</span>  <span class="c1"># Retrieve the network structure from the model.</span>
<span class="n">adopted_states</span> <span class="o">=</span> <span class="p">[</span><span class="n">agent</span><span class="o">.</span><span class="n">adopted</span> <span class="k">for</span> <span class="n">agent</span> <span class="ow">in</span> <span class="n">model</span><span class="o">.</span><span class="n">agents</span><span class="p">]</span>  <span class="c1"># Extract the adoption status (True/False) for all agents.</span>

<span class="c1"># Define node colors based on the adopted parameter.</span>
<span class="c1"># Nodes representing agents with 'adopted = True' will be red, otherwise black.</span>
<span class="n">node_colors</span> <span class="o">=</span> <span class="p">[</span><span class="s1">'red'</span> <span class="k">if</span> <span class="n">adopted</span> <span class="k">else</span> <span class="s1">'black'</span> <span class="k">for</span> <span class="n">adopted</span> <span class="ow">in</span> <span class="n">adopted_states</span><span class="p">]</span>

<span class="c1"># Generate labels for nodes based on the agent's category index.</span>
<span class="c1"># Each node is labeled with its corresponding agent's category index as a string.</span>
<span class="n">labels</span> <span class="o">=</span> <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">agent</span><span class="o">.</span><span class="n">category_idx</span><span class="p">)</span> <span class="k">for</span> <span class="n">agent</span> <span class="ow">in</span> <span class="n">model</span><span class="o">.</span><span class="n">agents</span><span class="p">]</span>
<span class="n">labels</span> <span class="o">=</span> <span class="p">{</span><span class="n">i</span><span class="p">:</span> <span class="n">labels</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">labels</span><span class="p">))}</span>  <span class="c1"># Map labels to node indices for visualization.</span>

<span class="c1"># Define the layout of the graph using the spring layout.</span>
<span class="n">pos</span> <span class="o">=</span> <span class="n">nx</span><span class="o">.</span><span class="n">spring_layout</span><span class="p">(</span><span class="n">network</span><span class="o">.</span><span class="n">graph</span><span class="p">)</span>  <span class="c1"># Position nodes using a force-directed layout algorithm.</span>

<span class="c1"># Draw the network graph using NetworkX's `draw` method.</span>
<span class="n">nx</span><span class="o">.</span><span class="n">draw</span><span class="p">(</span>
    <span class="n">network</span><span class="o">.</span><span class="n">graph</span><span class="p">,</span>         <span class="c1"># The graph to draw.</span>
    <span class="n">pos</span><span class="p">,</span>                   <span class="c1"># Node positions.</span>
    <span class="n">node_color</span><span class="o">=</span><span class="n">node_colors</span><span class="p">,</span>  <span class="c1"># Colors of the nodes based on adoption status.</span>
    <span class="n">with_labels</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>     <span class="c1"># Whether to show labels on the nodes (currently disabled).</span>
    <span class="n">node_size</span><span class="o">=</span><span class="mi">500</span>          <span class="c1"># Size of the nodes in the graph.</span>
<span class="p">)</span>

<span class="c1"># Add a legend to explain node colors.</span>
<span class="c1"># The legend will have two entries: one for 'Adopted' (red) and one for 'Not Adopted' (black).</span>
<span class="n">plt</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">handles</span><span class="o">=</span><span class="p">[</span>
    <span class="n">plt</span><span class="o">.</span><span class="n">Line2D</span><span class="p">([</span><span class="mi">0</span><span class="p">],</span> <span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">marker</span><span class="o">=</span><span class="s1">'o'</span><span class="p">,</span> <span class="n">color</span><span class="o">=</span><span class="s1">'w'</span><span class="p">,</span> <span class="n">label</span><span class="o">=</span><span class="s1">'Adopted'</span><span class="p">,</span> <span class="n">markerfacecolor</span><span class="o">=</span><span class="s1">'red'</span><span class="p">,</span> <span class="n">markersize</span><span class="o">=</span><span class="mi">10</span><span class="p">),</span>
    <span class="n">plt</span><span class="o">.</span><span class="n">Line2D</span><span class="p">([</span><span class="mi">0</span><span class="p">],</span> <span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">marker</span><span class="o">=</span><span class="s1">'o'</span><span class="p">,</span> <span class="n">color</span><span class="o">=</span><span class="s1">'w'</span><span class="p">,</span> <span class="n">label</span><span class="o">=</span><span class="s1">'Not Adopted'</span><span class="p">,</span> <span class="n">markerfacecolor</span><span class="o">=</span><span class="s1">'black'</span><span class="p">,</span> <span class="n">markersize</span><span class="o">=</span><span class="mi">10</span><span class="p">)</span>
<span class="p">])</span>

<span class="c1"># Add a title to the plot for better understanding.</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"Agent Network with Node Colors Based on Adoption Status"</span><span class="p">)</span>

<span class="c1"># Display the graph.</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
<span class="c1"># plt.close()  # Optionally close the plot if running in an interactive environment to avoid clutter.</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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q+Ft+3anxVVVlbZu3Ur9+/enihUrRlt3Y7ZMmTJRw4YNaezYsQmuPwCaOXNmrNd37txJAOjAgQOur6OT3Lt3j9ZrveWaDJsaGEgXzp+nX3/9lYYNG0b16tWj9OnTRx+jV155hdq1a0cTJkygbdu2UUhIiG5rTkRE//1H5O+v/9xlWUT8u6E02+12Gj16NAGgbNmy6bb1LUkSderUiex2uw4LbTxDhw6lggULmi0G8xKsUDJpFlVVqU6dOlS6dGmnLVQTJ04kRVGoTZs2cd67cuUKAaC1L1krZs+erduW1sCBA91TKl95xVwFxImAo4iICJo2bRoVKlSIgKTdAyRJila2mzVrRtufK61nz56lgIAAat++fZy1ioiIID8/Pxo/frzra5gIISEhtGDBAmrSpAlZLBayShI9sFpNV/r0alEA/VOhAl24cCHWOtjtdjpz5gwtWrSI3n//fapZsyb5+flFH69ixYpRx44dacqUKbRr1y4KDQ3V7iC88YZxqbEUhahLF5fECwsLo7feeosA0JdffkmPHz+mWrVqJehP7Yky2a5dO+18sJMBLVu2pIYNG5otBvMSrFAyaZo9e/YQAFqwYIFTnx81ahRJkkRffPFFnPdUVaUMGTLQuBiBCStWrNDdP+rTTz91feLvvGPeFmzevEmKFxwcTMWLFydJktxaP4elp0uXLlSqVCkqUqQIPX78ON6xXn/9dWrcuLHra/gST58+peXLl1ObNm3Ix8eHAFDNmjVp+vTpdOvWrVS/7f1qunQEgN544w1auXIlRUZGxrtONpuNjh8/Tj///DP179+fXn31VfL29iZAuHSUKlWKunbtSt9//z3t27fPvZytBw8avwaSRJRYftsYXLt2jSpWrEh+fn7022+/xTqHunXrFr0WntwXHD+uRowYob9Lh8EUL16cBg4caLYYzEuwQsmkeVq1akX58uVzyh+na9euBCS8TV6zZk1q3749EYmHRrp06XRXKCVJoh07drg26e+/N2fb22Ih6tQpQbFUVaWvvvqKZFnWZPvPsfYLFy5McMxx48ZRunTpElSAEiMiIoL++OMPevfddyndc4WqYsWKNGHChLjJ82/cIPLxMV3x0+WY1qpFYWFhNG/ePKpatSoBIohs5MiRdOnSpSTXMTIykg4fPkw//fQT9enThypWrEhWq5Ucluny5ctTr1696Mcf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"/>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=6124c578-1b00-4180-b00b-dd49bd3ce389">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>This plot shows the network at the final state with the nodes that adopted the technology shown in red, and the nodes that did not shown in black. There are clear "islands of Ludites" that have not adopted the technology and wont because of thresholds needed for adoption.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=7cc1aca1">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Playing-around-with-networkx-graphing">Playing around with networkx graphing<a class="anchor-link" href="#Playing-around-with-networkx-graphing">¶</a></h2>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=6158decf">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [39]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">networkx</span> <span class="k">as</span> <span class="nn">nx</span>
<span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span>

<span class="c1"># Parameters for the Watts-Strogatz graph</span>
<span class="n">n</span> <span class="o">=</span> <span class="mi">30</span>  <span class="c1"># Number of nodes</span>
<span class="n">k</span> <span class="o">=</span> <span class="mi">4</span>   <span class="c1"># Each node is connected to k nearest neighbors in ring topology</span>
<span class="n">p</span> <span class="o">=</span> <span class="mf">0.1</span> <span class="c1"># Probability of rewiring each edge</span>

<span class="c1"># Create a Watts-Strogatz small-world graph</span>
<span class="n">G</span> <span class="o">=</span> <span class="n">nx</span><span class="o">.</span><span class="n">watts_strogatz_graph</span><span class="p">(</span><span class="n">n</span><span class="p">,</span> <span class="n">k</span><span class="p">,</span> <span class="n">p</span><span class="p">)</span>

<span class="c1"># Draw the graph</span>
<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">8</span><span class="p">,</span> <span class="mi">6</span><span class="p">))</span>
<span class="n">nx</span><span class="o">.</span><span class="n">draw</span><span class="p">(</span><span class="n">G</span><span class="p">,</span> <span class="n">with_labels</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">node_color</span><span class="o">=</span><span class="s1">'lightblue'</span><span class="p">,</span> <span class="n">edge_color</span><span class="o">=</span><span class="s1">'gray'</span><span class="p">,</span> <span class="n">node_size</span><span class="o">=</span><span class="mi">500</span><span class="p">,</span> <span class="n">font_size</span><span class="o">=</span><span class="mi">10</span><span class="p">)</span>

<span class="c1"># Show the plot</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"Watts-Strogatz Graph"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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kPuaTVZUPtB7pIZGKZchM1bLFZlhjiszRERE5HeOQRyuGJOQiA+/LIHFbEZH+1NE6KLxrz/9IaLjx/pkfHJfdGgIFidF4UqrEfWGDrdW4wC4rk/UjMCUKLUkDzwlz2KYISIiIr+TywbfzUupUkGpUqHdoMfFk19h3d/8d5+OT+5RyGXIiNEidVQY6vRm1OrNsL0Iky+Hm66fK2QCkrUqJGlVbL9MLvw/gYiIiPxOKZe7/Vv6qhPHAIgYnTQODxvq8MWvPkRccgoWFq1xa2zhxfjkWypFENKi1JgYGQ6D1Q69xQa9xQaLwwGHU4RcJkApl0OrVECrVEATEjTg9tk0fDDMEBERkd9plQqIBvfuMbcbsfH//AKPHz5AmFaLmYvzUfzTnyFIoXDrOeKL8ck/ZIKACKUCEfwZ0CCwAQARERH5nbvnzHha5zkzRCQtrJoiIiIiv9OEBEHhp7oVhUyAJoSbVYikiGGGiIiI/E4mCEjSquDrOCMASNaqWItBJFEMM0RERBQQkrUqtxoAeIIIIEmr8vGoROQpDDNEREQUEFSKICRqRvh0zETNCLb5JZIwhhkiIiIKGFOi1FD66CBEpVyGKVFqn4xFRN7BMENEREQBQyGXITNW65OxMmO1PEGeSOL4L5iIiIgCSnRoCNJ13l0xSdepER0a4tUxiMj7GGaIiIgo4IyLCPVaoEnXqTEuItQrzyYi3+KhmURERBSwmk1WVD7Qw+JwvvazlC+2sHFFhmjoYJghIiKigGZzOHGl1Yh6QwcEwK32zZ3XJ2pGYEqUmjUyREMMwwwRERFJgtlmR53ejFq9GTbn89eXl8NN188VMgHJWhWStCq2XyYaohhmiIiISFKcogiD1Q69xQa9xQaLwwGHU4RcJkApl0OrVECrVEATEgSZIPh7ukTkRQwzREREREQkSdw4SkREREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREksQwQ0REREREkvT/AXxo3bojfWXFAAAAAElFTkSuQmCC"/>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=2ad24c28">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [ ]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span> 
</pre></div>
</div>
</div>
</div>
</div>
</div>
</main>
</body>
</html>

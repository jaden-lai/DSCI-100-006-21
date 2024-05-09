<html lang="en"><head><meta charset="utf-8">
<meta content="width=device-width, initial-scale=1.0" name="viewport">
<title>project_final</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
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
<script type="text/javascript" async="" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-AMS_CHTML-full,Safe"></script>
<!-- MathJax configuration -->
<script type="text/x-mathjax-config;executed=true">
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
    const mermaid = (await import("https://cdnjs.cloudflare.com/ajax/libs/mermaid/10.7.0/mermaid.esm.min.mjs")).default;
    const parser = new DOMParser();

    mermaid.initialize({
      maxTextSize: 100000,
      maxEdges: 100000,
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
        let { svg } = await mermaid.render(id, raw, el);
        svg = cleanMermaidSvg(svg);
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


    /**
     * Post-process to ensure mermaid diagrams contain only valid SVG and XHTML.
     */
    function cleanMermaidSvg(svg) {
      return svg.replace(RE_VOID_ELEMENT, replaceVoidElement);
    }


    /**
     * A regular expression for all void elements, which may include attributes and
     * a slash.
     *
     * @see https://developer.mozilla.org/en-US/docs/Glossary/Void_element
     *
     * Of these, only `<br>` is generated by Mermaid in place of `\n`,
     * but _any_ "malformed" tag will break the SVG rendering entirely.
     */
    const RE_VOID_ELEMENT =
      /<\s*(area|base|br|col|embed|hr|img|input|link|meta|param|source|track|wbr)\s*([^>]*?)\s*>/gi;

    /**
     * Ensure a void element is closed with a slash, preserving any attributes.
     */
    function replaceVoidElement(match, tag, rest) {
      rest = rest.trim();
      if (!rest.endsWith('/')) {
        rest = `${rest} /`;
      }
      return `<${tag} ${rest}>`;
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
<!-- End of mermaid configuration --><style type="text/css">.MathJax_Hover_Frame {border-radius: .25em; -webkit-border-radius: .25em; -moz-border-radius: .25em; -khtml-border-radius: .25em; box-shadow: 0px 0px 15px #83A; -webkit-box-shadow: 0px 0px 15px #83A; -moz-box-shadow: 0px 0px 15px #83A; -khtml-box-shadow: 0px 0px 15px #83A; border: 1px solid #A6D ! important; display: inline-block; position: absolute}
.MathJax_Menu_Button .MathJax_Hover_Arrow {position: absolute; cursor: pointer; display: inline-block; border: 2px solid #AAA; border-radius: 4px; -webkit-border-radius: 4px; -moz-border-radius: 4px; -khtml-border-radius: 4px; font-family: 'Courier New',Courier; font-size: 9px; color: #F0F0F0}
.MathJax_Menu_Button .MathJax_Hover_Arrow span {display: block; background-color: #AAA; border: 1px solid; border-radius: 3px; line-height: 0; padding: 4px}
.MathJax_Hover_Arrow:hover {color: white!important; border: 2px solid #CCC!important}
.MathJax_Hover_Arrow:hover span {background-color: #CCC!important}
</style><style type="text/css">#MathJax_About {position: fixed; left: 50%; width: auto; text-align: center; border: 3px outset; padding: 1em 2em; background-color: #DDDDDD; color: black; cursor: default; font-family: message-box; font-size: 120%; font-style: normal; text-indent: 0; text-transform: none; line-height: normal; letter-spacing: normal; word-spacing: normal; word-wrap: normal; white-space: nowrap; float: none; z-index: 201; border-radius: 15px; -webkit-border-radius: 15px; -moz-border-radius: 15px; -khtml-border-radius: 15px; box-shadow: 0px 10px 20px #808080; -webkit-box-shadow: 0px 10px 20px #808080; -moz-box-shadow: 0px 10px 20px #808080; -khtml-box-shadow: 0px 10px 20px #808080; filter: progid:DXImageTransform.Microsoft.dropshadow(OffX=2, OffY=2, Color='gray', Positive='true')}
#MathJax_About.MathJax_MousePost {outline: none}
.MathJax_Menu {position: absolute; background-color: white; color: black; width: auto; padding: 2px; border: 1px solid #CCCCCC; margin: 0; cursor: default; font: menu; text-align: left; text-indent: 0; text-transform: none; line-height: normal; letter-spacing: normal; word-spacing: normal; word-wrap: normal; white-space: nowrap; float: none; z-index: 201; box-shadow: 0px 10px 20px #808080; -webkit-box-shadow: 0px 10px 20px #808080; -moz-box-shadow: 0px 10px 20px #808080; -khtml-box-shadow: 0px 10px 20px #808080; filter: progid:DXImageTransform.Microsoft.dropshadow(OffX=2, OffY=2, Color='gray', Positive='true')}
.MathJax_MenuItem {padding: 2px 2em; background: transparent}
.MathJax_MenuArrow {position: absolute; right: .5em; padding-top: .25em; color: #666666; font-size: .75em}
.MathJax_MenuActive .MathJax_MenuArrow {color: white}
.MathJax_MenuArrow.RTL {left: .5em; right: auto}
.MathJax_MenuCheck {position: absolute; left: .7em}
.MathJax_MenuCheck.RTL {right: .7em; left: auto}
.MathJax_MenuRadioCheck {position: absolute; left: 1em}
.MathJax_MenuRadioCheck.RTL {right: 1em; left: auto}
.MathJax_MenuLabel {padding: 2px 2em 4px 1.33em; font-style: italic}
.MathJax_MenuRule {border-top: 1px solid #CCCCCC; margin: 4px 1px 0px}
.MathJax_MenuDisabled {color: GrayText}
.MathJax_MenuActive {background-color: Highlight; color: HighlightText}
.MathJax_MenuDisabled:focus, .MathJax_MenuLabel:focus {background-color: #E8E8E8}
.MathJax_ContextMenu:focus {outline: none}
.MathJax_ContextMenu .MathJax_MenuItem:focus {outline: none}
#MathJax_AboutClose {top: .2em; right: .2em}
.MathJax_Menu .MathJax_MenuClose {top: -10px; left: -10px}
.MathJax_MenuClose {position: absolute; cursor: pointer; display: inline-block; border: 2px solid #AAA; border-radius: 18px; -webkit-border-radius: 18px; -moz-border-radius: 18px; -khtml-border-radius: 18px; font-family: 'Courier New',Courier; font-size: 24px; color: #F0F0F0}
.MathJax_MenuClose span {display: block; background-color: #AAA; border: 1.5px solid; border-radius: 18px; -webkit-border-radius: 18px; -moz-border-radius: 18px; -khtml-border-radius: 18px; line-height: 0; padding: 8px 0 6px}
.MathJax_MenuClose:hover {color: white!important; border: 2px solid #CCC!important}
.MathJax_MenuClose:hover span {background-color: #CCC!important}
.MathJax_MenuClose:hover:focus {outline: none}
</style><style type="text/css">.MathJax_Preview .MJXf-math {color: inherit!important}
</style><style type="text/css">.MJX_Assistive_MathML {position: absolute!important; top: 0; left: 0; clip: rect(1px, 1px, 1px, 1px); padding: 1px 0 0 0!important; border: 0!important; height: 1px!important; width: 1px!important; overflow: hidden!important; display: block!important; -webkit-touch-callout: none; -webkit-user-select: none; -khtml-user-select: none; -moz-user-select: none; -ms-user-select: none; user-select: none}
.MJX_Assistive_MathML.MJX_Assistive_MathML_Block {width: 100%!important}
</style><style type="text/css">#MathJax_Zoom {position: absolute; background-color: #F0F0F0; overflow: auto; display: block; z-index: 301; padding: .5em; border: 1px solid black; margin: 0; font-weight: normal; font-style: normal; text-align: left; text-indent: 0; text-transform: none; line-height: normal; letter-spacing: normal; word-spacing: normal; word-wrap: normal; white-space: nowrap; float: none; -webkit-box-sizing: content-box; -moz-box-sizing: content-box; box-sizing: content-box; box-shadow: 5px 5px 15px #AAAAAA; -webkit-box-shadow: 5px 5px 15px #AAAAAA; -moz-box-shadow: 5px 5px 15px #AAAAAA; -khtml-box-shadow: 5px 5px 15px #AAAAAA; filter: progid:DXImageTransform.Microsoft.dropshadow(OffX=2, OffY=2, Color='gray', Positive='true')}
#MathJax_ZoomOverlay {position: absolute; left: 0; top: 0; z-index: 300; display: inline-block; width: 100%; height: 100%; border: 0; padding: 0; margin: 0; background-color: white; opacity: 0; filter: alpha(opacity=0)}
#MathJax_ZoomFrame {position: relative; display: inline-block; height: 0; width: 0}
#MathJax_ZoomEventTrap {position: absolute; left: 0; top: 0; z-index: 302; display: inline-block; border: 0; padding: 0; margin: 0; background-color: white; opacity: 0; filter: alpha(opacity=0)}
</style><style type="text/css">.MathJax_Preview {color: #888}
#MathJax_Message {position: fixed; left: 1em; bottom: 1.5em; background-color: #E6E6E6; border: 1px solid #959595; margin: 0px; padding: 2px 8px; z-index: 102; color: black; font-size: 80%; width: auto; white-space: nowrap}
#MathJax_MSIE_Frame {position: absolute; top: 0; left: 0; width: 0px; z-index: 101; border: 0px; margin: 0px; padding: 0px}
.MathJax_Error {color: #CC0000; font-style: italic}
</style><style type="text/css">.MJXp-script {font-size: .8em}
.MJXp-right {-webkit-transform-origin: right; -moz-transform-origin: right; -ms-transform-origin: right; -o-transform-origin: right; transform-origin: right}
.MJXp-bold {font-weight: bold}
.MJXp-italic {font-style: italic}
.MJXp-scr {font-family: MathJax_Script,'Times New Roman',Times,STIXGeneral,serif}
.MJXp-frak {font-family: MathJax_Fraktur,'Times New Roman',Times,STIXGeneral,serif}
.MJXp-sf {font-family: MathJax_SansSerif,'Times New Roman',Times,STIXGeneral,serif}
.MJXp-cal {font-family: MathJax_Caligraphic,'Times New Roman',Times,STIXGeneral,serif}
.MJXp-mono {font-family: MathJax_Typewriter,'Times New Roman',Times,STIXGeneral,serif}
.MJXp-largeop {font-size: 150%}
.MJXp-largeop.MJXp-int {vertical-align: -.2em}
.MJXp-math {display: inline-block; line-height: 1.2; text-indent: 0; font-family: 'Times New Roman',Times,STIXGeneral,serif; white-space: nowrap; border-collapse: collapse}
.MJXp-display {display: block; text-align: center; margin: 1em 0}
.MJXp-math span {display: inline-block}
.MJXp-box {display: block!important; text-align: center}
.MJXp-box:after {content: " "}
.MJXp-rule {display: block!important; margin-top: .1em}
.MJXp-char {display: block!important}
.MJXp-mo {margin: 0 .15em}
.MJXp-mfrac {margin: 0 .125em; vertical-align: .25em}
.MJXp-denom {display: inline-table!important; width: 100%}
.MJXp-denom > * {display: table-row!important}
.MJXp-surd {vertical-align: top}
.MJXp-surd > * {display: block!important}
.MJXp-script-box > *  {display: table!important; height: 50%}
.MJXp-script-box > * > * {display: table-cell!important; vertical-align: top}
.MJXp-script-box > *:last-child > * {vertical-align: bottom}
.MJXp-script-box > * > * > * {display: block!important}
.MJXp-mphantom {visibility: hidden}
.MJXp-munderover, .MJXp-munder {display: inline-table!important}
.MJXp-over {display: inline-block!important; text-align: center}
.MJXp-over > * {display: block!important}
.MJXp-munderover > *, .MJXp-munder > * {display: table-row!important}
.MJXp-mtable {vertical-align: .25em; margin: 0 .125em}
.MJXp-mtable > * {display: inline-table!important; vertical-align: middle}
.MJXp-mtr {display: table-row!important}
.MJXp-mtd {display: table-cell!important; text-align: center; padding: .5em 0 0 .5em}
.MJXp-mtr > .MJXp-mtd:first-child {padding-left: 0}
.MJXp-mtr:first-child > .MJXp-mtd {padding-top: 0}
.MJXp-mlabeledtr {display: table-row!important}
.MJXp-mlabeledtr > .MJXp-mtd:first-child {padding-left: 0}
.MJXp-mlabeledtr:first-child > .MJXp-mtd {padding-top: 0}
.MJXp-merror {background-color: #FFFF88; color: #CC0000; border: 1px solid #CC0000; padding: 1px 3px; font-style: normal; font-size: 90%}
.MJXp-scale0 {-webkit-transform: scaleX(.0); -moz-transform: scaleX(.0); -ms-transform: scaleX(.0); -o-transform: scaleX(.0); transform: scaleX(.0)}
.MJXp-scale1 {-webkit-transform: scaleX(.1); -moz-transform: scaleX(.1); -ms-transform: scaleX(.1); -o-transform: scaleX(.1); transform: scaleX(.1)}
.MJXp-scale2 {-webkit-transform: scaleX(.2); -moz-transform: scaleX(.2); -ms-transform: scaleX(.2); -o-transform: scaleX(.2); transform: scaleX(.2)}
.MJXp-scale3 {-webkit-transform: scaleX(.3); -moz-transform: scaleX(.3); -ms-transform: scaleX(.3); -o-transform: scaleX(.3); transform: scaleX(.3)}
.MJXp-scale4 {-webkit-transform: scaleX(.4); -moz-transform: scaleX(.4); -ms-transform: scaleX(.4); -o-transform: scaleX(.4); transform: scaleX(.4)}
.MJXp-scale5 {-webkit-transform: scaleX(.5); -moz-transform: scaleX(.5); -ms-transform: scaleX(.5); -o-transform: scaleX(.5); transform: scaleX(.5)}
.MJXp-scale6 {-webkit-transform: scaleX(.6); -moz-transform: scaleX(.6); -ms-transform: scaleX(.6); -o-transform: scaleX(.6); transform: scaleX(.6)}
.MJXp-scale7 {-webkit-transform: scaleX(.7); -moz-transform: scaleX(.7); -ms-transform: scaleX(.7); -o-transform: scaleX(.7); transform: scaleX(.7)}
.MJXp-scale8 {-webkit-transform: scaleX(.8); -moz-transform: scaleX(.8); -ms-transform: scaleX(.8); -o-transform: scaleX(.8); transform: scaleX(.8)}
.MJXp-scale9 {-webkit-transform: scaleX(.9); -moz-transform: scaleX(.9); -ms-transform: scaleX(.9); -o-transform: scaleX(.9); transform: scaleX(.9)}
.MathJax_PHTML .noError {vertical-align: ; font-size: 90%; text-align: left; color: black; padding: 1px 3px; border: 1px solid}
</style><style type="text/css">.mjx-chtml {display: inline-block; line-height: 0; text-indent: 0; text-align: left; text-transform: none; font-style: normal; font-weight: normal; font-size: 100%; font-size-adjust: none; letter-spacing: normal; word-wrap: normal; word-spacing: normal; white-space: nowrap; float: none; direction: ltr; max-width: none; max-height: none; min-width: 0; min-height: 0; border: 0; margin: 0; padding: 1px 0}
.MJXc-display {display: block; text-align: center; margin: 1em 0; padding: 0}
.mjx-chtml[tabindex]:focus, body :focus .mjx-chtml[tabindex] {display: inline-table}
.mjx-full-width {text-align: center; display: table-cell!important; width: 10000em}
.mjx-math {display: inline-block; border-collapse: separate; border-spacing: 0}
.mjx-math * {display: inline-block; -webkit-box-sizing: content-box!important; -moz-box-sizing: content-box!important; box-sizing: content-box!important; text-align: left}
.mjx-numerator {display: block; text-align: center}
.mjx-denominator {display: block; text-align: center}
.MJXc-stacked {height: 0; position: relative}
.MJXc-stacked > * {position: absolute}
.MJXc-bevelled > * {display: inline-block}
.mjx-stack {display: inline-block}
.mjx-op {display: block}
.mjx-under {display: table-cell}
.mjx-over {display: block}
.mjx-over > * {padding-left: 0px!important; padding-right: 0px!important}
.mjx-under > * {padding-left: 0px!important; padding-right: 0px!important}
.mjx-stack > .mjx-sup {display: block}
.mjx-stack > .mjx-sub {display: block}
.mjx-prestack > .mjx-presup {display: block}
.mjx-prestack > .mjx-presub {display: block}
.mjx-delim-h > .mjx-char {display: inline-block}
.mjx-surd {vertical-align: top}
.mjx-mphantom * {visibility: hidden}
.mjx-merror {background-color: #FFFF88; color: #CC0000; border: 1px solid #CC0000; padding: 2px 3px; font-style: normal; font-size: 90%}
.mjx-annotation-xml {line-height: normal}
.mjx-menclose > svg {fill: none; stroke: currentColor}
.mjx-mtr {display: table-row}
.mjx-mlabeledtr {display: table-row}
.mjx-mtd {display: table-cell; text-align: center}
.mjx-label {display: table-row}
.mjx-box {display: inline-block}
.mjx-block {display: block}
.mjx-span {display: inline}
.mjx-char {display: block; white-space: pre}
.mjx-itable {display: inline-table; width: auto}
.mjx-row {display: table-row}
.mjx-cell {display: table-cell}
.mjx-table {display: table; width: 100%}
.mjx-line {display: block; height: 0}
.mjx-strut {width: 0; padding-top: 1em}
.mjx-vsize {width: 0}
.MJXc-space1 {margin-left: .167em}
.MJXc-space2 {margin-left: .222em}
.MJXc-space3 {margin-left: .278em}
.mjx-chartest {display: block; visibility: hidden; position: absolute; top: 0; line-height: normal; font-size: 500%}
.mjx-chartest .mjx-char {display: inline}
.mjx-chartest .mjx-box {padding-top: 1000px}
.MJXc-processing {visibility: hidden; position: fixed; width: 0; height: 0; overflow: hidden}
.MJXc-processed {display: none}
.mjx-test {font-style: normal; font-weight: normal; font-size: 100%; font-size-adjust: none; text-indent: 0; text-transform: none; letter-spacing: normal; word-spacing: normal; overflow: hidden; height: 1px}
.mjx-test.mjx-test-display {display: table!important}
.mjx-test.mjx-test-inline {display: inline!important; margin-right: -1px}
.mjx-test.mjx-test-default {display: block!important; clear: both}
.mjx-ex-box {display: inline-block!important; position: absolute; overflow: hidden; min-height: 0; max-height: none; padding: 0; border: 0; margin: 0; width: 1px; height: 60ex}
.mjx-test-inline .mjx-left-box {display: inline-block; width: 0; float: left}
.mjx-test-inline .mjx-right-box {display: inline-block; width: 0; float: right}
.mjx-test-display .mjx-right-box {display: table-cell!important; width: 10000em!important; min-width: 0; max-width: none; padding: 0; border: 0; margin: 0}
#MathJax_CHTML_Tooltip {background-color: InfoBackground; color: InfoText; border: 1px solid black; box-shadow: 2px 2px 5px #AAAAAA; -webkit-box-shadow: 2px 2px 5px #AAAAAA; -moz-box-shadow: 2px 2px 5px #AAAAAA; -khtml-box-shadow: 2px 2px 5px #AAAAAA; padding: 3px 4px; z-index: 401; position: absolute; left: 0; top: 0; width: auto; height: auto; display: none}
.mjx-chtml .mjx-noError {line-height: 1.2; vertical-align: ; font-size: 90%; text-align: left; color: black; padding: 1px 3px; border: 1px solid}
.MJXc-TeX-unknown-R {font-family: STIXGeneral,'Cambria Math','Arial Unicode MS',serif; font-style: normal; font-weight: normal}
.MJXc-TeX-unknown-I {font-family: STIXGeneral,'Cambria Math','Arial Unicode MS',serif; font-style: italic; font-weight: normal}
.MJXc-TeX-unknown-B {font-family: STIXGeneral,'Cambria Math','Arial Unicode MS',serif; font-style: normal; font-weight: bold}
.MJXc-TeX-unknown-BI {font-family: STIXGeneral,'Cambria Math','Arial Unicode MS',serif; font-style: italic; font-weight: bold}
.MJXc-TeX-ams-R {font-family: MJXc-TeX-ams-R,MJXc-TeX-ams-Rw}
.MJXc-TeX-cal-B {font-family: MJXc-TeX-cal-B,MJXc-TeX-cal-Bx,MJXc-TeX-cal-Bw}
.MJXc-TeX-frak-R {font-family: MJXc-TeX-frak-R,MJXc-TeX-frak-Rw}
.MJXc-TeX-frak-B {font-family: MJXc-TeX-frak-B,MJXc-TeX-frak-Bx,MJXc-TeX-frak-Bw}
.MJXc-TeX-math-BI {font-family: MJXc-TeX-math-BI,MJXc-TeX-math-BIx,MJXc-TeX-math-BIw}
.MJXc-TeX-sans-R {font-family: MJXc-TeX-sans-R,MJXc-TeX-sans-Rw}
.MJXc-TeX-sans-B {font-family: MJXc-TeX-sans-B,MJXc-TeX-sans-Bx,MJXc-TeX-sans-Bw}
.MJXc-TeX-sans-I {font-family: MJXc-TeX-sans-I,MJXc-TeX-sans-Ix,MJXc-TeX-sans-Iw}
.MJXc-TeX-script-R {font-family: MJXc-TeX-script-R,MJXc-TeX-script-Rw}
.MJXc-TeX-type-R {font-family: MJXc-TeX-type-R,MJXc-TeX-type-Rw}
.MJXc-TeX-cal-R {font-family: MJXc-TeX-cal-R,MJXc-TeX-cal-Rw}
.MJXc-TeX-main-B {font-family: MJXc-TeX-main-B,MJXc-TeX-main-Bx,MJXc-TeX-main-Bw}
.MJXc-TeX-main-I {font-family: MJXc-TeX-main-I,MJXc-TeX-main-Ix,MJXc-TeX-main-Iw}
.MJXc-TeX-main-R {font-family: MJXc-TeX-main-R,MJXc-TeX-main-Rw}
.MJXc-TeX-math-I {font-family: MJXc-TeX-math-I,MJXc-TeX-math-Ix,MJXc-TeX-math-Iw}
.MJXc-TeX-size1-R {font-family: MJXc-TeX-size1-R,MJXc-TeX-size1-Rw}
.MJXc-TeX-size2-R {font-family: MJXc-TeX-size2-R,MJXc-TeX-size2-Rw}
.MJXc-TeX-size3-R {font-family: MJXc-TeX-size3-R,MJXc-TeX-size3-Rw}
.MJXc-TeX-size4-R {font-family: MJXc-TeX-size4-R,MJXc-TeX-size4-Rw}
.MJXc-TeX-vec-R {font-family: MJXc-TeX-vec-R,MJXc-TeX-vec-Rw}
.MJXc-TeX-vec-B {font-family: MJXc-TeX-vec-B,MJXc-TeX-vec-Bx,MJXc-TeX-vec-Bw}
@font-face {font-family: MJXc-TeX-ams-R; src: local('MathJax_AMS'), local('MathJax_AMS-Regular')}
@font-face {font-family: MJXc-TeX-ams-Rw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_AMS-Regular.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_AMS-Regular.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_AMS-Regular.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-cal-B; src: local('MathJax_Caligraphic Bold'), local('MathJax_Caligraphic-Bold')}
@font-face {font-family: MJXc-TeX-cal-Bx; src: local('MathJax_Caligraphic'); font-weight: bold}
@font-face {font-family: MJXc-TeX-cal-Bw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Caligraphic-Bold.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Caligraphic-Bold.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Caligraphic-Bold.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-frak-R; src: local('MathJax_Fraktur'), local('MathJax_Fraktur-Regular')}
@font-face {font-family: MJXc-TeX-frak-Rw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Fraktur-Regular.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Fraktur-Regular.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Fraktur-Regular.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-frak-B; src: local('MathJax_Fraktur Bold'), local('MathJax_Fraktur-Bold')}
@font-face {font-family: MJXc-TeX-frak-Bx; src: local('MathJax_Fraktur'); font-weight: bold}
@font-face {font-family: MJXc-TeX-frak-Bw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Fraktur-Bold.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Fraktur-Bold.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Fraktur-Bold.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-math-BI; src: local('MathJax_Math BoldItalic'), local('MathJax_Math-BoldItalic')}
@font-face {font-family: MJXc-TeX-math-BIx; src: local('MathJax_Math'); font-weight: bold; font-style: italic}
@font-face {font-family: MJXc-TeX-math-BIw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Math-BoldItalic.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Math-BoldItalic.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Math-BoldItalic.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-sans-R; src: local('MathJax_SansSerif'), local('MathJax_SansSerif-Regular')}
@font-face {font-family: MJXc-TeX-sans-Rw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_SansSerif-Regular.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_SansSerif-Regular.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_SansSerif-Regular.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-sans-B; src: local('MathJax_SansSerif Bold'), local('MathJax_SansSerif-Bold')}
@font-face {font-family: MJXc-TeX-sans-Bx; src: local('MathJax_SansSerif'); font-weight: bold}
@font-face {font-family: MJXc-TeX-sans-Bw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_SansSerif-Bold.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_SansSerif-Bold.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_SansSerif-Bold.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-sans-I; src: local('MathJax_SansSerif Italic'), local('MathJax_SansSerif-Italic')}
@font-face {font-family: MJXc-TeX-sans-Ix; src: local('MathJax_SansSerif'); font-style: italic}
@font-face {font-family: MJXc-TeX-sans-Iw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_SansSerif-Italic.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_SansSerif-Italic.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_SansSerif-Italic.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-script-R; src: local('MathJax_Script'), local('MathJax_Script-Regular')}
@font-face {font-family: MJXc-TeX-script-Rw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Script-Regular.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Script-Regular.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Script-Regular.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-type-R; src: local('MathJax_Typewriter'), local('MathJax_Typewriter-Regular')}
@font-face {font-family: MJXc-TeX-type-Rw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Typewriter-Regular.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Typewriter-Regular.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Typewriter-Regular.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-cal-R; src: local('MathJax_Caligraphic'), local('MathJax_Caligraphic-Regular')}
@font-face {font-family: MJXc-TeX-cal-Rw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Caligraphic-Regular.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Caligraphic-Regular.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Caligraphic-Regular.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-main-B; src: local('MathJax_Main Bold'), local('MathJax_Main-Bold')}
@font-face {font-family: MJXc-TeX-main-Bx; src: local('MathJax_Main'); font-weight: bold}
@font-face {font-family: MJXc-TeX-main-Bw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Main-Bold.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Main-Bold.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Main-Bold.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-main-I; src: local('MathJax_Main Italic'), local('MathJax_Main-Italic')}
@font-face {font-family: MJXc-TeX-main-Ix; src: local('MathJax_Main'); font-style: italic}
@font-face {font-family: MJXc-TeX-main-Iw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Main-Italic.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Main-Italic.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Main-Italic.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-main-R; src: local('MathJax_Main'), local('MathJax_Main-Regular')}
@font-face {font-family: MJXc-TeX-main-Rw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Main-Regular.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Main-Regular.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Main-Regular.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-math-I; src: local('MathJax_Math Italic'), local('MathJax_Math-Italic')}
@font-face {font-family: MJXc-TeX-math-Ix; src: local('MathJax_Math'); font-style: italic}
@font-face {font-family: MJXc-TeX-math-Iw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Math-Italic.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Math-Italic.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Math-Italic.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-size1-R; src: local('MathJax_Size1'), local('MathJax_Size1-Regular')}
@font-face {font-family: MJXc-TeX-size1-Rw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Size1-Regular.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Size1-Regular.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Size1-Regular.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-size2-R; src: local('MathJax_Size2'), local('MathJax_Size2-Regular')}
@font-face {font-family: MJXc-TeX-size2-Rw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Size2-Regular.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Size2-Regular.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Size2-Regular.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-size3-R; src: local('MathJax_Size3'), local('MathJax_Size3-Regular')}
@font-face {font-family: MJXc-TeX-size3-Rw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Size3-Regular.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Size3-Regular.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Size3-Regular.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-size4-R; src: local('MathJax_Size4'), local('MathJax_Size4-Regular')}
@font-face {font-family: MJXc-TeX-size4-Rw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Size4-Regular.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Size4-Regular.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Size4-Regular.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-vec-R; src: local('MathJax_Vector'), local('MathJax_Vector-Regular')}
@font-face {font-family: MJXc-TeX-vec-Rw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Vector-Regular.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Vector-Regular.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Vector-Regular.otf') format('opentype')}
@font-face {font-family: MJXc-TeX-vec-B; src: local('MathJax_Vector Bold'), local('MathJax_Vector-Bold')}
@font-face {font-family: MJXc-TeX-vec-Bx; src: local('MathJax_Vector'); font-weight: bold}
@font-face {font-family: MJXc-TeX-vec-Bw; src /*1*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/eot/MathJax_Vector-Bold.eot'); src /*2*/: url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/woff/MathJax_Vector-Bold.woff') format('woff'), url('https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/fonts/HTML-CSS/TeX/otf/MathJax_Vector-Bold.otf') format('opentype')}
</style></head>
<body class="jp-Notebook" data-jp-theme-light="true" data-jp-theme-name="JupyterLab Light"><div id="MathJax_Message" style="display: none;"></div>
<main>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=b336fa50-5302-4437-a25a-066940531ede">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h1 id="Data-Science-Group-Project-Report-006-021">Data Science Group Project Report 006-021<a class="anchor-link" href="#Data-Science-Group-Project-Report-006-021">¶</a></h1><h2 id="Heart-Disease-Hungarian-Data:">Heart Disease Hungarian Data:<a class="anchor-link" href="#Heart-Disease-Hungarian-Data:">¶</a></h2><h5 id="Members:">Members:<a class="anchor-link" href="#Members:">¶</a></h5><ul>
<li>Jaden Lai (79465795)</li>
<li>Percy Pham (70210562)</li>
<li>Sydney Trim (86059649)</li>
</ul>
<h4 id="Introduction:">Introduction:<a class="anchor-link" href="#Introduction:">¶</a></h4><p>Heart disease is a leading cause of death worldwide associated with many variables. This project aims to identify patients most likely to experience heart problems by analyzing age, resting blood pressure, maximum heart rate, and cholestrol. To answer this question we will be analyzing the Heart Disease Data Set from the Hungarian Institute of Cardiology. This dataset provides fourteen attributes. However, we have selected five of them to find an answer to our question.</p>
<h4 id="Question:">Question:<a class="anchor-link" href="#Question:">¶</a></h4><p>What kind of patients are most likely to experience heart disease using age, resting blood pressure, maximum heart rate, and cholestrol?</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=279b6d09-e456-4782-acd4-172ec93c9757">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[87]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">library</span><span class="p">(</span><span class="n">tidyverse</span><span class="p">)</span>
<span class="n">library</span><span class="p">(</span><span class="nb">repr</span><span class="p">)</span>
<span class="n">library</span><span class="p">(</span><span class="n">tidymodels</span><span class="p">)</span>
<span class="n">options</span><span class="p">(</span><span class="nb">repr</span><span class="o">.</span><span class="n">matrix</span><span class="o">.</span><span class="n">max</span><span class="o">.</span><span class="n">rows</span> <span class="o">=</span> <span class="mi">6</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=304e04df-2202-4c13-b1f3-57a83da68ca0">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="Methods-&amp;-Results">Methods &amp; Results<a class="anchor-link" href="#Methods-&amp;-Results">¶</a></h3><p>We begin by downloading, cleaning, and wrangling the data set where we assign column names, select our variables of interest, and filter missing cells; all the pre-processing needed to analyze this heart data set.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=9485b818-23a5-4e78-a08a-10b5c98530df">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[88]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">download</span><span class="o">.</span><span class="n">file</span><span class="p">(</span><span class="s2">"https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.hungarian.data"</span><span class="p">,</span> <span class="s2">"project.csv"</span><span class="p">)</span>
<span class="n">heart_disease_hungarian</span> <span class="o">&lt;-</span> <span class="n">read_csv</span><span class="p">(</span><span class="s2">"project.csv"</span><span class="p">,</span> <span class="n">col_names</span> <span class="o">=</span> <span class="n">FALSE</span><span class="p">)</span>
<span class="n">colnames</span><span class="p">(</span><span class="n">heart_disease_hungarian</span><span class="p">)</span> <span class="o">&lt;-</span> <span class="n">c</span><span class="p">(</span><span class="s2">"age"</span><span class="p">,</span> <span class="s2">"sex"</span><span class="p">,</span> <span class="s2">"chest_pain"</span><span class="p">,</span> <span class="s2">"resting_blood_pressure"</span><span class="p">,</span> <span class="s2">"cholesterol"</span><span class="p">,</span>
                                       <span class="s2">"fasting_blood_sugar"</span><span class="p">,</span> <span class="s2">"resting_electrocardiographic_results"</span><span class="p">,</span> <span class="s2">"maximum_heart_rate_achieved"</span><span class="p">,</span> 
                                       <span class="s2">"exercise_induced_angina"</span><span class="p">,</span> <span class="s2">"ST_depression"</span><span class="p">,</span>
                                       <span class="s2">"slope_of_peak_exercise_ST_segment"</span><span class="p">,</span>
                                       <span class="s2">"number_of_major_vessels"</span><span class="p">,</span> <span class="s2">"thalassemia"</span><span class="p">,</span> <span class="s2">"heart_disease_cases"</span><span class="p">)</span>

<span class="n">heart_disease_hungarian</span> <span class="o">&lt;-</span> <span class="n">heart_disease_hungarian</span> <span class="o">|&gt;</span>
             <span class="n">select</span><span class="p">(</span><span class="n">age</span><span class="p">,</span> <span class="n">resting_blood_pressure</span><span class="p">,</span> <span class="n">maximum_heart_rate_achieved</span><span class="p">,</span>  <span class="n">cholesterol</span><span class="p">,</span> <span class="n">heart_disease_cases</span><span class="p">)</span> <span class="o">|&gt;</span>
             <span class="n">mutate</span><span class="p">(</span><span class="n">maximum_heart_rate_achieved</span> <span class="o">=</span> <span class="k">as</span><span class="o">.</span><span class="n">numeric</span><span class="p">(</span><span class="n">maximum_heart_rate_achieved</span><span class="p">))</span> <span class="o">|&gt;</span>
             <span class="n">mutate</span><span class="p">(</span><span class="n">cholesterol</span> <span class="o">=</span> <span class="k">as</span><span class="o">.</span><span class="n">numeric</span><span class="p">(</span><span class="n">cholesterol</span><span class="p">))</span> <span class="o">|&gt;</span>
             <span class="n">mutate</span><span class="p">(</span><span class="n">resting_blood_pressure</span> <span class="o">=</span> <span class="k">as</span><span class="o">.</span><span class="n">numeric</span><span class="p">(</span><span class="n">resting_blood_pressure</span><span class="p">))</span> <span class="o">|&gt;</span>
             <span class="n">mutate</span><span class="p">(</span><span class="n">heart_disease_cases</span> <span class="o">=</span> <span class="k">as</span><span class="o">.</span><span class="n">factor</span><span class="p">(</span><span class="n">heart_disease_cases</span><span class="p">))</span> <span class="o">|&gt;</span>
             <span class="nb">filter</span><span class="p">(</span><span class="n">maximum_heart_rate_achieved</span> <span class="o">!=</span> <span class="s2">"NA"</span><span class="p">)</span> <span class="o">|&gt;</span>
             <span class="nb">filter</span><span class="p">(</span><span class="n">resting_blood_pressure</span> <span class="o">!=</span> <span class="s2">"NA"</span><span class="p">)</span> <span class="o">|&gt;</span>
             <span class="nb">filter</span><span class="p">(</span><span class="n">age</span> <span class="o">!=</span> <span class="s2">"NA"</span><span class="p">)</span> <span class="o">|&gt;</span>
             <span class="nb">filter</span><span class="p">(</span><span class="n">resting_blood_pressure</span> <span class="o">!=</span> <span class="s2">"NA"</span><span class="p">)</span> <span class="o">|&gt;</span>
             <span class="nb">filter</span><span class="p">(</span><span class="n">cholesterol</span> <span class="o">!=</span> <span class="s2">"?"</span><span class="p">)</span>

<span class="n">heart_disease_hungarian</span>
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
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="application/vnd.jupyter.stderr" tabindex="0">
<pre><span class="ansi-bold">Rows: </span><span class="ansi-blue-fg">294</span> <span class="ansi-bold">Columns: </span><span class="ansi-blue-fg">14</span>
<span class="ansi-cyan-fg">──</span> <span class="ansi-bold">Column specification</span> <span class="ansi-cyan-fg">────────────────────────────────────────────────────────</span>
<span class="ansi-bold">Delimiter:</span> ","
<span class="ansi-red-fg">chr</span> (9): X4, X5, X6, X7, X8, X9, X11, X12, X13
<span class="ansi-green-fg">dbl</span> (5): X1, X2, X3, X10, X14

<span class="ansi-cyan-fg">ℹ</span> Use `spec()` to retrieve the full column specification for this data.
<span class="ansi-cyan-fg">ℹ</span> Specify the column types or set `show_col_types = FALSE` to quiet this message.
Warning message in mask$eval_all_mutate(quo):
“NAs introduced by coercion”
Warning message in mask$eval_all_mutate(quo):
“NAs introduced by coercion”
Warning message in mask$eval_all_mutate(quo):
“NAs introduced by coercion”
</pre>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output" data-mime-type="text/html" tabindex="0">
<table class="dataframe">
<caption>A tibble: 270 × 5</caption>
<thead>
<tr><th scope="col">age</th><th scope="col">resting_blood_pressure</th><th scope="col">maximum_heart_rate_achieved</th><th scope="col">cholesterol</th><th scope="col">heart_disease_cases</th></tr>
<tr><th scope="col">&lt;dbl&gt;</th><th scope="col">&lt;dbl&gt;</th><th scope="col">&lt;dbl&gt;</th><th scope="col">&lt;dbl&gt;</th><th scope="col">&lt;fct&gt;</th></tr>
</thead>
<tbody>
<tr><td>28</td><td>130</td><td>185</td><td>132</td><td>0</td></tr>
<tr><td>29</td><td>120</td><td>160</td><td>243</td><td>0</td></tr>
<tr><td>30</td><td>170</td><td>170</td><td>237</td><td>0</td></tr>
<tr><td>⋮</td><td>⋮</td><td>⋮</td><td>⋮</td><td>⋮</td></tr>
<tr><td>56</td><td>155</td><td>150</td><td>342</td><td>1</td></tr>
<tr><td>58</td><td>180</td><td>110</td><td>393</td><td>1</td></tr>
<tr><td>65</td><td>130</td><td>115</td><td>275</td><td>1</td></tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=0af8dae2-4d47-4088-88be-d36be7cfcca9">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><em>Table 1: Cleaned heart disease data set</em></p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=857d31fa-7b61-4c31-8abc-8bf7c571af75">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h5 id="Variable-Explanation:">Variable Explanation:<a class="anchor-link" href="#Variable-Explanation:">¶</a></h5><ul>
<li>Resting blood pressure: mmHg</li>
<li>Cholesterol: mg/dl</li>
<li>Heat disease cases: 1 = Positive, 0 = Negative</li>
</ul>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=ac3ee5b0-f47a-4ddc-b36c-c4b4a45ac7af">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Now that we have cleaned our dataset, we perform a summary in preparation for exploratory data analysis.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=c22f12e9-6dab-43d6-a015-0c7eab0b20ec">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[89]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span> <span class="n">heart_disease_hungarian_summarize</span> <span class="o">&lt;-</span> <span class="n">heart_disease_hungarian</span> <span class="o">|&gt;</span> 
            <span class="nb">filter</span><span class="p">(</span><span class="n">heart_disease_cases</span> <span class="o">==</span> <span class="mi">1</span><span class="p">)</span> <span class="o">|&gt;</span>
            <span class="n">group_by</span><span class="p">(</span><span class="n">age</span><span class="p">)</span> <span class="o">|&gt;</span>
            <span class="n">summarize</span><span class="p">(</span><span class="n">case_count</span> <span class="o">=</span> <span class="n">n</span><span class="p">())</span> <span class="o">|&gt;</span>
            <span class="n">arrange</span><span class="p">(</span><span class="n">case_count</span><span class="p">)</span>

<span class="n">heart_disease_hungarian_summarize</span>
<span class="n">tail</span><span class="p">(</span><span class="n">heart_disease_hungarian_summarize</span><span class="p">,</span> <span class="mi">7</span><span class="p">)</span>
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
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output" data-mime-type="text/html" tabindex="0">
<table class="dataframe">
<caption>A tibble: 31 × 2</caption>
<thead>
<tr><th scope="col">age</th><th scope="col">case_count</th></tr>
<tr><th scope="col">&lt;dbl&gt;</th><th scope="col">&lt;int&gt;</th></tr>
</thead>
<tbody>
<tr><td>31</td><td>1</td></tr>
<tr><td>32</td><td>1</td></tr>
<tr><td>33</td><td>1</td></tr>
<tr><td>⋮</td><td>⋮</td></tr>
<tr><td>48</td><td>8</td></tr>
<tr><td>52</td><td>8</td></tr>
<tr><td>54</td><td>8</td></tr>
</tbody>
</table>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output" data-mime-type="text/html" tabindex="0">
<table class="dataframe">
<caption>A tibble: 7 × 2</caption>
<thead>
<tr><th scope="col">age</th><th scope="col">case_count</th></tr>
<tr><th scope="col">&lt;dbl&gt;</th><th scope="col">&lt;int&gt;</th></tr>
</thead>
<tbody>
<tr><td>56</td><td>5</td></tr>
<tr><td>58</td><td>5</td></tr>
<tr><td>46</td><td>6</td></tr>
<tr><td>⋮</td><td>⋮</td></tr>
<tr><td>48</td><td>8</td></tr>
<tr><td>52</td><td>8</td></tr>
<tr><td>54</td><td>8</td></tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=8fb96d4b-4589-400c-845b-657b6f9c48c7">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><em>Table 2 &amp; 3: Number of cases sorted by age in descending order</em></p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=dab60e49-ea5e-4145-8c37-537131fa09c1">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h5 id="Table-Summary:">Table Summary:<a class="anchor-link" href="#Table-Summary:">¶</a></h5><p>Organizing our data set, we can make an inference that heart disease cases are mostly found in older patients in the age range of 45-55,testing positive most frequently at the age of 54, and as early as 31.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=c0dbed5b-b265-418e-abf3-1eb6c8169428">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[90]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">options</span><span class="p">(</span><span class="nb">repr</span><span class="o">.</span><span class="n">plot</span><span class="o">.</span><span class="n">width</span> <span class="o">=</span> <span class="mi">13</span><span class="p">,</span> <span class="nb">repr</span><span class="o">.</span><span class="n">plot</span><span class="o">.</span><span class="n">height</span> <span class="o">=</span> <span class="mi">7</span><span class="p">)</span>

<span class="n">heart_disease_plot</span> <span class="o">&lt;-</span> <span class="n">heart_disease_hungarian</span> <span class="o">|&gt;</span> 
    <span class="n">ggplot</span><span class="p">(</span><span class="n">aes</span><span class="p">(</span><span class="n">x</span> <span class="o">=</span> <span class="n">age</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">resting_blood_pressure</span><span class="p">,</span> <span class="n">color</span> <span class="o">=</span> <span class="n">heart_disease_cases</span><span class="p">))</span> <span class="o">+</span> 
        <span class="n">geom_point</span><span class="p">(</span><span class="n">size</span> <span class="o">=</span> <span class="mi">3</span><span class="p">)</span> <span class="o">+</span>
        <span class="n">labs</span><span class="p">(</span><span class="n">x</span> <span class="o">=</span> <span class="s2">"Age"</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="s2">"Resting blood pressure"</span><span class="p">,</span> <span class="n">color</span> <span class="o">=</span> <span class="s2">"Heart disease cases"</span><span class="p">,</span> <span class="n">title</span> <span class="o">=</span> <span class="s2">"Comparing age and resting blood pressure with heart disease"</span><span class="p">)</span>

<span class="n">heart_disease_plot</span> <span class="o">&lt;-</span> <span class="n">heart_disease_plot</span> <span class="o">+</span> 
       <span class="n">scale_fill_brewer</span><span class="p">(</span><span class="n">palette</span> <span class="o">=</span> <span class="s2">"YlOrRd"</span><span class="p">)</span>
<span class="n">heart_disease_plot</span>
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
<img alt="No description has been provided for this image" class="" height="420" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAABhgAAANICAIAAAC6xnKGAAAACXBIWXMAABJ0AAASdAHeZh94
AAAgAElEQVR4nOzdeXxU1f3/8XOXWZNJJmQBWUVFAsgiIrIJuFKWanGve0tVVGz7aKUuuFBa
l5/i0i91RVGqVVtbRMRdQRBFREVFZZHFGNaQkG2SzHrv74/Racwyc5jMZDKT1/OvzM2ZM587
595Z3nPvuYppmgIAAAAAAACIRU11AQAAAAAAAEgPBEkAAAAAAACQQpAEAAAAAAAAKQRJAAAA
AAAAkEKQBAAAAAAAACkESQAAAAAAAJBCkAQAAAAAAAApBElp4MYbb1QU5dFHH011IWns888/
VxRl4sSJqS5EiHYc0FtuuUVRlL///e9tbJMoHWoUMk/M7eruu+9WFGX+/PmH1G189+oImmxv
vJACAAAACZEhQVJZWdmf//zn0aNHFxYW2my2nj17jhkzZv78+QcOHEh1aQmQl5fXp08fl8uV
6kIQp2eeeWbZsmWRmwwokqH5dtVkw0tfCVkR9jsAAAAgITIhSPrHP/7Rt2/fuXPnfvrpp4cf
fviECRNyc3M//fTT2bNn9+/f/6233kp1gW11ww03fPfddxdddFGqC0Gc/vSnPzX+GsyAIhma
b1dNNrz0lZAVYb8DAAAAEiLtg6QXXnjhsssu83q9c+bMKS8vX79+/VtvvfX111+Xlpb+9re/
raysnDJlyoYNG1JdJjqvHTt27Nu3L9VVoNPJmA0vY1YEAAAAyAzpHSTV1tZeffXVQoiHHnro
r3/9a05OTuRfRUVFf/vb32644YZQKNR4UoxAIPC3v/3t+OOPd7lcdrv9qKOOmjVr1p49eyIN
br31VkVRli1btnbt2okTJ7pcrsLCwssvv7y2ttY0zQcffLC4uNjpdA4cOPCuu+4yTTN8rz/8
4Q+KoixZsmTlypXhQ6JcLtf48ePffffdxgXX1NTcdNNNAwYMcDgcNputX79+s2fPrqmpiTSY
M2dO+NEffvjhHj16uN1u0Wxqj0iFX3/99fTp04uKiux2+7Bhw55//vnGj/X9999feOGFhYWF
Tqfz+OOPX7JkycGDBxVFOeGEE6I8pTErlOzZNM0nnnhi9OjRLpfL4XAMGDDg1ltvrauriz6g
MR9dct1LSkouuOCCgoICp9M5bNiwRYsWRX9c0cozL7ki//nPf04++eQuXbpYrdbu3btPnjz5
9ddfD//rnHPOOfLII4UQTz75pKIo48aNE+07oEIIVVXDm2VOTk52dva4cePeeeedKO1j7iOS
beIYBZn9KEkjJdNg1qxZiqI8/fTTje/y0UcfKYoybdq0tpfXWI8ePRwOh9/vjyxZv369oiiK
ouzevTuy8MCBA6qqHn/88eKn21WLG16YpmnffPPNtGnT8vLyHA7HsGHD/vWvf0UZFMl7yaxg
HC+AUVakiZjbW/M5kmJuDwlZqUQ9EAAAANBB6KkuoE2effbZqqqqESNGzJw5s8UGc+fOveaa
a3r37h2+aRjGmWee+frrrxcXF8+YMSMnJ+eTTz556KGHlixZsnbt2j59+gghrFarEOKjjz56
5JFHJk2adNlll7388suLFy82DKN79+7PPffc1KlT6+vrX3jhhZtvvrlnz56XXHJJ5F4rV658
8sknTzvttCuuuGLbtm3Lli2bNGnSO++8E57tNRAITJs27f333z/uuONmzZoVCATeeOON+fPn
r1q1au3atZqmRfpZtWrVo48+euaZZ2ZnZzdfqXCbDRs2XHrppSeccMLFF1+8devWV1999cIL
L+zatevJJ58shKioqBg3blxpaenYsWNPPfXUXbt2XXTRRbfccosQwm63t/Z8ylQo2fOll176
7LPPHnbYYVdddZXNZluxYsVf//rX5cuXr169urU5SuSfn+jrXllZeeKJJ5aWlo4fP378+PEH
DhyYM2fO5MmTo2xIUZ75mCuycOHCK6+8srCw8LzzzisqKtq9e/fSpUunTp26ePHiSy655Fe/
+pXL5Xr66adHjRp1/vnn9+jRoz0HNOzzzz//wx/+cNJJJ11xxRXbt29ftmzZ5MmT33nnnQkT
JjRvLLOPyLRpyyhE34+SNFIyDWTEXV4Tp5122uLFiz/++ONIdLJy5Uqr1er3+1etWnXhhReG
F7733numaU6aNKnJ3aNseLt37x47duzIkSNnzJjx7bffLlu27Je//GVBQcEpp5wSZb1i3ivm
Csb3AnjmmWfG3INEXNubzHAnZKUS8kAAAABAB2Kms7PPPlsIcd9990m2f/zxx4UQo0eP9nq9
kYXhb+PnnXde+OZdd90lhLDZbCtXrgwvKSkp0TTNYrEUFxdXVFSEFz7xxBNCiGnTpoVvzpkz
Rwihquorr7wS6fnee+8VQowaNSp887///W/4ZjAYDC/x+XzFxcVCiGXLloWX3HnnnUKI3Nzc
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
JjxN0nvvvdevX78jjjhCvs9kkFzB5L0AtmV7a224E75SbXwgAAAAoONI7zmSfvnLXxYVFW3f
vj18safm7rzzzttuuy18QoEQIjyTxQcffNC4zcGDB7ds2eJwOAYNGtTGej7++OPGN2trazdv
3qxpWq9evXw+3+7du7Ozsxt/3zBN84033mjjgzanaVrfvn1DodDmzZsbL4/+WDIVSvYcnpok
Mk9wRIuzO8s/ugxN0/r16yeazc+9Zs2aQ+onTGZFSkpKGkcJdrt95syZY8aMqaqqCk8G33bx
DWjEunXrGt/0+XxbtmxRVTV8bakmZPaRmG3aOApR9qPW7pKQkYrZwG63i2anBK5fvz7mGsWx
R4Qfbty4cWvWrPnggw+8Xm9k+v8TTzzxm2+++eabbzZv3nyo57UlScwVTOoLYHzbW8zhTtRK
tf2BAAAAgA4lvYMkh8Px5JNPKopyzz33/PrXv278+/O+ffuuvfbaW265JScn54knnggvDCdK
d955p9/vj7S88847g8HgRRdd1PaDR959993wtKlhTz/9tN/vHz9+fE5Ojs1m69Kli8fjiRxF
YprmvHnzwhOphg+4SKDw18sFCxZElnz88cfPPfdclLtIVijTc/h5njt3bvgQlbD333+/a9eu
4YuRxf3oMqZMmSKEuP/++yNLdu7c+eSTT8r3EBFzRb744ovDDz/84osvbrxF1dbW7tixQ9O0
oqIi8WP60Pwom0MSx4BGvPvuux9++GHk5sKFCxsaGk466aTwFGNNyOwjMm3aMgpR9qPW7tL2
kZIZyvCxP+HLuocbbNq0KXzJreji2CPCTjvttIqKivCr3IQJE8ILTzzxRNM077nnHhF1gqSE
bHiSYq5gW3ZwmRU51O1NZrgTslIJeSAAAACgQ0nvU9uEENOmTXvxxRd//etfP/XUU4sXLx48
eHBRUdHevXu3bt3q9/t79er16quvDhgwINz4kksuWbJkycsvv3zcccdNnjzZYrGsW7fu3Xff
Pfroo+++++62F3PxxReffvrpZ5111lFHHfXtt9/+85//tFgsd955Z/i/l19++f3333/KKadc
dtllQojly5dXVlYuXrx40qRJL7zwQq9evS666KK21xB2/fXXP/vss4899lhJScnIkSNLSkqW
LFlyyy233HDDDVHuJVOhTM/nnXfe0qVLn3/++WOPPfb88893uVxfffXVsmXLHA5H4wvYx/Ho
Muv+xz/+8R//+Me///3vHTt2jB49+sCBA6+//voVV1wxf/582adPekWGDh164YUXPvfccwMG
DJg8eXJ+fn55efmrr766a9eu3/3ud+G5fgcMGKAoyquvvjpjxgyr1frII48cahki3gENBoNC
iBkzZkyePHn69OlHHHHEpk2bXnzxRZvNdscdd7R4F5l9RKZNW0Yh+n7UoraPVH5+fsyhPPvs
s2+88cZVq1aNHTt21KhRe/fuXb58+e233z579uzw/FBxl9ea008//YYbbvjPf/4TniApvHDk
yJE2m+3555+3Wq2Rw5SaS8iGJ0lmBePewWVW5FC3N5k9N1ErlZAHAgAAADoQMyOUl5fPmzdv
1KhRBQUFuq7n5eWNHz/+iSeeaGhoaNIyEAg8+OCDw4cPdzqdNputuLj4pptuqqysjDS46667
hBD33ntv43uFjwXYtGlTZEn40s59+vQJ3wyfW/fwww+/8847EyZMyM7Ozs7OnjBhwurVqxvf
Zc6cOUceeaTNZuvVq9c111xTXl5umubll1+elZXVrVu3L7/8ssVHD4cFjzzySJQKv/32WyHE
0KFDI0s2bNhw2mmnuVyunJycCRMmrFixYuPGjUKIiRMntvY0ylQo2XMoFFq4cOHo0aNdLpeu
6z179rz00ksbP4HxPbrkum/atOnMM890u912u33w4MELFy4MH85wwgkntPboLfYssyKhUOih
hx4aM2ZMQUGBpmm5ubknnnjiokWLDMOItLn77rsLCgpsNtvw4cPNdhzQ3//+90KIF198ceXK
lePHj8/Ozs7KypowYcL7778faRPedBcsWBBZEnMfkWwTxyjI7EfJGymZody4cePJJ5/sdDqz
s7NPOOGEpUuXho8iiYxC3OW1yDCM8EErs2bNarx83LhxzYe+yXZlNtvwJLe0JiTvFXMF497B
m69Ii2Jub02eH5nhTshKJeSBAAAAgI7jh+sroY1uueWWO+64Y8GCBbNmzUp1La1at27dqFGj
pk6dunz58nTpGVFk3tOeFvsRAAAAAHRm6T1HElqzf//+1157rcnUsxs2bBBC9O3bt2P2jCh4
2gEAAAAAHQFBUmZ6++23p06devXVVwcCgfCS6urq++67Twgxbdq0jtkzouBpBwAAAAB0BGk/
2TZadN555z322GNr1qw59thjp0yZUl9f//LLL+/atWv69OltvF548npGFDztAAAAAICOgCOS
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
onh7ftEzJeU1lz85zHG6bs8vWlVe6U9wQghdVKD9aB2bnUUa796CoDh9UvefdXRNlT/BRUIe
KixZXFTauIpECClycQ8UljxeXOrphRLRFWW6j/6pOHfmsuRFkT2fqf3wPaasxPNLJVH9sEv9
xebGVSRCCLFZVbu+Uu/YSkL7gBBUVFWV9v3XL6si1XM61V/+L8TPU2Ucd8XZrENWGxEJafQZ
2kVxeXH5w0X+7pZfmeuuyc771fpHFYkQ4hTEdZXVM7Lzqjw0AYBO7qLTNfVC3qYac+MrDZGQ
72otUy/kHbLavLwW2qmoqKhhw4Zt3bq1puaPs8yHH374xBNPcBxXP8l7UlJSw6q3337bbrd7
akZECKEoihDCcW6u91JTU2NiYr7++uuGtjznzp07fvx48y0PHz48f/78xtWDqVOnEkLKy8v9
SVh22Cbp6fX6/v37f/HFF7W1tfVLMjMzU1NT165dG6QEvLyw+bsnj6QWSdu2bVu3bt3ChQsb
L7zrrrsee+yxdevWvf32255euG/fvnXr1g0aNCgrK6vx8rq6urvuuquheNbQUu61116rq6tb
sWKFSqX65JNPnn322ddff53GMxDoNFR7v2MvXvC4ds83fEwsnyqzBT5lqdNs+5y6NFRek5W0
qUaz7XPrLXfIflit+vlHxZnfCCFuX688uF+INaJdUjDsMNe+VFbhZe3LZcplxpjWTEk6piBP
/d1XHtfm5ah27bRPnSk7/oMnfzumc9++w0HT97v4niXFPeIT5AU/W1J8v4s4PJykjmrDHj75
2z+HD5MXPNgos0n9v00U53K7lq6q1Pxvk3X+rbIPCC+VVXxprvW09sXSij4q1fRwme2GKJtN
u+VTym53v7bWrNnymWXhnbKbs71fWf1xtcfC+vuVNX3V6gVy2yVRHKfZ8qmnOh1ls2m2fGr5
y72iQuaTfPb0SeXPP7qJTAghRHHmpBAT6xwxWl7w9k73yQeUu3sVQgghovLgfj4llevarVVz
kmx6dl4df+levdn38qOqmpFazTxDuLzg2U7nPQXFDg9FxjN2xz0FxZ+lJLldC52WSxQX5hUW
utyfR0w8f2te0Y/dUw3oVNvhvPzyy1OmTBk3btzf/va3+Pj4ffv2vfTSSwsWLGBZNiMjIzk5
+b333hs4cGB0dPSWLVsOHz48fvz4w4cP79mzZ9gwNxdF9cM/v/DCC3379p07d27jVTRN33vv
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
hMfHjPzc3uaDmvbpq5yIERFNcLv+MnqkyNAjCQAAACAjbPVImjt37rZt2wa+/txzz02dOjXd
KQEAAACYmepxv1Fbc2VRgXy4YMTIw9jNpUWvj6+plm2tJQIAAAAADtg601q7dm04HO73oqZp
W7Zsqa+vz0BWAAAAAGZGyNIDo6p+UlWxLhILGEaJKM71eb1YrA0gVzUr6u86upYFwy2aJhFN
9rgvLyy4sbTIg/mDAABDjUUhif17z37CCSckHDB79uw0ZwQAAABgT6Eonp7vH+wsAMDCC73B
/2rZHzV43x91og3R2IZo7JGunsdrRk60sRQjAADkDotC0vr16995553bbrvt4osvLisrO3IT
Y6y6uvrmm2/OZHoAAAAAADCEvRUK37yvNeGmPYpy5d7m5bU15ZKY5awAAMAxi0LSzJkzZ86c
+corr/ziF7+YOHFidnICAAAAAIBjQJzz/249aDKgRVXvOdD261FVWUsJAABSZKvZ9muvvTZy
5Mj9+/f3/TEajT7yyCP33nvvnj17MpkbAAAAAAAMYcsDoWZFNR/zXCAY0I3s5AMAAKmzVUja
vn37uHHjHn30USLSNG3RokU33njj7bffPnv27E8++STDGQIAAAAAwJC0KhK1HKMYfF3UehgA
AOQIW6u2ff/736+srLzyyiuJ6Omnn16zZs0DDzywZMmS66+//sc//vGzzz6b4SQBAABy135V
e6E3uDkWDxlGtSSenu9fnJeH1cP6rIxEXw+E9qqqi1idx3VhQX4duupmxbZY/KVAcHdcUTmv
dbvPyffP9XkHOykYjroNW1ONunQ905kAAEC62Cokvf/++0uXLq2trSWi559/fvr06V/96leJ
6NZbb73jjjsymyAAAECu4kS/au9c2tYZ5/zwi3/q6pnidv1hzMgpw7ticlDTvta8/91Q5NOX
evkv2zqvKS78cVWFGwt+Z0zEMP7f/rZnunuPeC10f3vn4nz/b0dVlYpoaQxZVSLaegCiDN9M
AIChw9aevaenp6qqioh0XV+xYsV5553X93p5efnBg2bN8wAAAI5h3249+NODHXHe/377trhy
Xn3j1lh8ULLKBW2adu6eps9UkYiImMb5Y1091zQ2q0eU3iCN4pxfsXffZ6tIh7wRDJ+/p6lb
w7wPyKoFPp/lGDdjczBjDgBg6LBVSKqsrOzrq/3WW291d3efc845fa/v27evtLQ0g9kBAADk
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
/vnn+3w+IUQkElm2bFlTU9PYsWM3bdrkcrkmTpzY16y8vLypqWnDhg2OFgtACCFef/31zZs3
X3bZZf1bOGCBwpROp5PJ5Ouvv37zzTdfc801P/7xj1taWgTHLFCQOjs7d+/eLYS48cYbL774
4m984xvr168XHLAAQJCEAZmmeeGFF15++eU7d+78wQ9+4HK5wuFwIBCQUva3qaysDIVCDhYJ
QAgRjUbvvvvur3zlK16vt38jByxQmGKxWDAY1HX9hhtu+OY3v5lKpb797W/39vZyzAIFqLOz
Uwjx7LPP3nLLLffee29zc/P3vve9UCjEAQsABEkYgKIod955549+9KOKiopbb701Go0KIfb9
vARQIO655545c+YceeSRB2zngAUKUGVl5QMPPPC1r31t6tSpU6dOveWWWxKJxGuvvSY4ZoFC
demllzY1NQUCgauvvlpK+eabbwoOWAAjHkESBtbU1HT44YffcsstoVBo+fLlwWAwHA7vuzR7
KBSqqqpysEIAb7/99ltvvXX11VcfsJ0DFigKPp+vrq6uo6ODYxYoQH1LmJWVlfU9VFW1urq6
u7ubAxYACJKwn1WrVl1//fXJZLLvoZRS0zQhxGGHHZZOpzdv3ty3PRwO79y5c/r06Y4VCkCI
Z555pre3d9GiRZdffvnll18eCoVuv/32H//4xxywQGHavn37//zP/+i63vcwkUi0t7ePHj2a
YxYoQNXV1VVVVX3rIgkhUqlUe3v7qFGjOGABQF28eLHTNaCABAKBxx9/fMuWLePHj4/H4488
8siGDRuuvfbaurq67du3v/DCC83NzbFY7Fe/+lVZWdnll1/OyF7AQbNnzz5zHy+++OIXv/jF
888/PxgMcsACBUhV1bvvvrulpWXChAmhUOjXv/51NBr98pe/HAgEOGaBQiOlNAzjz3/+86RJ
kzRNu//++9va2r70pS9xwAKA3HdYJiCE2L59+3333bd27Vop5bhx46644oojjjhCCBGLxZYs
WbJq1SrDMGbOnLlo0SIG8QIF5fOf//wNN9ywYMECwQELFKotW7bcd999fXd9am5uvu6660aN
GiU4ZoGCZJrmH/7wh2effTYajTY3N99www1jx44VHLAARjyCJAAAAAAAANjCGkkAAAAAAACw
hSAJAAAAAAAAthAkAQAAAAAAwBaCJAAAAAAAANhCkAQAAAAAAABbCJIAAAAAAABgC0ESAAAA
AAAAbCFIAgAA+wmHw+Xl5VLKpUuXOl0LAAAACgtBEgAA2M+DDz7Y29tbVVX129/+1ulaAAAA
UFikZVlO1wAAAArInDlzhBAnnnjiL3/5y23btjU1NTldEQAAAAoFI5IAAMBH3nzzzVWrVn32
s5+94oorDMO4//77991rmubixYvHjh3r9Xrnzp37zDPPfPWrX3W73f0Nli9ffvrpp1dUVPj9
/jlz5tx77735/gUAAAAwnAiSAADAR37zm9+oqnrFFVfMnTt39uzZ9957776Dl3/yk59873vf
O+aYY5YtW3bDDTdcddVV//rXv/qDpOeee+7UU09NpVIPPfTQ448/Pn/+/Guuuea///u/HfpV
AAAAkHtMbQMAAHtFo9HGxsbjjz/+qaeeEkLceeedN9988zPPPHPaaacJISzLamhoqKure+ed
d6SUQogVK1YsWLCgrKwsGo0KIebMmROJRFavXu33+/s6PO+881544YW2tjav1+vcrwUAAICc
YUQSAADY65FHHolEIldffXXfwyuuuMLtdt9zzz19D3fv3r1nz57TTz+9L0USQsyfP3/WrFl9
/9/W1rZq1aqzzz5bUZTEh84666xIJLJmzZr8/y4AAAAYDgRJAABgryVLllRWVh5zzDEdHR0d
HR2WZS1cuHDp0qVdXV1CiD179gghGhoa9v0nzc3Nff/T2toqhLjzzjt9+1i0aJEQ4oMPPsj3
bwIAAIDhoTldAAAAKAirV69euXKlEKKxsfGAXb///e9vuummZDIphFCU/a5C9Y9O6nP11Vdf
d911B/zzKVOm5L5cAAAAOIEgCQAACCHEkiVLhBAPP/xwbW3tvtuvuuqqe+6556abbqqurhYf
jkvqt2HDhr7/GTdunBDCMIwFCxbkqWIAAADkHYttAwAAEY/HGxoaZsyY8dprrx2w69vf/vZP
fvKTFStWzJkzp7a2duzYsf1rHq1cufLoo4/uX2x7/vz5GzZs2LZtWzAY7GvwwAMPbNy4cfHi
xZrGtSsAAIBSwBpJAABAPProo6FQ6Jprrjl4V9/a27/97W81TbvmmmvefffdL37xi//85z+X
LFlyySWXHHvssf0tf/azn8VisRNPPPGBBx745z//+V//9V/XXnttS0sLKRIAAEDJYEQSAAAQ
xx577OrVq3fv3l1eXn7w3hNPPHHVqlW7du3SNO0///M/H3744Xg8PmfOnJ///Od33nnnsmXL
IpFIX8tXXnnl+9///htvvJFIJCZOnHjttdd+7WtfI0gCAAAoGQRJAAAge6eddtratWv7btkG
AACAksfUNgAAYNcdd9xx4YUX6rre97Cnp+fNN9888sgjna0KAAAAecNQcwAAYFdNTc1jjz12
/vnnX3fddYlE4o477giHw1//+tedrgsAAAB5QpAEAADsuvLKK4UQt99++2WXXWZZ1pFHHvnk
k0+eeuqpTtcFAACAPGGNJAAAAAAAANjCGkkAAAAAAACwhSAJAAAAAAAAthAkAQAAAAAAwBaC
JAAAAAAAANhCkAQAAAAAAABbCJIAAAAAAABgC0ESAAAAAAAAbPn/5AYruVUBln4AAAAASUVO
RK5CYII=" width="780">
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=c1e70fd7-d006-4258-aa58-3e618d3980d0">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><em>Plot 1: Plotting age vs resting blood pressure</em></p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=636f7c06-0a48-4eed-9bd9-07967c4d9ee2">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h5 id="Explanation-of-Data-Graph:">Explanation of Data Graph:<a class="anchor-link" href="#Explanation-of-Data-Graph:">¶</a></h5><p>From reading the graph there seems to be no real relationship between the variables blood pressure and heart disease. Patients diagnosed with heart disease are predominantly found within the age range of 45-60 hence, we can establish the connection between age and heart disease cases.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=d1967f93-66a7-4c3d-96d8-f7a155417845">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h5 id="Forward-Selection:">Forward Selection:<a class="anchor-link" href="#Forward-Selection:">¶</a></h5><p>We begin our analysis by finding the most accurate model and best predictors for heart disease, hence, our reason for performing the forward selection process. We first extract the column names, and then create an empty tibble to store the results.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=14e3a529-aaf7-4353-9251-90493d261213">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[91]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">names</span> <span class="o">&lt;-</span> <span class="n">colnames</span><span class="p">(</span><span class="n">heart_disease_hungarian</span> <span class="o">|&gt;</span> <span class="n">select</span><span class="p">(</span><span class="o">-</span><span class="n">heart_disease_cases</span><span class="p">))</span>

<span class="n">accuracies</span> <span class="o">&lt;-</span> <span class="n">tibble</span><span class="p">(</span><span class="n">size</span> <span class="o">=</span> <span class="n">integer</span><span class="p">(),</span> 
                     <span class="n">model_string</span> <span class="o">=</span> <span class="n">character</span><span class="p">(),</span> 
                     <span class="n">accuracy</span> <span class="o">=</span> <span class="n">numeric</span><span class="p">())</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=37fee5e0-0a47-4464-ad5d-e0c7905f82d8">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Next, we create our model specification and perform our 5-fold cross-validation. To perform forward selection, we also must store the number of predictors, and store the selected predictors.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=225fb91d-b71a-4995-99d4-dd95277bf369">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[92]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">set</span><span class="o">.</span><span class="n">seed</span><span class="p">(</span><span class="mi">27</span><span class="p">)</span>
<span class="n">knn_spec</span> <span class="o">&lt;-</span> <span class="n">nearest_neighbor</span><span class="p">(</span><span class="n">weight_func</span> <span class="o">=</span> <span class="s2">"rectangular"</span><span class="p">,</span> 
                             <span class="n">neighbors</span> <span class="o">=</span> <span class="n">tune</span><span class="p">())</span> <span class="o">|&gt;</span>
     <span class="n">set_engine</span><span class="p">(</span><span class="s2">"kknn"</span><span class="p">)</span> <span class="o">|&gt;</span>
     <span class="n">set_mode</span><span class="p">(</span><span class="s2">"classification"</span><span class="p">)</span>

<span class="n">heart_disease_vfold</span> <span class="o">&lt;-</span> <span class="n">vfold_cv</span><span class="p">(</span><span class="n">heart_disease_hungarian</span><span class="p">,</span> <span class="n">v</span> <span class="o">=</span> <span class="mi">5</span><span class="p">,</span> <span class="n">strata</span> <span class="o">=</span> <span class="n">heart_disease_cases</span><span class="p">)</span>

<span class="n">n_total</span> <span class="o">&lt;-</span> <span class="n">length</span><span class="p">(</span><span class="n">names</span><span class="p">)</span>

<span class="n">selected</span> <span class="o">&lt;-</span> <span class="n">c</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=87c0f9e6-4ac6-4cb6-b899-bac1e16aa37e">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>The following code is taken directly from the textbook as forward selection goes beyond our knowledge in DSCI100</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=01a10985-6847-44c0-a93f-99aeb9de6d94">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[93]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">set</span><span class="o">.</span><span class="n">seed</span><span class="p">(</span><span class="mi">27</span><span class="p">)</span>
<span class="c1"># for every size from 1 to the total number of predictors</span>
<span class="k">for</span> <span class="p">(</span><span class="n">i</span> <span class="ow">in</span> <span class="mi">1</span><span class="p">:</span><span class="n">n_total</span><span class="p">)</span> <span class="p">{</span>
    <span class="c1"># for every predictor still not added yet</span>
    <span class="n">accs</span> <span class="o">&lt;-</span> <span class="nb">list</span><span class="p">()</span>
    <span class="n">models</span> <span class="o">&lt;-</span> <span class="nb">list</span><span class="p">()</span>
    <span class="k">for</span> <span class="p">(</span><span class="n">j</span> <span class="ow">in</span> <span class="mi">1</span><span class="p">:</span><span class="n">length</span><span class="p">(</span><span class="n">names</span><span class="p">))</span> <span class="p">{</span>
        <span class="c1"># create a model string for this combination of predictors</span>
        <span class="n">preds_new</span> <span class="o">&lt;-</span> <span class="n">c</span><span class="p">(</span><span class="n">selected</span><span class="p">,</span> <span class="n">names</span><span class="p">[[</span><span class="n">j</span><span class="p">]])</span>
        <span class="n">model_string</span> <span class="o">&lt;-</span> <span class="n">paste</span><span class="p">(</span><span class="s2">"heart_disease_cases"</span><span class="p">,</span> <span class="s2">"~"</span><span class="p">,</span> <span class="n">paste</span><span class="p">(</span><span class="n">preds_new</span><span class="p">,</span> <span class="n">collapse</span><span class="o">=</span><span class="s2">"+"</span><span class="p">))</span>

        <span class="c1"># create a recipe from the model string</span>
        <span class="n">heart_disease_recipe</span> <span class="o">&lt;-</span> <span class="n">recipe</span><span class="p">(</span><span class="k">as</span><span class="o">.</span><span class="n">formula</span><span class="p">(</span><span class="n">model_string</span><span class="p">),</span> 
                                <span class="n">data</span> <span class="o">=</span> <span class="n">heart_disease_hungarian</span><span class="p">)</span> <span class="o">|&gt;</span>
                          <span class="n">step_scale</span><span class="p">(</span><span class="n">all_predictors</span><span class="p">())</span> <span class="o">|&gt;</span>
                          <span class="n">step_center</span><span class="p">(</span><span class="n">all_predictors</span><span class="p">())</span>

        <span class="c1"># tune the KNN classifier with these predictors, </span>
        <span class="c1"># and collect the accuracy for the best K</span>
        <span class="n">acc</span> <span class="o">&lt;-</span> <span class="n">workflow</span><span class="p">()</span> <span class="o">|&gt;</span>
          <span class="n">add_recipe</span><span class="p">(</span><span class="n">heart_disease_recipe</span><span class="p">)</span> <span class="o">|&gt;</span>
          <span class="n">add_model</span><span class="p">(</span><span class="n">knn_spec</span><span class="p">)</span> <span class="o">|&gt;</span>
          <span class="n">tune_grid</span><span class="p">(</span><span class="n">resamples</span> <span class="o">=</span> <span class="n">heart_disease_vfold</span><span class="p">,</span> <span class="n">grid</span> <span class="o">=</span> <span class="mi">10</span><span class="p">)</span> <span class="o">|&gt;</span>
          <span class="n">collect_metrics</span><span class="p">()</span> <span class="o">|&gt;</span>
          <span class="nb">filter</span><span class="p">(</span><span class="o">.</span><span class="n">metric</span> <span class="o">==</span> <span class="s2">"accuracy"</span><span class="p">)</span> <span class="o">|&gt;</span>
          <span class="n">summarize</span><span class="p">(</span><span class="n">mx</span> <span class="o">=</span> <span class="nb">max</span><span class="p">(</span><span class="n">mean</span><span class="p">))</span>
        <span class="n">acc</span> <span class="o">&lt;-</span> <span class="n">acc</span><span class="err">$</span><span class="n">mx</span> <span class="o">|&gt;</span> <span class="n">unlist</span><span class="p">()</span>

        <span class="c1"># add this result to the dataframe</span>
        <span class="n">accs</span><span class="p">[[</span><span class="n">j</span><span class="p">]]</span> <span class="o">&lt;-</span> <span class="n">acc</span>
        <span class="n">models</span><span class="p">[[</span><span class="n">j</span><span class="p">]]</span> <span class="o">&lt;-</span> <span class="n">model_string</span>
    <span class="p">}</span>
    <span class="n">jstar</span> <span class="o">&lt;-</span> <span class="n">which</span><span class="o">.</span><span class="n">max</span><span class="p">(</span><span class="n">unlist</span><span class="p">(</span><span class="n">accs</span><span class="p">))</span>
    <span class="n">accuracies</span> <span class="o">&lt;-</span> <span class="n">accuracies</span> <span class="o">|&gt;</span> 
      <span class="n">add_row</span><span class="p">(</span><span class="n">size</span> <span class="o">=</span> <span class="n">i</span><span class="p">,</span> 
              <span class="n">model_string</span> <span class="o">=</span> <span class="n">models</span><span class="p">[[</span><span class="n">jstar</span><span class="p">]],</span> 
              <span class="n">accuracy</span> <span class="o">=</span> <span class="n">accs</span><span class="p">[[</span><span class="n">jstar</span><span class="p">]])</span>
    <span class="n">selected</span> <span class="o">&lt;-</span> <span class="n">c</span><span class="p">(</span><span class="n">selected</span><span class="p">,</span> <span class="n">names</span><span class="p">[[</span><span class="n">jstar</span><span class="p">]])</span>
    <span class="n">names</span> <span class="o">&lt;-</span> <span class="n">names</span><span class="p">[</span><span class="o">-</span><span class="n">jstar</span><span class="p">]</span>
<span class="p">}</span>
<span class="n">accuracies</span>
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
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output" data-mime-type="text/html" tabindex="0">
<table class="dataframe">
<caption>A tibble: 4 × 3</caption>
<thead>
<tr><th scope="col">size</th><th scope="col">model_string</th><th scope="col">accuracy</th></tr>
<tr><th scope="col">&lt;int&gt;</th><th scope="col">&lt;chr&gt;</th><th scope="col">&lt;dbl&gt;</th></tr>
</thead>
<tbody>
<tr><td>1</td><td>heart_disease_cases ~ maximum_heart_rate_achieved                                       </td><td>0.6673045</td></tr>
<tr><td>2</td><td>heart_disease_cases ~ maximum_heart_rate_achieved+cholesterol                           </td><td>0.6819147</td></tr>
<tr><td>3</td><td>heart_disease_cases ~ maximum_heart_rate_achieved+cholesterol+age                       </td><td>0.6816378</td></tr>
<tr><td>4</td><td>heart_disease_cases ~ maximum_heart_rate_achieved+cholesterol+age+resting_blood_pressure</td><td>0.6778769</td></tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=71a5f103-f209-488c-b61e-42af384a8cc9">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><em>Table 4: Accuracy estimates produced using forward selection</em></p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=c90b1772-dc2e-4104-b4eb-bdc7cde9a94f">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[96]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">accuracy_vs_k</span> <span class="o">&lt;-</span> <span class="n">ggplot</span><span class="p">(</span><span class="n">accuracies</span><span class="p">,</span> <span class="n">aes</span><span class="p">(</span><span class="n">x</span> <span class="o">=</span> <span class="n">size</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">accuracy</span><span class="p">))</span> <span class="o">+</span>
  <span class="n">geom_point</span><span class="p">()</span> <span class="o">+</span>
  <span class="n">geom_line</span><span class="p">()</span> <span class="o">+</span>
  <span class="n">labs</span><span class="p">(</span><span class="n">x</span> <span class="o">=</span> <span class="s2">"Number of Predictors"</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="s2">"Accuracy Estimate"</span><span class="p">,</span> <span class="n">title</span> <span class="o">=</span> <span class="s2">"Estimated Accuracy vs Number of Predictors"</span><span class="p">)</span> <span class="o">+</span> 
  <span class="n">theme</span><span class="p">(</span><span class="n">text</span> <span class="o">=</span> <span class="n">element_text</span><span class="p">(</span><span class="n">size</span> <span class="o">=</span> <span class="mi">12</span><span class="p">))</span>

<span class="n">accuracy_vs_k</span>
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
<img alt="No description has been provided for this image" class="" height="420" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAABhgAAANICAMAAAACehXjAAADAFBMVEUAAAABAQECAgIDAwME
BAQFBQUGBgYHBwcICAgJCQkKCgoLCwsMDAwNDQ0ODg4PDw8QEBARERESEhITExMUFBQVFRUW
FhYXFxcYGBgZGRkaGhobGxscHBwdHR0eHh4fHx8gICAhISEiIiIjIyMkJCQlJSUmJiYnJyco
KCgpKSkqKiorKyssLCwtLS0uLi4vLy8wMDAxMTEyMjIzMzM0NDQ1NTU2NjY3Nzc4ODg5OTk6
Ojo7Ozs8PDw9PT0+Pj4/Pz9AQEBBQUFCQkJDQ0NERERFRUVGRkZHR0dISEhJSUlKSkpLS0tM
TExNTU1OTk5PT09QUFBRUVFSUlJTU1NUVFRVVVVWVlZXV1dYWFhZWVlaWlpbW1tcXFxdXV1e
Xl5fX19gYGBhYWFiYmJjY2NkZGRlZWVmZmZnZ2doaGhpaWlqampra2tsbGxtbW1ubm5vb29w
cHBxcXFycnJzc3N0dHR1dXV2dnZ3d3d4eHh5eXl6enp7e3t8fHx9fX1+fn5/f3+AgICBgYGC
goKDg4OEhISFhYWGhoaHh4eIiIiJiYmKioqLi4uMjIyNjY2Ojo6Pj4+QkJCRkZGSkpKTk5OU
lJSVlZWWlpaXl5eYmJiZmZmampqbm5ucnJydnZ2enp6fn5+goKChoaGioqKjo6OkpKSlpaWm
pqanp6eoqKipqamqqqqrq6usrKytra2urq6vr6+wsLCxsbGysrKzs7O0tLS1tbW2tra3t7e4
uLi5ubm6urq7u7u8vLy9vb2+vr6/v7/AwMDBwcHCwsLDw8PExMTFxcXGxsbHx8fIyMjJycnK
ysrLy8vMzMzNzc3Ozs7Pz8/Q0NDR0dHS0tLT09PU1NTV1dXW1tbX19fY2NjZ2dna2trb29vc
3Nzd3d3e3t7f39/g4ODh4eHi4uLj4+Pk5OTl5eXm5ubn5+fo6Ojp6enq6urr6+vs7Ozt7e3u
7u7v7+/w8PDx8fHy8vLz8/P09PT19fX29vb39/f4+Pj5+fn6+vr7+/v8/Pz9/f3+/v7////i
sF19AAAACXBIWXMAABJ0AAASdAHeZh94AAAgAElEQVR4nO3dCXxTVd7/8V9XoOy7gIC4MaiI
Di7jjIorOkoLiIKiVhFxYbSuiMrTcdRRHLV/N1xGRHBAHaWu4zaKgCIggsguWHYopa3jgguy
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" width="780">
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=6cfc4271-0b1a-4c26-9672-05bb4671fc8e">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><em>Plot 2: Finding the optimal number of predictors</em></p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=1c7ebc2e-71dc-42c0-a4b4-d7c095cbe24b">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Notice that the number of predictors is estimated to be the most accurate at two predictors.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=7fe01c2f-0cc4-475e-b887-32fd54ec4d06">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[98]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">options</span><span class="p">(</span><span class="nb">repr</span><span class="o">.</span><span class="n">plot</span><span class="o">.</span><span class="n">width</span> <span class="o">=</span> <span class="mi">13</span><span class="p">,</span> <span class="nb">repr</span><span class="o">.</span><span class="n">plot</span><span class="o">.</span><span class="n">height</span> <span class="o">=</span> <span class="mi">7</span><span class="p">)</span>

<span class="n">heart_disease_plot_best</span> <span class="o">&lt;-</span> <span class="n">heart_disease_hungarian</span> <span class="o">|&gt;</span> 
    <span class="n">ggplot</span><span class="p">(</span><span class="n">aes</span><span class="p">(</span><span class="n">x</span> <span class="o">=</span> <span class="n">maximum_heart_rate_achieved</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">cholesterol</span><span class="p">,</span> <span class="n">color</span> <span class="o">=</span> <span class="n">heart_disease_cases</span><span class="p">))</span> <span class="o">+</span> 
        <span class="n">geom_point</span><span class="p">(</span><span class="n">size</span> <span class="o">=</span> <span class="mi">3</span><span class="p">)</span> <span class="o">+</span>
        <span class="n">labs</span><span class="p">(</span><span class="n">x</span> <span class="o">=</span> <span class="s2">"Maximum Heart Rate Achieved"</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="s2">"Cholesterol"</span><span class="p">,</span> <span class="n">color</span> <span class="o">=</span> <span class="s2">"Heart disease cases"</span><span class="p">,</span> <span class="n">title</span> <span class="o">=</span> <span class="s2">"Associating maximum heart rate and cholesterol with Heart Disease"</span><span class="p">)</span>

<span class="n">heart_disease_plot</span> <span class="o">&lt;-</span> <span class="n">heart_disease_plot</span> <span class="o">+</span> 
       <span class="n">scale_fill_brewer</span><span class="p">(</span><span class="n">palette</span> <span class="o">=</span> <span class="s2">"YlOrRd"</span><span class="p">)</span>
<span class="n">heart_disease_plot_best</span>
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
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="application/vnd.jupyter.stderr" tabindex="0">
<pre>Scale for 'fill' is already present. Adding another scale for 'fill', which
will replace the existing scale.

</pre>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" height="420" src="data:image/png;base64,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
rYIg+OCDDzp8tsvtpKcWsEdmBADAgNTvg6RMJnPzzTdHo9HsNQVZJ5xwQhAEN998c+uen/3s
ZzOZzD777HPbbbe1jIeavRYjTIdMJvPSSy8FQTBr1qzWky0tLZ06dWp9ff3f//73IAj++Mc/
BkGw8847t+5z5plnXn311Ztttln7+jfddNPDDjtsl112CYKgsrJy+fLly5cvT6fTQRCE+TrX
WvayghZDhw5tmUhzc/Obb74ZjUazF020aLliqHNtXlVaWhoEwXbbbdempaXgkAs1Y8aM888/
/+mnnz7kkENeeOGF7373u1tvvXXPVhJeT025zVrI5lDl5eXZh88//3zQbhMaMmTINttss2zZ
suxXx/CbxAZ9P+/khd3bCMMsS3vh59X59vzGG28EQbD99tu37tPJaF9ZIXfPTlZiyONAG2He
qy4PUN2bbFbrNd69RWhj9OjR22233Z/+9KempqYgCF544YWqqqpZs2bNnj37rbfe+uijj4Ig
+Pjjj99444399tuv83S4jc73oPWpqalZuB7ZClvkyT7YiezllpWVlR0+2+V20lML2CMzAgBg
QNqAz/f56be//e2777574IEHbrLJJi2NRx555BlnnHHXXXf94Ac/aPlB9frrr29qarrttttO
PPHEIAi22mqrOXPmzJ07d/LkyWE6rF27tra2NplMlpWVtalh5MiRQRCsXLmyqqqqqqoqlUpl
LxkL6aGHHrr66qtfeumlDgcIDy97XU+L7A/mmUwmW3x9fX1ZWVkikWjdZ9KkSWGmPGLEiPZT
bt3Yel5ZIRfqO9/5zoMPPvjb3/52p512yl671OOVhNRTU85uDC2i0WjLq2pqatauXRv8+4ti
e0uWLMluxiHfvTbzCq/9Czd0Iwy/LO2FnFeX23P7HW348OGdTDD87tnJSgxzHGjTHvK96vIA
1b3Jtl+ibixChw444ICrr7765Zdf3mWXXZ588slIJLLXXnstXrw4CIKnn376iCOOeOqpp4Ig
+PSnPx1mam1qaNH6ze/ElClT3nnnnQ6fKi4ubhn+OX/2wU6sWrUq+HeC1l7n20kPLmBPzQgA
gIGn3wdJN910UxAEv/vd77LfM9u4++67TzrppOz/E4nEvHnzLrnkkkceeeSxxx77/e9//4Mf
/OD666+/8847jzjiiC47dJIjNDc3B0EQiUSy33myo/x0WE97t9xyyymnnFJSUjJ37txdd921
rKwsGo0+9NBDbU6n2kjZstuXFLLIDRV+oZYvX5795pm9bfb48eN7o548kX23I5FIdnyf9rLR
Sfh3r00sGF6bF3ZjIwy5LO31yAaf3Z7b74xtzj1poxu7Z3thjgMdvqTL96rLA1T3JpvVeo13
YxE6lA2SnnnmmV122eX3v//91ltvPWLEiGHDhpWWlmaDpCeffDIIgh6/8mtj5M8+2IkXXngh
CILsiEXthfk71SML2CMzAgBgQOrfQdLixYsfffTRIUOGZAd3aK2qquqBBx64+eabW4KkrLFj
x55yyimnnHJKbW3t7bff/s1vfvOUU0459NBDW8YKWV+H4uLidDpdXV29Zs2alltoZ61YsSII
gpEjRxYWFpaUlFRWVq5atarNGS7rk71B1YIFC2bPnt3S2MmoKN1TXFwci8UqKyubmppaBsUI
giAb4vS48At14oknrl279oorrrjgggu+9rWvtbm39Mbr8DvzsmXLenYuIaVSqbKysvLy8lNP
PbWTExn6ZpPYyDmGXJYemVd72e25rq6upqam9elFLRfgdKgbu2eHs+7yONDmJRv0XnV5gOre
ZDdyETo0e/bsVCr1zDPPnHrqqc8999zXvva1IAii0eisWbOywyQ99dRTW2yxRYeX9OZK3u6D
Lerr6+++++4gCA4++OBOuq1vO+nxBdzIGQEAMCD17zGSbr755qampuOPP/72dn75y19Omzbt
pZde+stf/pLtvGjRotYJQiqVmjt37qxZs9asWfPee++F6ZAdUSI7zEqL1atXv/XWW4WFhdnx
fbJ9nnjiidZ9rrjiiv333/9Pf/pTm/rr6uqWLFlSXFzc+tN8JpP5zW9+0wPvTiuxWGzy5MlN
TU3ZW9q16PEZBRuyUDfffPPjjz9+6qmnnn/++SeccMJvfvOb7OitPSiVSgVB8Mknn7RufPHF
F3t2LuFlB/FpGaK4xerVq7P/6bNNokW359jlsvTgvNqIxWJbbLFF0G587meffbbzF27Q7tn5
RDo/DrQR5r3q8vjTvcn21CK0l0ql9thjj2efffaPf/xjbW1ty1j1e+655+uvv/7666+/+eab
G3pdWx/Iw32wtbPPPnvJkiXbbLPNQQcd1GGHLreTnlrAjZ8RAAADVT8OkhoaGn76058GQZD9
Jby97MgO8+bNC4Lgb3/726abbvrlL3+5vr6+pUNlZeV7770Xi8VGjRrVZYeWCV5++eWt+1x+
+eWNjY3HHHNM9pSB4447LgiCq6++umVUjvfff/+qq6567rnnpk+f3qbCgoKCYcOGrV27tuXM
oEwmc9lll2WHKV2zZk22MZuGZAfO6LbsN7obb7yxpeWFF17I/vTds0Iu1KJFi84555xNNtkk
exftq6++etSoUWeddVaXt2faINmzIbI3tM62vPHGGz0eV4WX3YQuvfTS7KkfWX/4wx9Gjx6d
vStZyHevQ93bTrq9EXa5LN2eVxjZ8zWuvfbalpZ//vOf2QNCJzZo91yfMMeBDl/SyXsV5vjT
I6ug24vQoQMOOGDVqlU//elPswMkZRv33HPPTCbzgx/8IOh0gKQeOax1Qx7ug1kffvjhMccc
c+ONN6bT6Z///OcdXmAY/u/URi5gj8wIAICBqh9f2vbggw8uX758jz32yN4sub3jjjvuwgsv
vPfee6+55prtt9/+S1/60t133z19+vSDDjpo+PDhK1eufPTRRz/88MMzzjhj+PDhw4cP77xD
EARf+cpX5s+f//DDD++8884HHXRQIpH485//vHDhwi233PLKK6/MzvQrX/nKAw88sGDBgq23
3vqggw6qqqp66KGHKisrb7311uxtp9r46le/eu211+63337Zr7gLFiz45JNP7rjjjk9/+tP3
3nvvxIkTjznmmOnTp0cikUcfffTEE09MJpPZYaE21Nlnn33XXXfdfPPNixYt2nXXXRctWjR/
/vyLLrrovPPO68bUOtflQn3pS1864YQTKisr77333uxYrUOHDr3hhhuOPvro448/fuHChT01
eNMXvvCF7I3hPvWpT+2+++7Lli1bsGDBJZdccs4552SHg+ljRxxxxEMPPXTPPffsuOOORx55
ZElJyf/+7/8+8sgjhYWF55xzTrZPmE2iw4l3ezvp3kYYZlm6N68wNZ911lk///nP77///vfe
e2/mzJkrVqx47LHHTjrppKuvvrqTV23o7rm+iXR5HGijy/eqywNU0NH67d4q6N4idOjAAw88
77zzHnjggewASdnGXXfdtaCg4J577kkmky2nKbXXI4e1bsiTfXD58uWHH3549v/19fWLFy9+
9dVXm5ubx48ff//99++4444dvirMdtJTC9gjMwIAYGDK9FvZryh33HFHJ32yv4veeOONmUym
qanpRz/60axZs0aMGBGLxcrKyvbcc8/bbrutubk527nLDplMpqGh4frrr99pp53S6XRBQcG0
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
jxx++khXsQEAQD/magIAAAAAQhEkAQAAABCKIAkAAACAUARJAAAAAIQiSAIAAAAgFEESAAAA
AKHEO3lu2rRpYSbx5ptv9lAxAAAAAOSvzoKkESNG9FkdAAAAAOS5zoKkZ599ts/qAAAAACDP
dRYktbFq1arnn39+6dKl0Wh0woQJs2bNKikp6b3KAAAAAMgroQbbbm5uPvvss8eOHTtnzpyT
Tz75a1/72mc+85mxY8deddVVvV0fAAAA0KsuvfTSSCTy/PPPt38qlUrtv//+fV9Se0cddVRx
cXH2/7vvvnvIYZ3pcaHOSLrmmmuuueaaww47bM6cOWPHjm1ubl6yZMn8+fPPPffc0aNHH3vs
sb1dJQAAADCQvPLKKzvuuGMmk+nGa4866qiampoeL4kwQgVJP/vZz/7zP//zmmuuad148skn
n3LKKTfccIMgCQAAANggf/jDH7r92jPPPLMHK2GDhLq07b333jvkkEPatx966KFvvPFGT5cE
AAAA5KOnn376gAMOKC0tTafTO+2002233db62XvvvXfXXXdNp9OlpaW77LLLvffe2/LUHnvs
MXv27AULFkycOHHWrFmf+cxnTj/99CAIIpHILrvs0n5GmUzmsssumzhxYiqV2nbbbR944IHW
z7a+tG3ZsmUnnXTSpEmTUqnUmDFjvvCFL7z55psbX/DGTLaNxx9/fK+99iopKRkzZswRRxzx
zjvv9GoBnb9w44UKkuLxeHV1dfv2hoaGWCzWg9UAAAAA+WnhwoX77bdffX393Xff/fDDD++2
224nnnhiy9VL991339FHHz1hwoRf/vKX99xzz8iRI48++uhHH300+2xBQUF5efk555xzwQUX
XHjhhTfeeOOhhx4aBMGLL7545513tp/XVVdddckll+y1114LFiy4+OKLv/vd777yyisdVvX5
z39+wYIF3/nOdx577LFrr7327bff3muvvbIhxsYU3O3JtvH4449/+tOfTqVS8+bNu/zyy196
6aXZs2cvX7689wro5IU9ItSlbTvuuOO111574IEHJpPJlsba2tof//jHHQaHAAAAQP+ybNmy
999/v01j6zGMzjnnnMmTJz/22GPpdDoIggMOOGDp0qXf/e53Tz311FQq9d577+2777733ntv
NjrYc889hw8ffs8992SvcIpEIq+++ur8+fMPO+yw7NRGjBgRBMH6Tke64YYbttlmm7vuuivb
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
MXLkyIMHDwaKe/fu3bt37/oNTJo0KT09/RIe6pJ9+umno0aNSkpKstvt11xzzaJFi7S8IEKI
QYMGDRkyZPXq1Xl5eUVFRTfeeOMDDzwghJAkqU+fPtobKCgoyMvL279/f9iDNnqI0P03sGXL
lm3btk2dOvWuu+5SFOX1119vUPDRRx8NHTrU4XBkZWXddttt9bsyGo2HDh0aM2aMw+FwOBy3
3357eXl5YFeDqW1NtTRo0KD09HSfz1f/iAMGDMjJyVEUJfRzUVX1sccey8vLs1qtPXv2fOed
dzS8tAAAAJFDkAQAaDmmTJni9/vffPPN4JaysrKPP/546tSpgT/gA95+++077rijTZs2y5cv
X7p0aevWre+44441a9YIISZMmDBjxoz58+cfOXJECFFVVfXggw9ef/31c+fObXAss9lcWlo6
f/78l19++Ztvvunfv//Pf/7zsWPH2u32zZs3r1mzpqSkJJCGhHUFH6opa9euHTFihMfjWbJk
yd///vf+/fvfe++9wbwsxAsihLBYLJWVlf/3f/83b968Rx555IUXXrjpppuEECUlJX/961+1
93D69OmTJ08G57uFOOjFhwjd/8VeeeUVg8Fw1113XXvttb169Vq0aFH9WXIfffTRDTfcYLVa
X3755ccff3zr1q1Dhgw5efJkYK+iKJMnTx4yZMibb745Z86c5cuXP/TQQ9/rJZ02bdrZs2c/
+eSTYPGRI0c2b958xx13GAyG0M/lqaeemj9//tChQ1evXv3oo4/++te/3r59u/YXGQAAoNmp
AADEvvnz5wshnE7nyJEju3fvHtz+xBNP2Gy2qqqq/v37X3fddYGNjz/++PDhw91ud+BmZWWl
0Wi88847AzcrKiry8vImTpyoqurcuXMdDkdpaWlgV//+/bt27Rr4esSIEUKI7du3B24GpmIV
FRUFD33nnXcmJCQEvi4oKCgoKKjf8E033dSqVatLeKhGn3hxcfGhi5jN5hEjRgTKCgsL8/Pz
a2trg3ecOHGiw+FwOp1hX5BAe8XFxcH73nvvvSE+QgRaWrNmzYnvlJaWvv/++3379pUkac2a
NYGy0AdtcIjQ/TdQXV3tcDjGjh0buPncc88JIT766KNgQZ8+fTp06OD1egM3N23aZDabn3/+
+UafbFFRUUZGRuDr+j8AIVo6ffq00WicNWtWcNdTTz0lhNi2bVvoO/r9/pycnB49egR3HT9+
3GQyNfXdBwAAiDxGJAEAWpS777579+7dwauDvfHGG5MmTXI4HPVr5s2bt3btWrPZHLiZlJSU
lZUVGIIkhEhOTn711Vffe++9X/7yly+99NIzzzzTrl27Ro+VkJAQXHopOztbCFFUVBTcm52d
XVtbW11draXty3yom2++ucNFPB5PYO+pU6e2bds2btw4WZZd3xk7dmx1dfXOnTvDviBCCLPZ
PH78eC1PJGjcuHHZ32nfvv2YMWOqqqqWLFkyduzYQEHYgwaF7b+Bt956q7q6+p577gncvOuu
u8xm86uvvhq4efbs2S1btowZM8Zo/O9Kkf369XO73cExX1artf4yW/n5+WfOnPleLaWnp48a
NWrlypV+vz9Qv2zZsu7du/fu3Tv0HY8ePXr8+PHhw4cHD5Sdnf295g8CAAA0NxbbBgC0KJMn
T3Y4HK+99lrfvn1LSkq+/vrrZ555pkFNVVXV008/vWLFiiNHjtTW1gohFEWpnxaNGjXqvvvu
+93vfjdy5MiZM2c2dazgIkdCCIPBIIRo1apVgy31p9SFcJkP9eSTT3bp0qXBxttuuy3wxfHj
x4UQzz///PPPP9+g5tixY3379g37gqSnp3/fy949++yzweWEnnjiiU2bNn388cf1V7wOe9Cg
sP032LhgwYLk5OSioqJgADR69OgVK1aUl5enpaWdOHFCCJGRkdFU55mZmZIkBW+aTKZgHqS9
pWnTpr3//vufffbZsGHDSktLS0pKnnjiibB3VFVVCNG6dev623Nycr788sumugUAAIgwgiQA
QItit9unTJmydOnSZ5555o033sjOzh41alSDmgkTJqxfv/7hhx++8cYbU1JSJEm64YYb6hf4
/f6vv/5akqRvvvkmME8qgs/gUgwZMqTBJdKEELJ8wbjje+6557777mtQk5+fLzS8IN83RRJC
DBgwINhSmzZtevfu/b//+7/Lly8PFoQ9aAMh+q9vx44dgfFoOTk5DXb99a9//elPfxp4WS7O
hi5BiJYmTZpkt9vfeeedYcOGLVu2TJKkadOmhb3jgQMHLj6KxiwSAAAgMgiSAAAtzYwZMxYt
WvThhx++/fbbM2bMCAznCdq/f/9nn30WGHAU2OLz+crLyzt06BCsefbZZzdu3Pjee+/deeed
Dz300IIFCy6zJVmWvV5v/S3BpZ0joG3btkIIRVEuDpuEthfkMvXo0WPWrFkvvfTShx9+OHr0
6O970ND9NxD4Zi1durT+IC8hxIwZM1599dWf/vSneXl5QoijR4/W33v48GG73d5gKFAIYVtK
TEycMGHCihUrXnzxxeXLlw8dOjRw3NB3rKqqEhf9bJSWlmrsCgAAIAJYIwkA0NIMHjy4Y8eO
v/nNb86cOTN9+vQGewOBTv05Vi+99JLL5QqO+9i7d++jjz760EMPjR8//vHHH3/llVf++c9/
XmZLqampJ0+eVL+7cNipU6ciOVkpLS2tX79+K1eurKioCG5cvHjxL3/5S5/PF/YFuVhg5leD
y9uH9thjj6WkpPzkJz8JrNwU9qD1DxG6//pHcTqdf/vb3wYOHDh16tSRF5o+ffrOnTs3b97s
cDh69uy5evXq4JpTe/bsad++/V/+8hftT0dLS9OmTTt+/PjKlSu3bNnygx/8QMsd27dvn56e
/sEHHwQHTO3bt2/Hjh3aGwMAAGhuBEkAgJZGkqTp06dv2bKloKCgV69eDfbm5+fn5eUtWLDg
vffeW79+/c9+9rPi4uJhw4bt3r37k08+qaqquvvuu3NycgKXHrv//vsHDhx477331v+z/xJM
nDjxzJkzTz755Lfffrtt27apU6d27Njxch7w+/rDH/5QV1c3dOjQxYsXf/jhh48++ujMmTPL
ysqMRmPoFySwelEDgVljjz/++LvvvquxgfT09Pnz5+/bty9w/bKwB21wiBD91z/K22+/XVlZ
GbjiWwOBtbcXLlwohPj9739/9uzZUaNGLV269JVXXrnpppsyMjJmz559pV7SQMGYMWPS0tIe
eughq9V66623armjLMv333//gQMHpkyZUlxc/PLLL48ePfqaa675Xo0BAAA0L70vGwcAwBUQ
yH2CF4M/ePCgJEl//OMfgwX9+/e/7rrrAl+XlJQMHDjQbrdnZmbOnj27srJy1apV6enpqamp
gQxi7dq1wTvu2rXLZDJNnz5dvfDq7yNGjGjXrl2w7NChQ0KI3//+98EtDz/8sBDi3Llzqqq6
3e4HH3wwNzfXYrEUFBSsWrVq7ty5DofjEh6q0Se+YcOGi3dZLJYRI0YEb65bt27UqFEOh8Nk
MnXp0uUPf/iD1+sN+4Ls3bu3QXuqqh49erSwsNBkMgVfDS0teTyerl272my2Q4cOhT3oxYcI
0X9QUVFRQkJCdXX1xV2pqjpkyBCHw1FTU6Oq6po1awYMGGC32zMyMiZPnrxv375AzcVPNvAj
Efi6/g+AlpZmzZolhJgyZUqDTkLc0efz/eIXv8jKyjKbzT179lyxYsWPf/xjs9nc6DMCAACI
PEn9bpg9AAAAAAAAEAJT2wAAAAAAAKAJQRIAAAAAAAA0IUgCAAAAAACAJgRJAAAAAAAA0IQg
CQAAAAAAAJoQJAEAAAAAAEATgiQAAAAAAABoQpAEAAAAAAAATQiSAAAAAAAAoAlBEgAAAAAA
ADQhSAIAAAAAAIAm/x/4qKa4uxAhGAAAAABJRU5ErkJggg==" width="780">
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=0196f850-e0b1-4e76-a93c-1e91d257189c">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><em>Plot 3: Plotting the two highest accuracy estimate predictors</em></p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=3f04a107-0ba7-425b-b454-80e3f2cee131">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Now that we have found the best accuracy estimate predictors to use, we will begin our cross-validation by splitting our data into a training and testing set.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=599d1198-2c4e-4819-9aec-5bac385eae56">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[99]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">set</span><span class="o">.</span><span class="n">seed</span><span class="p">(</span><span class="mi">27</span><span class="p">)</span>
<span class="n">hd_keep</span> <span class="o">&lt;-</span> <span class="n">select</span><span class="p">(</span><span class="n">heart_disease_hungarian</span><span class="p">,</span> <span class="n">maximum_heart_rate_achieved</span><span class="p">,</span> <span class="n">cholesterol</span><span class="p">,</span><span class="n">heart_disease_cases</span><span class="p">)</span>

<span class="n">hd_split</span> <span class="o">&lt;-</span> <span class="n">initial_split</span><span class="p">(</span><span class="n">hd_keep</span><span class="p">,</span> <span class="n">prop</span> <span class="o">=</span> <span class="mf">0.75</span><span class="p">,</span> <span class="n">strata</span> <span class="o">=</span> <span class="n">heart_disease_cases</span><span class="p">)</span>
<span class="n">hd_train</span> <span class="o">&lt;-</span> <span class="n">training</span><span class="p">(</span><span class="n">hd_split</span><span class="p">)</span>   
<span class="n">hd_test</span> <span class="o">&lt;-</span> <span class="n">testing</span><span class="p">(</span><span class="n">hd_split</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=3eb286bf-e7b5-4818-a123-d8db8f2678d4">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>We use vfold to split the training data for cross validation and a recipe that specifies our target and predictor variables with scaling.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=8d0cb6d0-0673-4570-914c-73eda7cdc895">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[41]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">hd_vfold</span> <span class="o">&lt;-</span> <span class="n">vfold_cv</span><span class="p">(</span><span class="n">hd_train</span><span class="p">,</span> <span class="n">v</span> <span class="o">=</span> <span class="mi">5</span><span class="p">,</span> <span class="n">strata</span> <span class="o">=</span> <span class="n">heart_disease_cases</span><span class="p">)</span>

<span class="n">hd_recipe</span> <span class="o">&lt;-</span> <span class="n">recipe</span><span class="p">(</span><span class="n">heart_disease_cases</span> <span class="o">~</span> <span class="n">maximum_heart_rate_achieved</span> <span class="o">+</span> <span class="n">cholesterol</span><span class="p">,</span> <span class="n">data</span> <span class="o">=</span> <span class="n">hd_train</span><span class="p">)</span> <span class="o">|&gt;</span>
              <span class="n">step_scale</span><span class="p">(</span><span class="n">all_predictors</span><span class="p">())</span> <span class="o">|&gt;</span>
              <span class="n">step_center</span><span class="p">(</span><span class="n">all_predictors</span><span class="p">())</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=616e6df5-af2b-4fa7-9a6c-a4518a0eedd2">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>We now create a nearest neighbors workflow using our previously created recipe and model to estimate our classifiers accuacy for selected K values.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=87f60c45-c478-47bf-864b-b31c3e5d49b7">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[101]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">knn_spec</span> <span class="o">&lt;-</span> <span class="n">nearest_neighbor</span><span class="p">(</span><span class="n">weight_func</span> <span class="o">=</span> <span class="s2">"rectangular"</span><span class="p">,</span> <span class="n">neighbors</span> <span class="o">=</span> <span class="n">tune</span><span class="p">())</span> <span class="o">|&gt;</span>
            <span class="n">set_engine</span><span class="p">(</span><span class="s2">"kknn"</span><span class="p">)</span> <span class="o">|&gt;</span>
            <span class="n">set_mode</span><span class="p">(</span><span class="s2">"classification"</span><span class="p">)</span>

<span class="n">knn_results</span> <span class="o">&lt;-</span> <span class="n">workflow</span><span class="p">()</span> <span class="o">|&gt;</span>
                 <span class="n">add_recipe</span><span class="p">(</span><span class="n">hd_recipe</span><span class="p">)</span> <span class="o">|&gt;</span>
                 <span class="n">add_model</span><span class="p">(</span><span class="n">knn_spec</span><span class="p">)</span> <span class="o">|&gt;</span>
                 <span class="n">tune_grid</span><span class="p">(</span><span class="n">resamples</span> <span class="o">=</span> <span class="n">hd_vfold</span><span class="p">,</span> <span class="n">grid</span> <span class="o">=</span> <span class="n">tibble</span><span class="p">(</span><span class="n">neighbors</span> <span class="o">=</span> <span class="n">c</span><span class="p">(</span><span class="mi">2</span><span class="p">,</span><span class="mi">3</span><span class="p">,</span><span class="mi">4</span><span class="p">,</span><span class="mi">5</span><span class="p">,</span><span class="mi">6</span><span class="p">,</span><span class="mi">7</span><span class="p">,</span><span class="mi">8</span><span class="p">,</span><span class="mi">9</span><span class="p">,</span><span class="mi">10</span><span class="p">)))</span> <span class="o">|&gt;</span>
                 <span class="n">collect_metrics</span><span class="p">()</span> <span class="o">|&gt;</span>
                 <span class="nb">filter</span><span class="p">(</span><span class="o">.</span><span class="n">metric</span> <span class="o">==</span> <span class="s1">'accuracy'</span><span class="p">)</span>

<span class="n">knn_results</span>
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
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output" data-mime-type="text/html" tabindex="0">
<table class="dataframe">
<caption>A tibble: 9 × 7</caption>
<thead>
<tr><th scope="col">neighbors</th><th scope="col">.metric</th><th scope="col">.estimator</th><th scope="col">mean</th><th scope="col">n</th><th scope="col">std_err</th><th scope="col">.config</th></tr>
<tr><th scope="col">&lt;dbl&gt;</th><th scope="col">&lt;chr&gt;</th><th scope="col">&lt;chr&gt;</th><th scope="col">&lt;dbl&gt;</th><th scope="col">&lt;int&gt;</th><th scope="col">&lt;dbl&gt;</th><th scope="col">&lt;chr&gt;</th></tr>
</thead>
<tbody>
<tr><td>2</td><td>accuracy</td><td>binary</td><td>0.5919512</td><td>5</td><td>0.02347474</td><td>Preprocessor1_Model1</td></tr>
<tr><td>3</td><td>accuracy</td><td>binary</td><td>0.6668293</td><td>5</td><td>0.01594556</td><td>Preprocessor1_Model2</td></tr>
<tr><td>4</td><td>accuracy</td><td>binary</td><td>0.6668293</td><td>5</td><td>0.01594556</td><td>Preprocessor1_Model3</td></tr>
<tr><td>⋮</td><td>⋮</td><td>⋮</td><td>⋮</td><td>⋮</td><td>⋮</td><td>⋮</td></tr>
<tr><td> 8</td><td>accuracy</td><td>binary</td><td>0.7015854</td><td>5</td><td>0.017181278</td><td>Preprocessor1_Model7</td></tr>
<tr><td> 9</td><td>accuracy</td><td>binary</td><td>0.6914634</td><td>5</td><td>0.006852639</td><td>Preprocessor1_Model8</td></tr>
<tr><td>10</td><td>accuracy</td><td>binary</td><td>0.6914634</td><td>5</td><td>0.006852639</td><td>Preprocessor1_Model9</td></tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=e84b9d39-8ce9-4d5b-8625-48654d64e272">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><em>Table 5: Workflow with recipe and model to find accuarcy estimates using different K values</em></p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=89980179-9828-4049-a997-0413df243e6c">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Next, we plot our k values against their estimated accuracies in order to choose the most optimal k value.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=eca00f32-3cfc-4c40-b766-4fb5f0ee4829">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[102]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">cross_val_plot</span> <span class="o">&lt;-</span> <span class="n">ggplot</span><span class="p">(</span><span class="n">accuracy</span><span class="p">,</span> <span class="n">aes</span><span class="p">(</span><span class="n">x</span> <span class="o">=</span> <span class="n">neighbors</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="n">mean</span><span class="p">))</span> <span class="o">+</span>
                  <span class="n">geom_point</span><span class="p">()</span> <span class="o">+</span>
                  <span class="n">geom_line</span><span class="p">()</span> <span class="o">+</span>
                  <span class="n">labs</span><span class="p">(</span><span class="n">x</span> <span class="o">=</span> <span class="s1">'Neighbors'</span><span class="p">,</span> <span class="n">y</span> <span class="o">=</span> <span class="s1">'Accuracy Estimate'</span><span class="p">,</span> <span class="n">title</span> <span class="o">=</span> <span class="s2">"Accuracy estimate vs Number of neighbors"</span><span class="p">)</span>

<span class="n">knn_results</span> <span class="o">&lt;-</span> <span class="n">knn_results</span> <span class="o">|&gt;</span> <span class="n">arrange</span><span class="p">(</span><span class="n">mean</span><span class="p">)</span>

<span class="n">cross_val_plot</span>
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
<img alt="No description has been provided for this image" class="" height="420" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAABhgAAANICAMAAAACehXjAAADAFBMVEUAAAABAQECAgIDAwME
BAQFBQUGBgYHBwcICAgJCQkKCgoLCwsMDAwNDQ0ODg4PDw8QEBARERESEhITExMUFBQVFRUW
FhYXFxcYGBgZGRkaGhobGxscHBwdHR0eHh4fHx8gICAhISEiIiIjIyMkJCQlJSUmJiYnJyco
KCgpKSkqKiorKyssLCwtLS0uLi4vLy8wMDAxMTEyMjIzMzM0NDQ1NTU2NjY3Nzc4ODg5OTk6
Ojo7Ozs8PDw9PT0+Pj4/Pz9AQEBBQUFCQkJDQ0NERERFRUVGRkZHR0dISEhJSUlKSkpLS0tM
TExNTU1OTk5PT09QUFBRUVFSUlJTU1NUVFRVVVVWVlZXV1dYWFhZWVlaWlpbW1tcXFxdXV1e
Xl5fX19gYGBhYWFiYmJjY2NkZGRlZWVmZmZnZ2doaGhpaWlqampra2tsbGxtbW1ubm5vb29w
cHBxcXFycnJzc3N0dHR1dXV2dnZ3d3d4eHh5eXl6enp7e3t8fHx9fX1+fn5/f3+AgICBgYGC
goKDg4OEhISFhYWGhoaHh4eIiIiJiYmKioqLi4uMjIyNjY2Ojo6Pj4+QkJCRkZGSkpKTk5OU
lJSVlZWWlpaXl5eYmJiZmZmampqbm5ucnJydnZ2enp6fn5+goKChoaGioqKjo6OkpKSlpaWm
pqanp6eoqKipqamqqqqrq6usrKytra2urq6vr6+wsLCxsbGysrKzs7O0tLS1tbW2tra3t7e4
uLi5ubm6urq7u7u8vLy9vb2+vr6/v7/AwMDBwcHCwsLDw8PExMTFxcXGxsbHx8fIyMjJycnK
ysrLy8vMzMzNzc3Ozs7Pz8/Q0NDR0dHS0tLT09PU1NTV1dXW1tbX19fY2NjZ2dna2trb29vc
3Nzd3d3e3t7f39/g4ODh4eHi4uLj4+Pk5OTl5eXm5ubn5+fo6Ojp6enq6urr6+vs7Ozt7e3u
7u7v7+/w8PDx8fHy8vLz8/P09PT19fX29vb39/f4+Pj5+fn6+vr7+/v8/Pz9/f3+/v7////i
sF19AAAACXBIWXMAABJ0AAASdAHeZh94AAAgAElEQVR4nO3dB5wU9fnH8efu4OggCHbsib0i
NuwYo1FQYwmCng0SIxasaIiFqJCo/DESjaIEWzQGexfRRDQKooANREERPOBurSDSb/5b7o5d
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" width="780">
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=03a5c67b-62e4-4b34-9cc6-2cebcdd576bc">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><em>Plot 4: Plotting neighbors vs accuracy estimate</em></p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=429da339-3c99-40f6-b3a1-c23d5804c1db">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>It appears the most optimal k value is k = 8. We also verify this by analyzing the accuracy estimated results sorted by the mean. Now we can create a new model specification with the best K value and re-train the classifier using fit(). After we have created our new model, we can evaluate the estimated accuracy of the new classifier on the test set using predict().</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=f60093a5-823c-422c-8f7c-b9bf164b67aa">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[72]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">hd_spec</span> <span class="o">&lt;-</span> <span class="n">nearest_neighbor</span><span class="p">(</span><span class="n">weight_func</span> <span class="o">=</span> <span class="s2">"rectangular"</span><span class="p">,</span> <span class="n">neighbors</span> <span class="o">=</span> <span class="mi">5</span><span class="p">)</span> <span class="o">|&gt;</span>
       <span class="n">set_engine</span><span class="p">(</span><span class="s2">"kknn"</span><span class="p">)</span> <span class="o">|&gt;</span>
       <span class="n">set_mode</span><span class="p">(</span><span class="s2">"classification"</span><span class="p">)</span>

<span class="n">hd_fit</span> <span class="o">&lt;-</span> <span class="n">workflow</span><span class="p">()</span> <span class="o">|&gt;</span>
       <span class="n">add_recipe</span><span class="p">(</span><span class="n">hd_recipe</span><span class="p">)</span> <span class="o">|&gt;</span>
       <span class="n">add_model</span><span class="p">(</span><span class="n">hd_spec</span><span class="p">)</span> <span class="o">|&gt;</span>
       <span class="n">fit</span><span class="p">(</span><span class="n">data</span> <span class="o">=</span> <span class="n">hd_train</span><span class="p">)</span>

<span class="n">hd_predictions</span> <span class="o">&lt;-</span> <span class="n">predict</span><span class="p">(</span><span class="n">hd_fit</span> <span class="p">,</span> <span class="n">hd_test</span><span class="p">)</span> <span class="o">|&gt;</span>
       <span class="n">bind_cols</span><span class="p">(</span><span class="n">hd_test</span><span class="p">)</span>

<span class="n">hd_acc</span> <span class="o">&lt;-</span> <span class="n">hd_predictions</span> <span class="o">|&gt;</span> 
    <span class="n">metrics</span><span class="p">(</span><span class="n">truth</span> <span class="o">=</span> <span class="n">heart_disease_cases</span><span class="p">,</span> <span class="n">estimate</span> <span class="o">=</span> <span class="o">.</span><span class="n">pred_class</span><span class="p">)</span> <span class="o">|&gt;</span> 
    <span class="n">select</span><span class="p">(</span><span class="o">.</span><span class="n">metric</span><span class="p">,</span> <span class="o">.</span><span class="n">estimate</span><span class="p">)</span> <span class="o">|&gt;</span> 
    <span class="n">head</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>

<span class="n">hd_cm</span> <span class="o">&lt;-</span> <span class="n">hd_predictions</span> <span class="o">|&gt;</span> 
    <span class="n">conf_mat</span><span class="p">(</span><span class="n">truth</span> <span class="o">=</span> <span class="n">heart_disease_cases</span><span class="p">,</span> <span class="n">estimate</span> <span class="o">=</span> <span class="o">.</span><span class="n">pred_class</span><span class="p">)</span>

<span class="n">hd_acc</span>
<span class="n">hd_cm</span>
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
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output" data-mime-type="text/html" tabindex="0">
<table class="dataframe">
<caption>A tibble: 1 × 2</caption>
<thead>
<tr><th scope="col">.metric</th><th scope="col">.estimate</th></tr>
<tr><th scope="col">&lt;chr&gt;</th><th scope="col">&lt;dbl&gt;</th></tr>
</thead>
<tbody>
<tr><td>accuracy</td><td>0.6231884</td></tr>
</tbody>
</table>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-OutputPrompt jp-OutputArea-prompt"></div>
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>          Truth
Prediction  0  1
         0 33 16
         1 10 10</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=b4b66c91-6763-4fe6-8f2e-4bcdfb70c68c">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><em>Table 6: Classification accuracy</em></p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=218b07b6-c7e3-492a-8977-9765c5edf8e9">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p><em>Table 7: Confusion matrix</em></p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=3ec12379-9759-4bd0-9970-d9760ce0df72">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Our model using the highest estimated accuracy predictors, and the highest estimated accuracy K value, yielded an accuracy estimate of 62%. In our confusion matrix, notice that 33 cases were predicted correctly as negative, while 10 were predicted correctly as positive for heart disease. 16 + 10 = 26 classifications however, were incorrectly predicted.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=715fa90c-a52a-496b-a7a0-2364581b6258">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="Discussion:">Discussion:<a class="anchor-link" href="#Discussion:">¶</a></h3><h4 id="What-did-we-find?">What did we find?<a class="anchor-link" href="#What-did-we-find?">¶</a></h4><h4 id="Is-this-what-we-expected?">Is this what we expected?<a class="anchor-link" href="#Is-this-what-we-expected?">¶</a></h4><h4 id="What-impacts-do-these-findings-have?">What impacts do these findings have?<a class="anchor-link" href="#What-impacts-do-these-findings-have?">¶</a></h4><h4 id="What-future-questions-does-this-lead-to?">What future questions does this lead to?<a class="anchor-link" href="#What-future-questions-does-this-lead-to?">¶</a></h4><h4 id="What-do-we-expect-to-find:">What do we expect to find:<a class="anchor-link" href="#What-do-we-expect-to-find:">¶</a></h4><p>We expect to find associations between heart disease with our chosen predictors. Based on our findings we will be able to identify the most telltale variable for heart disease as well as the relationship predictors may have with one another. We can expect heart disease risk and diagnosis to increase with age, but the same could not be said for the other predictors.</p>
<h4 id="What-impact-do-such-findings-have:">What impact do such findings have:<a class="anchor-link" href="#What-impact-do-such-findings-have:">¶</a></h4><p>Our findings will contribute to identifying portions of the population at higher risk for heart disease based on our predictor variables. This research is done to advocate for health and prevention and to contribute to the current knowledge we have on heart disease.</p>
<h4 id="What-future-questions-could-this-lead-to:">What future questions could this lead to:<a class="anchor-link" href="#What-future-questions-could-this-lead-to:">¶</a></h4><p>Our project leads to many future questions: How can we prevent it within the population, especially if the community doesn't necessarily have the resources for prevention? Also, what other variables other than the ones we have tested could lead to being predisposed to heart disease? Lastly, how much control do patients have over their risk for heart disease and how can they prevent heart disease with this new information?</p>
<h3 id="References:">References:<a class="anchor-link" href="#References:">¶</a></h3><ul>
<li>Ashley, E. A., Raxwal, V., &amp; Froelicher, V. (2001). An evidence-based review of the resting electrocardiogram as a screening technique for heart disease. Progress in Cardiovascular Diseases, 44(1), 55–67. <a href="https://doi.org/10.1053/pcad.2001.24683">https://doi.org/10.1053/pcad.2001.24683</a></li>
<li>He, K., Chen, X., Shi, Z., Shi, S., Tian, Q., Hu, X., Song, R., Bai, K., Shi, W., Wang, J., Li, H., Ding, J., Geng, S., &amp; Sheng, X. (2022). Relationship of resting heart rate and blood pressure with all-cause and cardiovascular disease mortality. Public Health, 208, 80–88. <a href="https://doi.org/10.1016/j.puhe.2022.03.020">https://doi.org/10.1016/j.puhe.2022.03.020</a></li>
<li>Maas, A. H. E. M., &amp; Appelman, Y. E. A. (2010). Gender differences in coronary heart disease. Netherlands Heart Journal, 18(12), 598–603. <a href="https://doi.org/10.1007/s12471-010-0841-y">https://doi.org/10.1007/s12471-010-0841-y</a></li>
<li>Moran, A. E., Tzong, K. Y., Forouzanfar, M. H., Roth, G. A., Mensah, G. A., Ezzati, M., Murray, C. J. L., &amp; Naghavi, M. (2014). Variations in ischemic heart disease burden by age, country, and income: the global burden of diseases, injuries, and risk factors 2010 study. Global Heart, 9(1), 91. <a href="https://doi.org/10.1016/j.gheart.2013.12.007">https://doi.org/10.1016/j.gheart.2013.12.007</a></li>
<li>Park, C., Guallar, E., Linton, J. A., Lee, D.-C., Jang, Y., Son, D. K., Han, E.-J., Baek, S. J., Yun, Y. D., Jee, S. H., &amp; Samet, J. M. (2013). Fasting glucose level and the risk of incident atherosclerotic cardiovascular diseases. Diabetes Care, 36(7), 1988–1993. <a href="https://doi.org/10.2337/dc12-1577">https://doi.org/10.2337/dc12-1577</a></li>
</ul>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=1d18ece7-f811-42e0-9eec-865e29eda4b4">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[&nbsp;]:</div>
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


</body></html>

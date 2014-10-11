ragingwind-seed-element
================

See the [component page](http://ragingwind.github.io/ragingwind-seed-element) for more information.

## Getting Started

We've put together a [guide for ragingwind-seed-element](http://www.polymer-project.org/docs/start/reusableelements.html) to help get you rolling.

## Drawer menu with core-element

- Change path to the element

```
bower install Polymer/core-elements --save
```

- Put `core-` dependecies into top of the raging-seed-element.html

```
<link rel="import" href="../core-scaffold/core-scaffold.html">
<link rel="import" href="../core-toolbar/core-toolbar.html">
<link rel="import" href="../core-header-panel/core-header-panel.html">
<link rel="import" href="../core-menu/core-menu.html">
<link rel="import" href="../core-item/core-item.html">
<link rel="import" href="../core-iconset-svg/core-iconset-svg.html">
```

- Put styles into top of templace code

```
<style>
  .content {
    padding: 20px;
  }
  core-item[icon="polymer"] {
    color: #a4c639;
  }
</style>
```

- Add relevant codes into `content` tag

```
<core-scaffold responsiveWidth="1024px">
  <core-header-panel navigation flex>
    <core-toolbar>Menu</core-toolbar>
    <core-menu>
      <core-item icon="home" label="Home"></core-item>
      <core-item icon="account-box" label="Profile"></core-item>
      <core-item icon="settings" label="Settings"></core-item>
    </core-menu>
  </core-header-panel>
  <div tool>Drawer-Content App</div>
  <div fit class="content">
    Alo, Alo
  </div>
</core-scaffold>
```

